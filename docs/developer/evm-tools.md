---
title: Celo EVM Compatible Tooling
description: Overview of Celo EVM-compatible tools and the value they provide to developers.
---

# Developer Tools

A guide to available tools, components, patterns, and platforms for developing applications on EVM-compatible chains.

:::warning
As of block height 31,056,500 (March 26, 2025, 3:00 AM UTC), Celo is no longer a standalone Layer 1 blockchain—it is now an Ethereum Layer 2!
Some documentation may be outdated as updates are in progress. If you encounter issues, please [file a bug report](https://github.com/celo-org/docs/issues/new/choose).

For the most up-to-date information, refer to our [Celo L2 documentation](https://docs.celo.org/cel2).
:::

---

## New developers start here

- [Solidity](https://soliditylang.org/) - The most popular smart contract language.
- [Metamask](https://metamask.io/) - Browser extension wallet to interact with Dapps.
- [thirdweb](https://thirdweb.com) - SDKs in every language, smart contracts, tools, and infrastructure for web3 development.
- [Hardhat](https://hardhat.org/) - Flexible, extensible and fast Ethereum development environment.
- [Cryptotux](https://cryptotux.org/) - A Linux image ready to be imported in VirtualBox that includes the development tools mentionned above
- [EthereumDev.io](https://ethereumdev.io) - The definitive guide for getting started with Ethereum smart contract programming.
- [Brownie](https://github.com/iamdefinitelyahuman/brownie) - Brownie is a Python framework for deploying, testing and interacting with Ethereum smart contracts.
- [Ethereum Stack Exchange](https://ethereum.stackexchange.com/) - Post and search questions to help your development life cycle.
- [dfuse](https://dfuse.io) - Slick blockchain APIs to build world-class applications.
- [Biconomy](https://biconomy.io) - Do gasless transactions in your dapp by enabling meta-transactions using simple to use SDK.
- [Blocknative](https://blocknative.com) — Blockchain events before they happen. Blocknative's portfolio of developers tools make it easy to build with mempool data.
- [useWeb3.xyz](https://useweb3.xyz/) — A curated overview of the best and latest resources on Ethereum, blockchain and Web3 development.

## Developing Smart Contracts

### Smart Contract Languages

- [Solidity](https://docs.soliditylang.org/en/latest/) - Ethereum smart contracting language
- [Vyper](https://vyper.readthedocs.io/en/latest/) - New experimental pythonic programming language

### Frameworks

- [thirdweb](https://portal.thirdweb.com/contracts/build/get-started) - Provides the tools needed to build custom smart contracts efficiently by offering a set of prebuilt base contracts and a set of reusable components, or extensions, that can be integrated into your own smart contracts.
- [Hardhat](https://hardhat.org/) - Flexible, extensible and fast Ethereum development environment.
- [Embark](https://github.com/embark-framework/embark) - Framework for DApp development
- [Dapp](https://dapp.tools/dapp/) - Framework for DApp development, successor to DApple
- [Etherlime](https://github.com/LimeChain/etherlime) - ethers.js based framework for Dapp deployment
- [Parasol](https://github.com/Lamarkaz/parasol) - Agile smart contract development environment with testing, INFURA deployment, automatic contract documentation and more. It features a flexible and unopinionated design with unlimited customizability
- [0xcert](https://github.com/0xcert/framework/) - JavaScript framework for building decentralized applications
- [OpenZeppelin SDK](https://openzeppelin.com/sdk/) - OpenZeppelin SDK: A suite of tools to help you develop, compile, upgrade, deploy and interact with smart contracts.
- [sbt-ethereum](https://sbt-ethereum.io/) - A tab-completey, text-based console for smart-contract interaction and development, including wallet and ABI management, ENS support, and advanced Scala integration.
- [Cobra](https://github.com/cobraframework/cobra) - A fast, flexible and simple development environment framework for Ethereum smart contract, testing and deployment on Ethereum virtual machine(EVM).

### IDEs

- [Remix](https://remix.ethereum.org/) - Web IDE with built in static analysis, test blockchain VM.
- [Ethereum Studio](https://github.com/SuperblocksHQ/ethereum-studio?tab=readme-ov-file) - Web IDE. Built in browser blockchain VM, Metamask integration (one click deployments to Testnet/Mainnet), transaction logger and live code your WebApp among many other features.
- [Vim solidity](https://github.com/tomlion/vim-solidity) - Vim syntax file for solidity
- [Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=JuanBlanco.solidity) - Visual Studio Code extension that adds support for Solidity
- [Ethcode](https://marketplace.visualstudio.com/items?itemName=7finney.ethcode) - Visual Studio Code extension to compile, execute & debug Solidity & Vyper programs
- [Intellij Solidity Plugin](https://github.com/intellij-solidity/intellij-solidity/wiki) - Open-source plug-in for [JetBrains IntelliJ Idea IDE](https://jetbrains.com/idea/) (free/commercial) with syntax highlighting, formatting, code completion etc.

## Other tools

- [Atra Blockchain Services](https://console.atra.io) - Atra provides web services to help you build, deploy, and maintain decentralized applications on the Ethereum blockchain.

## Test Blockchain Networks

- [ethnode](https://github.com/vrde/ethnode) - Run an Ethereum node (Geth or Parity) for development, as easy as `npm i -g ethnode && ethnode`.
- [Kaleido](https://kaleido.io/) - Use Kaleido for spinning up a consortium blockchain network. Great for PoCs and testing
- [Besu Private Network](https://besu.hyperledger.org/private-networks/tutorials/azure) - Run a private network of Besu nodes in a Docker container
  **[Orion](https://github.com/PegaSysEng/orion) - Component for performing private transactions by PegaSys
  ** [Artemis](https://github.com/PegaSysEng/artemis) - Java implementation of the Ethereum 2.0 Beacon Chain by PegaSys
- [Cliquebait](https://github.com/f-o-a-m/cliquebait) - Simplifies integration and accepting testing of smart contract applications with docker instances that closely resembles a real blockchain network
- [Local Raiden](https://github.com/ConsenSys/Local-Raiden) - Run a local Raiden network in docker containers for demo and testing purposes
- [Private networks deployment scripts](https://github.com/ConsenSys/private-networks-deployment-scripts) - Out-of-the-box deployment scripts for private PoA networks
- [Local Ethereum Network](https://github.com/ConsenSys/local_ethereum_network) - Out-of-the-box deployment scripts for private PoW networks
- [Ethereum on Azure](https://docs.microsoft.com/en-us/azure/blockchain/templates/ethereum-poa-deployment) - Deployment and governance of consortium Ethereum PoA networks
- [Infura](https://infura.io/) - Ethereum API access to Ethereum networks (Mainnet, Ropsten, Rinkeby, Goerli, Kovan)
- [CloudFlare Distributed Web Gateway](https://cloudflare.com/distributed-web-gateway/) - Provides access to the Ethereum network through the Cloudflare instead of running your own node
- [Chainstack](https://chainstack.com/) - Shared and dedicated Ethereum nodes as a service (Mainnet, Ropsten)
- [Alchemy](https://alchemyapi.io/) - Blockchain Developer Platform, Ethereum API, and Node Service (Mainnet, Ropsten, Rinkeby, Goerli, Kovan)
- [Watchdata](https://watchdata.io) - Provide simple and reliable API access to Ethereum blockchain

### Alternative Celo Faucet

- [LearnWeb3 Faucet](https://learnweb3.io/faucets)

### Test Ether Faucets

- [Rinkeby faucet](https://rinkebyfaucet.io/)
- [Kovan faucet](https://github.com/kovan-testnet/faucet)
- [Sepolia faucet](https://www.sepoliafaucet.io/)
- [Nethereum.Faucet](https://github.com/Nethereum/Nethereum.Faucet) - A C#/.NET faucet

## Communicating with Ethereum

### Frontend Ethereum APIs

- [thirdweb](https://thirdweb.com) - Build web3 applications that can interact with your smart contracts using our powerful SDKs.
- [Web3.js](https://github.com/ethereum/web3.js/) - Javascript Web3
- [Eth.js](https://github.com/ethjs) - Javascript Web3 alternative
- [Ethers.js](https://github.com/ethers-io/ethers.js/) - Javascript Web3 alternative, useful utilities and wallet features
- [useDApp](https://usedapp.io) - React based framework for rapid DApp development on Ethereum
- [Ethereumjs](https://github.com/ethereumjs/) - A collection of utility functions for Ethereum like [ethereumjs-util](https://github.com/ethereumjs/ethereumjs-util) and [ethereumjs-tx](https://github.com/ethereumjs/ethereumjs-tx)
- [Alchemy-web3.js](https://github.com/alchemyplatform/alchemy-web3) - Javascript Web3 wrapper with automatic retries, access to [Alchemy's enhanced APIs](https://docs.alchemyapi.io/documentation/alchemy-web3/enhanced-web3-api), and robust websocket connections.
- [flex-contract](https://github.com/merklejerk/flex-contract) and [flex-ether](https://github.com/merklejerk/flex-ether) - Modern, zero-configuration, high-level libraries for interacting with smart contracts and making transactions.
- [ez-ens](https://github.com/merklejerk/ez-ens) - Simple, zero-configuration Ethereum Name Service address resolver.
- [web3x](https://github.com/xf00f/web3x) - A TypeScript port of web3.js. Benefits includes tiny builds and full type safety, including when interacting with contracts.
- [Nethereum](https://github.com/Nethereum/) - Cross-platform Ethereum development framework
- [dfuse](https://github.com/dfuse-io/client-js) - A TypeScript library to use [dfuse Ethereum API](https://dfuse.io)
- [Tasit SDK](https://github.com/tasitlabs/tasitsdk) - A JavaScript SDK for making native mobile Ethereum dapps using React Native
- [useMetamask](https://github.com/mdtanrikulu/use-metamask) - a custom React Hook to manage Metamask in Ethereum ĐApp projects
- Strictly Typed - Javascript alternatives
  - [elm-ethereum](https://github.com/cmditch/elm-ethereum)
  - [purescript-web3](https://github.com/f-o-a-m/purescript-web3)
- [ChainAbstractionLayer](https://github.com/liquality/chainify) - Communicate with different blockchains (including Ethereum) using a single interface.
- [Delphereum](https://github.com/svanas/delphereum) - a Delphi interface to the Ethereum blockchain that allows for development of native dApps for Windows, macOS, iOS, and Android.
- [Torus](https://tor.us/) - Open-sourced SDK to build dapps with a seamless onboarding UX
- [Fortmatic](https://fortmatic.com/) - A simple to use SDK to build web3 dApps without extensions or downloads.
- [Portis](https://portis.io/) - A non-custodial wallet with an SDK that enables easy interaction with DApps without installing anything.
- [create-eth-app](https://github.com/paulrberg/create-eth-app) - Create Ethereum-powered front-end apps with one command.
- [Scaffold-ETH-2](https://github.com/scaffold-eth/scaffold-eth-2) - Beginner friendly forkable github for getting started building smart contracts.
- [Notify.js](https://www.blocknative.com/blog/notify-api) - Deliver real-time notifications to your users. With built-in support for Speed-Ups and Cancels, Blocknative Notify.js helps users transact with confidence. Notify.js is easy to integrate and quick to customize.

### Backend Ethereum APIs

- [thirdweb](https://thirdweb.com) - Build web3 applications that can interact with your smart contracts using our powerful SDKs.
- [Web3.py](https://github.com/ethereum/web3.py) - Python Web3
- [Web3.php](https://github.com/web3p/web3.php) - PHP Web3
- [Ethereum-php](https://github.com/digitaldonkey/ethereum-php) - PHP Web3
- [Web3j](https://github.com/web3j/web3j) - Java Web3
- [Nethereum](https://nethereum.com/) - .Net Web3
- [Ethereum.rb](https://github.com/EthWorks/ethereum.rb) - Ruby Web3
- [rust-web3](https://github.com/tomusdrw/rust-web3) - Rust Web3
- [Web3.hs](https://hackage.haskell.org/package/web3) - Haskell Web3
- [KEthereum](https://github.com/komputing/KEthereum) - Kotlin Web3
- [Eventeum](https://github.com/ConsenSys/eventeum) - A bridge between Ethereum smart contract events and backend microservices, written in Java by Kauri
- [Ethereumex](https://github.com/mana-ethereum/ethereumex) - Elixir JSON-RPC client for the Ethereum blockchain
- [Ethereum-jsonrpc-gateway](https://github.com/HydroProtocol/ethereum-jsonrpc-gateway) - A gateway that allows you to run multiple Ethereum nodes for redundancy and load-balancing purposes. Can be run as an alternative to (or on top of) Infura. Written in Golang.
- [EthContract](https://github.com/zyield/eth_contract) - A set of helper methods to help query ETH smart contracts in Elixir
- [Ethereum Logging Framework](https://bitbucket.csiro.au/users/kli039/repos/ethereum-logging-framework/browse) - provides advanced logging capabilities for Ethereum applications and networks including a query language, query processor, and logging code generation
- [Watchdata](https://watchdata.io) - Provide simple and reliable API access to Ethereum blockchain

### Bootstrap/Out-of-Box tools

- [Create Eth App](https://github.com/paulrberg/create-eth-app) - Create Ethereum-powered frontend apps with one command
- [Besu Private Network](https://besu.hyperledger.org/private-networks/tutorials/azure) - Run a private network of Besu nodes in a Docker container
- [Testchains](https://github.com/Nethereum/TestChains) - Pre-configured .NET devchains for fast response (PoA)
  \*\* [Blazor/Blockchain Explorer](https://github.com/Nethereum/NethereumBlazor) - Wasm blockchain explorer (functional sample)
- [Local Raiden](https://github.com/ConsenSys/Local-Raiden) - Run a local Raiden network in docker containers for demo and testing purposes
- [Local Ethereum Network](https://github.com/ConsenSys/local_ethereum_network) - Out-of-the-box deployment scripts for private PoW networks
- [Kaleido](https://kaleido.io/) - Use Kaleido for spinning up a consortium blockchain network. Great for PoCs and testing
- [aragonCLI](https://github.com/aragon/aragon-cli) - aragonCLI is used to create and develop Aragon apps and organizations.
- [ColonyJS](https://github.com/JoinColony/colonyJS) - JavaScript client that provides an API for interacting with the Colony Network smart contracts.
- [ArcJS](https://github.com/daostack/arc.js) - Library that facilitates javascript application access to the DAOstack Arc ethereum smart contracts.
- [Onboard.js](https://blocknative.com/onboard) - Blocknative Onboard is the quick and easy way to add multi-wallet support to your project. With built-in modules for more than 20 unique hardware and software wallets, Onboard saves you time and headaches.
- [web3-react](https://github.com/NoahZinsmeister/web3-react) - React framework for building single-page Ethereum dApps

### Ethereum ABI (Application Binary Interface) tools

- [Online ABI encoder](https://github.com/HashEx/abiencoder) - Free ABI encoder online service that allows you to encode your Solidity contract’s functions and constructor arguments.
- [ABI decoder](https://github.com/ConsenSys/abi-decoder) - library for decoding data params and events from Ethereum transactions
- [Ethereum ABI UI](https://github.com/hiddentao/ethereum-abi-ui) - Auto-generate UI form field definitions and associated validators from an Ethereum contract ABI
- [headlong](https://github.com/esaulpaugh/headlong/) - type-safe Contract ABI and Recursive Length Prefix library in Java
- [One Click dApp](https://oneclickdapp.com) - Instantly create a dApp at a unique URL using the ABI.
- [Nethereum-CodeGenerator](https://github.com/StefH/Nethereum-CodeGenerator) - A web based generator which creates a Nethereum based C# Interface and Service based on Solidity Smart Contracts.
- [EVMConnector](https://evmconnector.dev) - Create shareable contract dashboards and interact with arbitrary EVM-based blockchain functions, with or without an ABI.

### Patterns & Best Practices

#### Patterns for Smart Contract Development

- [Dappsys: Safe, simple, and flexible Ethereum contract building blocks](https://github.com/dapphub/dappsys)
  - has solutions for common problems in Ethereum/Solidity, eg.
    - [Whitelisting](https://steemit.com/ethereum/@nexusdev/dapp-a-day-11-whitelist-boring)
    - [Upgradable ERC20-Token](https://steemit.com/ethereum/@nikolai/dapp-a-day-6-upgradeable-tokens)
    - [ERC20-Token-Vault](https://steemit.com/ethereum/@nexusdev/dapp-a-day-18-erc20-token-vault)
    - [Authentication (RBAC)](https://steemit.com/ethereum/@nikolai/dapp-a-day-4-access-control-via-auth)
    - [...several more...](https://github.com/dapphub/dappsys)
  - provides building blocks for the [MakerDAO](https://github.com/makerdao/maker-otc) or [The TAO](https://github.com/ryepdx/the-tao)
  - should be consulted before creating own, untested, solutions
  - usage is described in [Dapp-a-day 1-10](https://steemit.com/@nikolai) and [Dapp-a-day 11-25](https://steemit.com/@nexusdev)
- [OpenZeppelin Contracts: An open framework of reusable and secure smart contracts in the Solidity language.](https://github.com/OpenZeppelin/openzeppelin-contracts)
  - Likely the most widely-used libraries and smart contracts
  - [Blog about Best Practices with Security Audits](https://blog.openzeppelin.com/)
- [CryptoFin Solidity Auditing Checklist](https://github.com/cryptofinlabs/audit-checklist) - A checklist of common findings, and issues to watch out for when auditing a contract for a Mainnet launch.
- [aragonOS: A smart contract framework for building DAOs, Dapps and protocols](https://docs.aragon.org/)
  - Upgradeability: Smart contracts can be upgraded to a newer version
  - Permission control: By using the `auth` and `authP` modifiers, you can protect functionality so only other apps or entities can access it
  - Forwarders: aragonOS apps can send their intent to perform an action to other apps, so that intent is forwarded if a set of requirements are met
- [EIP-2535 Diamond Standard](https://eips.ethereum.org/EIPS/eip-2535)
  - Organize contracts so they share the same contract storage and Ethereum address.
  - Solves the 24KB max contract size limit.
  - Upgrade diamonds by adding/replacing/removing any number of functions in a single transaction.
  - Upgrades are transparent by recording them with a standard event.
  - Get information about a diamond with events and/or four standard functions.

#### Upgradeability

- [Blog von Elena Dimitrova, Dev at colony.io](https://blog.colony.io/author/elena/)
  - https://blog.colony.io/writing-more-robust-smart-contracts-99ad0a11e948
  - https://blog.colony.io/writing-upgradeable-contracts-in-solidity-6743f0eecc88
- [Aragon developer blog](https://blog.aragon.org/development-updates/)
  - [Library driven development](https://blog.aragon.org/library-driven-development-in-solidity-2bebcaf88736)
  - [Advanced Solidity code deployment techniques](https://blog.aragon.org/advanced-solidity-code-deployment-techniques-dc032665f434/)
- [OpenZeppelin on Proxy Libraries](https://blog.openzeppelin.com/proxy-libraries-in-solidity-79fbe4b970fd/)

## Infrastructure

### Ethereum Clients

- [Besu](https://besu.hyperledger.org/en/latest/) - an open-source Ethereum client developed under the Apache 2.0 license and written in Java. The project is hosted by Hyperledger.
- [Geth](https://geth.ethereum.org/docs/) - Go client
- [Nethermind](https://github.com/NethermindEth/nethermind) - .NET Core client
- [Infura](https://infura.io/) - A managed service providing Ethereum client standards-compliant APIs
- [Ethereumjs](https://github.com/ethereumjs/ethereumjs-monorepo/tree/master/packages/client) - JS client using [ethereumjs-vm](https://github.com/ethereumjs/ethereumjs-vm)
- [Seth](https://github.com/dapphub/dapptools/tree/master/src/seth) - Seth is an Ethereum client tool—like a "MetaMask for the command line"
- [Mustekala](https://github.com/musteka-la/mustekala) - Ethereum Light Client project of Metamask
- [Exthereum](https://github.com/exthereum/blockchain) - Elixir client
- [EWF Parity](https://github.com/energywebfoundation/energyweb-ui) - Energy Web Foundation client for the Tobalaba test network
- [Quorum](https://github.com/jpmorganchase/quorum) - A permissioned implementation of Ethereum supporting data privacy by [JP Morgan](https://jpmorgan.com/quorum)
- [Mana](https://github.com/mana-ethereum/mana) - Ethereum full node implementation written in Elixir.
- [Chainstack](https://chainstack.com/) - A managed service providing shared and dedicated Geth nodes
- [QuickNode](https://quicknode.com/) - Blockchain developer cloud with API access and node-as-a-service.
- [Watchdata](https://watchdata.io) - Provide simple and reliable API access to Ethereum blockchain

### Storage

- [IPFS](https://ipfs.io/) - Decentralised storage and file referencing
  - [Mahuta](https://github.com/ConsenSys/Mahuta) - IPFS Storage service with added search capability, formerly IPFS-Store
  - [OrbitDB](https://github.com/orbitdb/orbit-db) - Decentralised database on top of IPFS
  - [PINATA](https://pinata.cloud) - The Easiest Way to Use IPFS
- [Infura](https://infura.io/) - A managed IPFS API Gateway and pinning service
- [Ceramic Storage](https://developers.ceramic.network/docs/composedb/guides/composedb-server/data-storage) - An api for user controlled, distrubuted storage. Built on top of IPFS and Orbitdb.
- [Aleph.im](https://aleph.im/) - an offchain incentivized peer-to-peer cloud project (database, file storage, computing and DID) compatible with Ethereum and IPFS.

### Messaging

- [DEVp2p Wire Protocol](https://github.com/ethereum/devp2p/blob/master/rlpx.md) - Peer-to-peer communications between nodes running Ethereum/Whisper
- [Pydevp2p](https://github.com/ethereum/pydevp2p) - Python implementation of the RLPx network layer
- [3Box Threads](https://docs.3box.io/api/messaging) - API to allow developers to implement IPFS persisted, or in memory peer to peer messaging.

## Testing Tools

- [Solidity coverage](https://github.com/sc-forks/solidity-coverage) - Alternative code coverage for Solidity smart-contracts
- [Solidity function profiler](https://github.com/EricR/sol-function-profiler) - Solidity contract function profiler
- [Sol-profiler](https://github.com/Aniket-Engg/sol-profiler) - Alternative and updated Solidity smart contract profiler
- [Espresso](https://github.com/hillstreetlabs/espresso) - Speedy, parallelised, hot-reloading solidity test framework
- [Eth tester](https://github.com/ethereum/eth-tester) - Tool suite for testing Ethereum applications
- [Cliquebait](https://github.com/f-o-a-m/cliquebait) - Simplifies integration and accepting testing of smart contract applications with docker instances that closely resembles a real blockchain network
- [Hevm](https://github.com/dapphub/dapptools/tree/master/src/hevm) - The hevm project is an implementation of the Ethereum virtual machine (EVM) made specifically for unit testing and debugging smart contracts
- [Ethereum graph debugger](https://github.com/fergarrui/ethereum-graph-debugger) - Solidity graphical debugger
- [Tenderly CLI](https://github.com/Tenderly/tenderly-cli) - Speed up your development with human readable stack traces
- [Solhint](https://github.com/protofire/solhint) - Solidity linter that provides security, style guide and best practice rules for smart contract validation
- [Ethlint](https://github.com/duaraghav8/Ethlint) - Linter to identify and fix style & security issues in Solidity, formerly Solium
- [Decode](https://github.com/hacker-DOM/decode) - npm package which parses tx's submitted to a local testrpc node to make them more readable and easier to understand
- [Psol](https://github.com/Lamarkaz/psol) - Solidity lexical preprocessor with mustache.js-style syntax, macros, conditional compilation and automatic remote dependency inclusion.
- [Decode and Publish](https://flightwallet.github.io/decode-eth-tx/) – Decode and publish raw ethereum tx. Similar to https://live.blockcypher.com/btc-testnet/decodetx/
- [Waffle](https://github.com/TrueFiEng/Waffle/tree/master/waffle-mock-contract) - a library for mocking smart contract dependencies during unit testing.
- [rocketh](https://github.com/wighawag/rocketh) - A simple lib to test ethereum smart contract that allow to use whatever web3 lib and test runner you choose.

## Security Tools

- [Mythril](https://github.com/ConsenSys/mythril) - Open-source EVM bytecode security analysis tool
- [Evmdis](https://github.com/Arachnid/evmdis) - Alternative EVM disassembler
- [Hydra](https://github.com/IC3Hydra/Hydra) - Framework for cryptoeconomic contract security, decentralised security bounties
- [Solgraph](https://github.com/raineorshine/solgraph) - Visualise Solidity control flow for smart contract security analysis
- [Manticore](https://github.com/trailofbits/manticore) - Symbolic execution tool on Smart Contracts and Binaries
- [Slither](https://github.com/crytic/slither) - A Solidity static analysis framework
- [Adelaide](https://github.com/sec-bit/adelaide) - The SECBIT static analysis extension to Solidity compiler
- [solc-verify](https://github.com/SRI-CSL/solidity/) - A modular verifier for Solidity smart contracts
- [Solidity security blog](https://github.com/sigp/solidity-security-blog) - Comprehensive list of known attack vectors and common anti-patterns
- [Awesome Buggy ERC20 Tokens](https://github.com/sec-bit/awesome-buggy-erc20-tokens) - A Collection of Vulnerabilities in ERC20 Smart Contracts With Tokens Affected
- [Free Smart Contract Security Audit](https://callisto.network/smart-contract-audit/) - Free smart contract security audits from Callisto Network

## Monitoring

- [Alethio](https://aleth.io/) - An advanced Ethereum analytics platform that provides live monitoring, insights and anomaly detection, token metrics, smart contract audits, graph visualization and blockchain search. Real-time market information and trading activities across Ethereum's decentralized exchanges can also be explored.
- [amberdata.io](https://amberdata.io) - Provides live monitoring, insights and anomaly detection, token metrics, smart contract audits, graph visualization and blockchain search.
- [Neufund - Smart Contract Watch](https://github.com/Neufund/smart-contract-watch) - A tool to monitor a number of smart contracts and transactions
- [Tenderly](https://tenderly.co/) - A platform that gives users reliable smart contract monitoring and alerting in the form of a web dashboard without requiring users to host or maintain infrastructure
- [BlockScout](https://github.com/poanetwork/blockscout) - A tool for inspecting and analyzing EVM based blockchains. The only full featured blockchain explorer for Ethereum networks.
- [Terminal](https://terminal.co/) - A control panel for monitoring dapps. Terminal can be used to monitor your users, dapp, blockchain infrastructure, transactions and more.
- [Ethereum-watcher](https://github.com/HydroProtocol/ethereum-watcher) - An extensible framework written in Golang for listening to on-chain events and doing something in response.
- [Alchemy Notify](https://docs.alchemyapi.io/guides/alchemy-notify) - Notifications for mined and dropped transactions, gas price changes, and address activity for desired addresses.
- [Blocknatve Mempool Explorer](https://www.blocknative.com/explorer) — Monitor any contract or wallet address and get streaming mempool events for every lifecycle stage — including drops, confirms, speedups, cancels, and more. Automatically decode confirmed internal transactions. And filter exactly how you want. Recieve events in our visual, no-code, interface or associate them with your API key to get events via a webhook. Mempool Explorer helps exchanges, protocols, wallets, and traders monitor and act on transactions in real-time.
- [Ethernal](https://www.tryethernal.com) - Ethereum block explorer for private chain. Browse transactions, decode function calls, event data or contract variables values on your locally running chain.

## Other Miscellaneous Tools

- [Solc](https://docs.soliditylang.org/en/latest/using-the-compiler.html) - Solidity compiler
- [Solidity cli](https://github.com/pubkey/solidity-cli) - Compile solidity-code faster, easier and more reliable
- [Solidity flattener](https://github.com/poanetwork/solidity-flattener) - Combine solidity project to flat file utility. Useful for visualizing imported contracts or for verifying your contract on Etherscan
- [Sol-merger](https://github.com/RyuuGan/sol-merger) - Alternative, merges all imports into single file for solidity contracts
- [eth-cli](https://github.com/protofire/eth-cli) - A collection of CLI tools to help with ethereum learning and development
- [Ethereal](https://github.com/wealdtech/ethereal) - Ethereal is a command line tool for managing common tasks in Ethereum
- [Eth crypto](https://github.com/pubkey/eth-crypto) - Cryptographic javascript-functions for Ethereum and tutorials to use them with web3js and solidity
- [Parity Signer](https://github.com/paritytech/parity-signer) - mobile app allows signing transactions
- [Decode](https://github.com/hacker-DOM/decode) - npm package which parses tx's submitted to a local testrpc node to make them more readable and easier to understand
- [TypeChain](https://github.com/ethereum-ts/TypeChain) - Typescript bindings for Ethereum smartcontracts
- [PHP based Blockchain indexer](https://github.com/digitaldonkey/ethereum-php-eventlistener) - allows indexing blocks or listening to Events in PHP
- [Node-Metamask](https://github.com/JoinColony/node-metamask) - Connect to MetaMask from node.js
- [Solidity-docgen](https://github.com/OpenZeppelin/solidity-docgen) - Documentation generator for Solidity projects
- [Ethereum ETL](https://github.com/blockchain-etl/ethereum-etl) - Export Ethereum blockchain data to CSV or JSON files
- [prettier-plugin-solidity](https://github.com/prettier-solidity/prettier-plugin-solidity) - Prettier plugin for formatting Solidity code
- [Unity3dSimpleSample](https://github.com/Nethereum/Unity3dSimpleSample) - Ethereum and Unity integration demo
- [Flappy](https://github.com/Nethereum/Nethereum.Flappy) - Ethereum and Unity integration demo/sample
- [Wonka](https://github.com/Nethereum/Wonka) - Nethereum business rules engine demo/sample
- [Resolver-Engine](https://github.com/Crypto-Punkers/resolver-engine) - A set of tools to standarize Solidity import and artifact resolution in frameworks.
- [eth-reveal](https://github.com/justinjmoses/eth-reveal) - A node and browser tool to inspect transactions - decoding where possible the method, event logs and any revert reasons using ABIs found online.
- [Ethereum-tx-sender](https://github.com/HydroProtocol/ethereum-tx-sender) - A useful library written in Golang to reliably send a transaction — abstracting away some of the tricky low level details such as gas optimization, nonce calculations, synchronization, and retries.
- [Blocknative Gas Platform](https://www.blocknative.com/gas) — Gas estimation for builders, by builders. Gas Platform harnesses Blocknative's real-time mempool data infrastructure to accurately and consistently estimate Ethereum transaction fees. This provides builders and traders with an up-to-the-moment gas fee API.
- [ETH Gas.watch](https://ethgas.watch/) - A gas price watcher with email notifications on price change

## Smart Contract Standards & Libraries

### [ERCs](https://eips.ethereum.org/erc) - The Ethereum Request for Comment repository

- Tokens
  - [ERC-20](https://eips.ethereum.org/EIPS/eip-20) - Original token contract for fungible assets
  - [ERC-721](https://eips.ethereum.org/EIPS/eip-721) - Token standard for non-fungible assets
  - [ERC-777](https://eips.ethereum.org/EIPS/eip-777) - An improved token standard for fungible assets
  - [ERC-918](https://eips.ethereum.org/EIPS/eip-918) - Mineable Token Standard
- [ERC-165](https://eips.ethereum.org/EIPS/eip-165) - Creates a standard method to publish and detect what interfaces a smart contract implements.
- [ERC-725](https://eips.ethereum.org/EIPS/eip-725) - Proxy contract for key management and execution, to establish a Blockchain identity.
- [ERC-173](https://eips.ethereum.org/EIPS/eip-173) - A standard interface for ownership of contracts

### Popular Smart Contract Libraries

- [Zeppelin](https://github.com/OpenZeppelin/openzeppelin-contracts) - Contains tested reusable smart contracts like SafeMath and OpenZeppelin SDK [library](https://github.com/OpenZeppelin/openzeppelin-sdk) for smart contract upgradeability
- [cryptofin-solidity](https://github.com/cryptofinlabs/cryptofin-solidity) - A collection of Solidity libraries for building secure and gas-efficient smart contracts on Ethereum.
- [Modular Libraries](https://github.com/Modular-Network/ethereum-libraries) - A group of packages built for use on blockchains utilising the Ethereum Virtual Machine
- [DateTime Library](https://github.com/bokkypoobah/BokkyPooBahsDateTimeLibrary) - A gas-efficient Solidity date and time library
- [Aragon](https://github.com/aragon/aragon) - DAO protocol. Contains [aragonOS smart contract framework](https://github.com/aragon/aragonOS) with focus on upgradeability and governance
- [ARC](https://github.com/daostack/arc) - an operating system for DAOs and the base layer of the DAO stack.
- [0x](https://github.com/0xProject) - DEX protocol
- [Token Libraries with Proofs](https://github.com/sec-bit/tokenlibs-with-proofs) - Contains correctness proofs of token contracts wrt. given specifications and high-level properties
- [Provable API](https://github.com/provable-things/ethereum-api) - Provides contracts for using the Provable service, allowing for off-chain actions, data-fetching, and computation
- [ABDK Libraries for Solidity](https://github.com/abdk-consulting/abdk-libraries-solidity) - Fixed-point (64.64 bit) and IEEE-754 compliant quad precision (128 bit) floating-point math libraries for Solidity

## Developer Guides for 2nd Layer Infrastructure

### Scalability

### Payment/State Channels

- [Ethereum Payment Channel](https://medium.com/@matthewdif/ethereum-payment-channel-in-50-lines-of-code-a94fad2704bc) - Ethereum Payment Channel in 50 lines of code
- [µRaiden Documentation](https://microraiden.readthedocs.io) - Guides and Samples for µRaiden Sender/Receiver Use Cases

### Plasma

- [Learn Plasma](https://github.com/ethsociety/learn-plasma) - Website as Node application that was started at the 2018 IC3-Ethereum Crypto Boot Camp at Cornell University, covering all Plasma variants (MVP/Cash/Debit)
- [Plasma MVP](https://github.com/omisego/plasma-contracts) - OmiseGO's research implementation of Minimal Viable Plasma
- [Plasma MVP Golang](https://github.com/kyokan/plasma) - Golang implementation and extension of the Minimum Viable Plasma specification
- [Plasma Guard](https://github.com/mesg-foundation/plasma-guard) - Automatically watch and challenge or exit from Omisego Plasma Network when needed.

### Side-Chains

- [POA Bridge UI](https://github.com/omni/bridge-ui)
- [POA Bridge Contracts](https://github.com/omni/tokenbridge-contracts)
- [Loom Network](https://github.com/loomnetwork)

### Privacy / Confidentiality

#### ZK-SNARKs

- [ZoKrates](https://github.com/Zokrates/ZoKrates) - A toolbox for zkSNARKS on Ethereum
- [Nightfall](https://github.com/EYBlockchain/nightfall_3) - Make any ERC-20 / ERC-721 token private - open source tools & microservices
- Proxy Re-encryption (PRE)
  **[NuCypher Network](https://github.com/nucypher/nucypher) - A proxy re-encryption network to empower data privacy in decentralized systems
  ** [pyUmbral](https://github.com/nucypher/pyumbral) - Threshold proxy re-encryption cryptographic library

### Scalability + Privacy

### ZK-STARKs

- [StarkWare](https://github.com/starkware-industries) and [StarkWare Resources](https://github.com/starkware-libs) - StarkEx scalability engine storing state transitions on-chain

### Prebuilt UI Components

- [ui.decentraland.org](https://github.com/decentraland/ui) - A React library including Dapp components
- [dapparatus](https://github.com/austintgriffith/dapparatus) - Reusable React Dapp components
- [Metamask ui](https://github.com/MetaMask/metamask-extension/tree/main/ui/components) - Metamask React Components
- [DappHybrid](https://github.com/Nethereum/Nethereum.DappHybrid) - A cross-platform hybrid hosting mechanism for web-based decentralized applications
- [Nethereum.UI.Desktop](https://github.com/Nethereum/Nethereum.UI.Desktop) - Cross-platform desktop wallet sample
- [eth-button](https://eth-button.github.io/eth-button/) - Minimalist donation button
- [3Box Plugins](https://docs.3box.io/build/plugins) - Drop in react components for social functionality. Including comments, profiles, and messaging.

:::info

Inspired by: https://github.com/ConsenSys/ethereum-developer-tools-list

:::
