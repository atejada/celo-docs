---
title: Celo CLI
description: The Command Line Interface allows users to interact with the Celo Protocol smart contracts.
sidebar_position: 1
---

# Celo CLI

Introduction to the Celo Command Line Interface and installation instructions.

## What is the Celo CLI {#what-is-the-celo-cli}

The Command Line Interface allows users to interact with the Celo Protocol smart contracts.

It’s a command-line interface for interacting with the Celo Protocol and core contracts. Some common features you may want try include transferring tokens, viewing account balances, participating in elections or in on-chain governance, voting for validators,  or helping users interact with multi-sig contracts.

## Installation {#installation}


### Homebrew {#brew-tap}

If you're on macOS or Linux, celocli is available as a *tap* on Homebrew. 

```bash
brew tap celo-org/brew
brew install celocli

celocli --version
```

### NPM Package {#npm-package}

The Celo CLI is published as a node module on NPM. Assuming you have [npm](https://www.npmjs.com/get-npm) and [git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) both installed, you can install the Celo CLI using the following command:

```bash
npm install -g @celo/celocli
```

If you want the cutting edge, @betas are distributed via npm. `npm install -g @celo/celocli@beta`

:::info

If you have trouble installing globally \(i.e. with the `-g` flag\), try installing to a local directory instead with `yarn add @celo/celocli` and run with `yarn celocli`.

:::

## Commands {#commands}

The tool is broken down into modules and commands with the following pattern:

```text
celocli <module>:<command> <...args> <...flags?>
```

The `celocli` tool assumes that users are running a node which they have access to signing transactions on, or have another mechanism for signing transactions (such as a Ledger wallet or supplying the private key as an argument to the command). See the documentation on the [config](config.md) module for information about how to set which node commands are sent to.

:::info

All balances of CELO or Celo Dollars are expressed in units of 10^-18.

:::

You can find the Celo CLI package on NPM [here](https://www.npmjs.com/package/@celo/celocli).

To see all available commands, run `celocli commands`.

To see all available flags for a command, add the flag `--globalHelp` to the command.

## Optional: Run a Full Node {#optional-run-a-full-node}

Commands need to connect to a Celo node to execute most functionality. You can either use [Forno](/network/node/forno) (this is the easiest way) or run your own full node if you prefer. See the [Running a Full Node](/network/mainnet/run-full-node) instructions for more details on running a full node.

The easiest way to connect `celocli` to the Celo network is by running the following command in your terminal with `celocli` installed:

```bash
celocli config:set --node=https://forno.celo.org
```

You can verify that `celocli` is connected by running

```bash
celocli config:get
```

## Import Accounts {#import-accounts}

If you are connecting to a remote node (like Forno), Celo CLI will need to sign transactions locally before sending them. To do this, Celo CLI needs access to a private key. There are a couple ways to sign transactions using Celo CLI.

### Import Private Key (less secure) {#import-private-key-less-secure}

Add the `--privateKey` flag followed by the private key associated with the sending account. For example:

```shell
celocli transfer:celo --from <accountAddress> --to <addressOfChoice> --value <valueInCeloWei> --privateKey <privateKey> --node https://forno.celo.org
```

Or you can use a Ledger hardware wallet. (preferred, see below)

## Using a Ledger Wallet {#using-a-ledger-wallet}

The Celo CLI supports using a [Ledger hardware wallet](/wallet/ledger/setup) to sign transactions. Just add the `--useLedger` flag to a command that requires a signature.

You can specify the number of addresses to get for local signing with the `--ledgerAddresses` flag.

You can specify an array of index addresses for local signing. Example `--ledgerCustomAddresses "[4,99]"`.

For example:

```shell
celocli transfer:celo --to <addressOfChoice> --value 1000000 --from <accountAddress> --useLedger
```

