# Mix SDK

## Introduction

The Mix SDK is a set of tools for creating, managing, and engaging with Mix Smart Wallets in client applications. Mix Smart Wallets are smart contract wallets associated with each user's Externally Owned Account (EOA) that provide added security compared to traditional EOAs with a single private key. With Mix Smart Wallets, users can deposit funds that no one else can control and withdraw at any time.

### Purpose of the SDK

The Mix Wallet SDK is designed to make it easy for developers to create, manage, and engage with Mix Smart Wallets in their Flutter and TypeScript applications. The SDK provides pre-built functions and utilities, allowing developers to interact with Mix Smart Wallets securely and efficiently.

### **Benefits of using Mix Smart Wallets**

Using Mix Smart Wallets provides several benefits, including:

* Enhanced security: Mix Smart Wallets are non-custodial accounts that allow users to deposit funds that no one else can control and withdraw at any time. Each Mix Smart Wallet is a smart contract associated with the user's EOA and can only be controlled by that user.
* Enhanced UX: Mix Smart Wallets support gasless transactions, improving the user experience and making it more seamless to interact with the blockchain.
* Better developer experience: The Mix Wallet SDK abstracts away the complexities of web3 development, such as cryptography, wallet management, and smart contract interactions, making it easier for developers to build blockchain-based applications.

### **Features**

The Mix Wallet SDK provides several features that allow developers to create, manage, and engage with Mix Smart Wallets in their applications. Some of the key features include:

* **Create a Mix Smart Wallet**: Create a new Mix Smart Wallet associated with a user's EOA.
* **Retrieve an existing Mix Smart Wallet**: Retrieve an existing Mix Smart Wallet associated with a user's EOA if it exists.
* **Send transactions**: Send transactions, including ERC20 and NFT transfers and interaction with arbitrary smart contracts, through the Mix relayer that will cover the gas fees. This allows users to interact with the blockchain without worrying about gas fees.
* **Retrieve transactions history**: Retrieve a user's transaction history for their Mix Smart Wallet. This makes it easy to keep track of their activity on the blockchain.
* **Retrieve ERC20 and ERC721 token balances**: Retrieve a user's ERC20 and ERC721 token balances for their Mix Smart Wallet. This makes it easy to monitor their holdings on the blockchain.
* **Staking**: Let Smart Wallet owners stake their native MIX tokens directly in the app and earn rewards.
* **Trading**: Let Smart Wallet owners swap various assets and get price data for several assets on the Mix network.

### **Language and Framework Requirements**

The Mix Wallet SDK is currently available for Flutter/Dart. A Typescript SDK is planned for release in the near future.

### **Limitations**

The Mix Wallet SDK works only on the Mix network, an EVM-compatible L1 blockchain. Support for other blockchains is planned for the future.

In the following sections, we will cover how to start with the Mix Wallet SDK, an overview of its architecture, and frequently asked questions. If you have any questions or feedback, please get in touch with our support team at [**support@**](mailto:support@chargesmartwallets.com)[**fuse.io**](http://fuse.io)**.**
