---
title: Recover ETH or ERC-20 tokens from a Celo address
description: How to recover ETH or ERC-20 tokens if you accidentally transferred them to a CELO (previously Celo Gold) address.
---

# Recover ETH or ERC-20 tokens from a Celo address

How to recover ETH or ERC-20 tokens if you accidentally transferred them to a CELO (previously Celo Gold) address.

:::warning
As of block height 31,056,500 (March 26, 2025, 3:00 AM UTC), Celo is no longer a standalone Layer 1 blockchain—it is now an Ethereum Layer 2!
Some documentation may be outdated as updates are in progress. If you encounter issues, please [file a bug report](https://github.com/celo-org/docs/issues/new/choose).

For the most up-to-date information, refer to our [Celo L2 documentation](https://docs.celo.org/cel2).
:::

---

## Prerequisites

This guide assumes that you have access to the following:

- The [24-word recovery phrase](https://help.myetherwallet.com/en/?q=mnemonic) of your Celo address
- An Ethereum wallet manager such as MyEtherWallet or MyCrypto. It is recommended to use the Desktop or offline version over a webapp version.

:::danger

There are [risks](https://www.cryptomathic.com/news-events/blog/cryptographic-key-management-the-risks-and-mitigations) associated with using a recovery phrase or a private key. Please do not share them with anyone else.

:::

## Steps

Please follow the instructions below closely because missteps can lead to errors or permanent loss of your tokens. To understand these steps, please read [What is Ethereum](https://ethereum.org/en/what-is-ethereum/) and [Celo Overview](/general/).

### MyEtherWallet

1. [Download and run MEW Offline](https://help.myetherwallet.com/en/articles/6512619-using-mew-offline) (scroll down until you see the download instructions)
2. Open MEW and click on **Access My Wallet > Software > Mnemonic Phrase > Continue**
3. Change to a 24 Value mnemonic and enter in the words from your Recovery Phrase. Then click **Continue**
4. Change the HD Derivation Path to **Add Custom path**
5. Call your Alias "Celo" for easy reference. Enter in your Path as `m/44'/52752'/0'/0`. Click **Add Custom Path.**
6. Go back to your Derivation Path dropdown and select **Celo (m/44'/52752'/0'/0)**. You should see the addresses change. Select the address that matches your Valora Account Number (it's usually the first one).
7. Accept the Terms
8. Click **Access My Wallet**
9. Now you can send your token back to your original address:
   1. Click on **Send Transaction**
   2. Fill in the **Type, Amount,** and **To Address**.
   3. Confirm that the information is correct and you have enough funds to cover any fees.
   4. Click **Send Transaction**.

### MyCrypto

1. [Download](https://app.mycrypto.com/download-desktop-app) then open the MyCrypto desktop app and click on **View & Send**
2. Access using **Mnemonic Phrase**
3. Enter in your Valora Recovery Phrase into the Mnemonic Phrase box (tip: click the eye icon to easily see your phrase) the click **Choose address**
4. Change the **Address** from "Default (ETH)" to "Custom". Enter `m/44'/52752'/0'/0` into the box that pops up next to it.
5. Select the address that matches your Valora Account number (it's usually the first one).
6. Click **Unlock**
7. Scroll down and look for a button that says **Scan For Tokens**. Click it.
8. You should be able to see your token.
9. Now you can send your token back to your original address:
   1. Enter your address in the **To Address** box
   2. Change the currency.
   3. Fill in the **Amount** or click the "double up-arrow" icon to send your entire balance.
   4. Confirm that the information is correct and you have enough funds to cover any fees.
   5. Click **Send Transaction**
