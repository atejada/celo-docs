---
title: Deploy with Remix
description: How to deploy a Smart Contract to Celo using remix.ethereum.org.
---

# Deploy on Celo with Remix

How to deploy a smart contract to Celo testnet, Mainnet, or a local network using [Remix](https://remix.ethereum.org/).

:::warning
As of block height 31,056,500 (March 26, 2025, 3:00 AM UTC), Celo is no longer a standalone Layer 1 blockchain—it is now an Ethereum Layer 2!
Some documentation may be outdated as updates are in progress. If you encounter issues, please [file a bug report](https://github.com/celo-org/docs/issues/new/choose).

For the most up-to-date information, refer to our [Celo L2 documentation](https://docs.celo.org/cel2).
:::

---

## Introduction to Remix

The [Remix IDE](https://remix-project.org/) is an open-source web and desktop application for creating and deploying Smart Contracts. Originally created for Ethereum, it fosters a fast development cycle and has a rich set of plugins with intuitive GUIs. Remix is used for the entire journey of contract development and is a playground for learning and teaching Celo.

In this guide, you will learn to deploy a smart contract on Celo using [remix.ethereum.org](http://remix.ethereum.org).

:::warning
For Celo L1 Remix does not support Solidity compiler version `0.8.20` and above for EVM versions above **Paris**. If you try to deploy a smart contract with a higher version, you will receive this error message:


```bash
Gas estimation errored with the following message (see below). The transaction execution will likely fail. Do you want to force sending?

invalid opcode: opcode 0x5f not defined
The EVM version used by the selected environment is not compatible with the compiler EVM version.
```

A **workaround** is to go into the advanced settings for the compiler in Remix and choose Paris as the EVM version.

For Alfajores L2 everything should be working as on every other EVM compatible chain.
:::

:::tip

To learn more about the features available to you as a smart contract developer with Remix, visit the [Remix documentation](https://remix-ide.readthedocs.io/en/latest/).

:::



## Create a Smart Contract

- Navigate to [remix.ethereum.org](http://remix.ethereum.org) and select **contracts > 1_Storage.sol** from the **File Explorers** pane.
- Review the smart contract code and learn more using the [Solidity docs](https://docs.soliditylang.org/en/latest/) or with [Solidity by Example](https://solidity-by-example.org/).
- Complete any changes to your smart contract and save the final version (Command/Ctrl + S).

![github](/img/doc-images/deploy-remix/image1.png)

## Compile the Contract

- Choose the **Solidity Compiler Icon** on the left side menu.
- Check that your compiler version is within the versions specified in the **pragma solidity statement**.
- Select the **Compile** button to compile your smart contract.

![github](/img/doc-images/deploy-remix/image2.png)

## Deploy the Contract

- Click the **Deploy and Run Transactions Icon** on the left side menu.
- Choose **Injected Web3** as your environment.
- [Connect MetaMask to Celo](/wallet/metamask/use) testnet and verify that the environment reads:
  - **Custom (44787) network** for Celo Alfajores testnet
  - **Custom (42220) network** for Celo Mainnet
- Click **Deploy** and select **Confirm** in the MetaMask notification window to pay for the transaction

![github](/img/doc-images/deploy-remix/image3.png)

## Interacting with the Contract

- Select the **dropdown** on the newly deployed contract at the bottom of the left panel.
- View the deployed contract’s functions using the **Deployed Contracts** window.
- Select functions to read or write on the Celo testnet using the function inputs as needed.
- Confirm write transactions in the **MetaMask Notification Window** to pay the transaction’s gas fee.

![github](/img/doc-images/deploy-remix/image4.png)

## View Contract Details

- Copy the contract address from the **Deployed Contracts** window on the left panel.
- Navigate to the [Celo Block Explorer](https://explorer.celo.org/) and use the contract address to search for your contract.
- Explore the details of your deployed smart contract and learn more about the explorer [here](http://docs.blockscout.com).

![github](/img/doc-images/deploy-remix/image6.png)

## Verify Contracts on Celo

- [Using Blockscout](/developer/verify/blockscout)
- [Using Remix](/developer/verify/remix)
- [Using CeloScan](/developer/verify/celoscan)
- [Using Hardhat](/developer/verify/hardhat)
