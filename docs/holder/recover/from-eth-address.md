---
title: Recover CELO from an Ethereum Address
description: How to recover CELO (previously Celo Gold) if you accidentally transferred them to an account generated using an Ethereum wallet.
---

# Recover CELO from an Ethereum Address

How to recover [CELO (previously Celo Gold)](/general/) if you accidentally transferred them to an account generated using an Ethereum wallet.

:::warning
As of block height 31,056,500 (March 26, 2025, 3:00 AM UTC), Celo is no longer a standalone Layer 1 blockchain—it is now an Ethereum Layer 2!
Some documentation may be outdated as updates are in progress. If you encounter issues, please [file a bug report](https://github.com/celo-org/docs/issues/new/choose).

For the most up-to-date information, refer to our [Celo L2 documentation](https://docs.celo.org/cel2).
:::

:::note

You only need to go through this process when going from mnemonic (secret phrase) to account because of the different account derivation paths between Celo and Ethereum. This is only relevant if you're using a wallet that can’t connect to both the Ethereum and Celo networks or you can’t export the private key. Private key--account pairs are the same for both Celo and Ethereum, it's just menemonic (secret phrase) to private keys that are different.

With Metamask, recovery is easy because you just switch Metamask to the network where the funds are--the accounts and private keys for both networks are the same. The problem occurs when the wallet only accepts the secret phrase and derives private keys and accounts differently based on the network it is designed for.

:::

---

## Prerequisites

This guide assumes you have access to the recipient's mnemonic recovery phrase (note, in Valora and Celo Wallet it's called your 'Recovery Phrase').

:::danger

There are [risks](https://www.cryptomathic.com/news-events/blog/cryptographic-key-management-the-risks-and-mitigations) associated with using a recovery phrase or a private key. Please keep these secret.

:::

## Recovering with CeloWallet.app

The Celo Wallet for Web and Desktop can be used to import mnemonic phrases with custom derivation paths (like Ethereum's) in order to recover your funds.

### Steps to access funds

1. Visit [celowallet.app](https://celowallet.app) in a modern browser (Chrome is recommended).
2. For small accounts, you can import in the web version directly. For larger accounts, downloading the desktop version is **strongly** recommended.
3. Click 'Use Existing Account', then 'Use Recovery Phrase', then choose the 'Advanced' tab.
4. Specify your deriviation path and click import.
5. Set a strong password and click Continue. You should reach the home screen and see your account funds.

![](https://storage.googleapis.com/celo-website/docs/celo-wallet-advanced-import-screen.png)

### Steps to migrate funds

Once you've been able to access your funds, it's recommended that you move them to an account derived from the Celo derivation path.

1. Create a new account: you can use the celowallet.app again, Valora, the Celo CLI, or any other wallets compatible with Celo.
2. Copy the address of your new account
3. In the first Celo Wallet window, click the Send button in the top-left.
4. Send your funds to your new account.
5. If you intend to keep this new account permanently, be sure to save its password and recovery phrase in a safe place!

## Recovering with the Celo CLI

### Prerequisites

This guide assumes that you have access to the following:

- A computer with a [Command Line Interface](https://wikipedia.org/wiki/Command-line_interface). You can access it following these instructions:
  - [Windows](https://www.howtogeek.com/270810/how-to-quickly-launch-a-bash-shell-from-windows-10s-file-explorer/)
  - [Mac](https://macpaw.com/how-to/use-terminal-on-mac)
  - [Linux](https://askubuntu.com/questions/196212/how-do-you-open-a-command-line)
- [Celo Command Line Interface](/cli/) installed on your computer
- The [24-word recovery phrase](https://help.myetherwallet.com/en/?q=mnemonic) of your Ethereum address

### Steps

Please follow the instructions below closely, because missteps can lead to errors or permanent loss of your tokens. To understand these steps, please read [What is Ethereum](https://ethereum.org/en/what-is-ethereum/) and [Celo Overview](/general/).

#### Prepare your recovery phases

Write your recovery phrase to a file using the following commands:

1. `nano recovery.txt`
2. Paste `<word1> <word2> … <word24>`
3. Replace the `<word>`s in brackets with the words from your recovery phrase (usually 24 words, but can be 12, 15, 18, 21 or 24 words, as specified in the [BIP 39 standard](https://github.com/bitcoin/bips/blob/master/bip-0039.mediawiki)
4. Press ctrl-o to save
5. Press ctrl-x to exit

#### Recover your Ethereum address on Celo

Recover your Ethereum address on the Celo network:

```
celocli account:new --mnemonicPath recovery.txt --derivationPath "eth" --node https://forno.celo.org
```

This command will return you with:

- `accountAddress`: the same address as your Ethereum address
- `privateKey`: the private key associated with your address -- please record this private key on paper and not share with anyone else
- `publicKey`: the public key associated with your address

**_Note_**

Using the `eth` derivation path as above will work for the default Ethereum path used by nearly all Ethereum wallets (`"m/44'/60'/0'/0/0"`). If your address was generated using a different derivation path you can specify that using a combination of the flags `addressIndex`, `changeIndex` and `derivationPath`.

For example, for the address corresponding to the path `m/44'/78'/1'/4/23` use:

```
celocli account:new --mnemonicPath recovery.txt --derivationPath "m/44'/78'/1'" --changeIndex 4 --addressIndex 23 --node https://forno.celo.org
```

#### Check your CELO balanace

Check your Celo account balance using this command:

```
celocli account:balance <accountAddress> --node https://forno.celo.org
```

Replace `<accountAddress>` with the `accountAddress` you got from the previous step.

#### Transfer CELO

Now, you can transfer your CELO to an address of choice:

```
celocli transfer:celo --from <accountAddress> --to <addressOfChoice> --value <valueInCeloWei> --privateKey <privateKey> --node https://forno.celo.org
```

- Replace `<accountAddress>` with the `accountAddress` you got from the previous step.
- Replace `<addressOfChoice>` with the address that you want to send CELO to.
- Replace `<valueInCeloWei>` with the amount you want to send, but this number needs to be slightly lower than your balance, as there’s a transaction fee.

:::info

Note that the value has a unit of CELO Wei (1 CELO = 10^18 CELO Wei), so if you want to send 1 CELO, the `<valueInCeloWei>` should be 1000000000000000000.

:::
