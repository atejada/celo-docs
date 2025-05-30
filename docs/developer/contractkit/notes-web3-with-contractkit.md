---
title: Using Web3 from ContractKit with Celo
description: How to use Web3 from ContractKit to read data from the Celo blockchain.
---

# Using Web3 from ContractKit

How to use Web3 from ContractKit to read data from the Celo blockchain.

---

:::warning
As of block height 31,056,500 (March 26, 2025, 3:00 AM UTC), Celo is no longer a standalone Layer 1 blockchain—it is now an Ethereum Layer 2!
Some documentation may be outdated as updates are in progress. If you encounter issues, please [file a bug report](https://github.com/celo-org/docs/issues/new/choose).

For the most up-to-date information, refer to our [Celo L2 documentation](https://docs.celo.org/cel2).
:::

The ContractKit, for every interaction with the node, uses internally a Web3 instance.

Because of this, the `Ethereum` JSON-RPC calls done via the web3 (except some specific calls that we will explain in this page) are also supported

For example:

```ts
const web3 = kit.web3;

web3.eth.getBalance(someAddress);
```

or

```ts
const web3 = kit.web3;

web3.eth.getBlock("latest");
```

will work the same way.

## Web3 limitations

As you have read in our guide, Celo uses an extra field: `feeCurrency`, that allows you to pay gas with ERC20 Tokens.

To facilitate the life of every developer, we decided to wrap the `Provider` set in the `Web3` instance, and add our way to handle local signing using these new fields. Similar to what _Metamask_ does, we intercept every transaction and perform a local signing when required. This wrapper is called `CeloProvider`.

This let you use the Web3 instance to interact with node's Json RPC API in a transparent way, just deciding which Provider do you need.

This is also the reason that the `Kit` requires a valid provider from the beginning.


