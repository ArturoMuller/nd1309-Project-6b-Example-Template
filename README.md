# Supply chain & data auditing

This repository containts an Ethereum DApp that demonstrates a Supply Chain flow between a Seller and Buyer. The user story is similar to any commonly used supply chain process. A Seller can add items to the inventory system stored in the blockchain. A Buyer can purchase such items from the inventory system. Additionally a Seller can mark an item as Shipped, and similarly a Buyer can mark an item as Received.

The DApp User Interface when running should look like...

![truffle test](images/ftc_product_overview.png)

![truffle test](images/ftc_farm_details.png)

![truffle test](images/ftc_product_details.png)

![truffle test](images/ftc_transaction_history.png)


## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

Please make sure you've already installed ganache-cli, Truffle and enabled MetaMask extension in your browser.

```
Give examples (to be clarified)
```

### Installing

> The starter code is written for **Solidity v0.4.24**. At the time of writing, the current Truffle v5 comes with Solidity v0.5 that requires function *mutability* and *visibility* to be specified (please refer to Solidity [documentation](https://docs.soliditylang.org/en/v0.5.0/050-breaking-changes.html) for more details). To use this starter code, please run `npm i -g truffle@4.1.14` to install Truffle v4 with Solidity v0.4.24. 

A step by step series of examples that tell you have to get a development env running

Clone this repository:

```
git clone https://github.com/udacity/nd1309/tree/master/course-5/project-6
```

Change directory to ```project-6``` folder and install all requisite npm packages (as listed in ```package.json```):

```
cd project-6
npm install
```

Launch Ganache:

```
ganache-cli -m "spirit supply whale amount human item harsh scare congress discover talent hamster"
```

Your terminal should look something like this:

![truffle test](images/ganache-cli.png)

In a separate terminal window, Compile smart contracts:

```
truffle compile
```

Your terminal should look something like this:

![truffle test](images/truffle_compile.png)

This will create the smart contract artifacts in folder ```build\contracts```.

Migrate smart contracts to the locally running blockchain, ganache-cli:

```
truffle migrate
```

Your terminal should look something like this:

![truffle test](images/truffle_migrate.png)

Test smart contracts:

```
truffle test
```

All 10 tests should pass.

![truffle test](images/truffle_test.png)

In a separate terminal window, launch the DApp:

```
npm run dev
```

## Built With

* [Ethereum](https://www.ethereum.org/) - Ethereum is a decentralized platform that runs smart contracts
* [IPFS](https://ipfs.io/) - IPFS is the Distributed Web | A peer-to-peer hypermedia protocol
to make the web faster, safer, and more open.
* [Truffle Framework](http://truffleframework.com/) - Truffle is the most popular development framework for Ethereum with a mission to make your life a whole lot easier.


## Authors

See also the list of [contributors](https://github.com/your/project/contributors.md) who participated in this project.

## Acknowledgments

* Solidity
* Ganache-cli
* Truffle
* IPFS

Your project files

## UML documents:

[Activity](activity.png)

[Sequence](sequence.png)

[State](state.png)

[class](project-6.svg)


## Deploy 
node  v12.0.0
Truffle v4.1.14 (core: 4.1.14)
Solidity v0.4.24 (solc-js)
web3

[etherscan link](https://rinkeby.etherscan.io/address/0x7d84c5ab4443f4b20ba6d6ba3b84f88f3f75a385#code)
```
Deploying FarmerRole...
  ... 0x5dc345135a8da7df82721c71635ca9f1b7e09220334eba43b917d52823af9d11
  FarmerRole: 0x19abd1b1c1a98f6a02d85d4bf606b2e3e86bcd7c
  Deploying DistributorRole...
  ... 0x1ba8612a6b9d8c005e12ea180b86d306971235ca568ac50022dfde4ad67edd13
  DistributorRole: 0x07ffd501851f84d3c63b4c54b363fb082e22c693
  Deploying RetailerRole...
  ... 0x94616a30cd50b5f2a492a2287b494dcd6158eda840653ef1805fa10798657d6c
  RetailerRole: 0x65c676157f0e29f84bc4dfdc7ea801e83b830987
  Deploying ConsumerRole...
  ... 0xd21d67240c69d3ac373716cebf6366c0673a5e32bf5479ec7ed58f20b233e111
  ConsumerRole: 0xfa2fde8a8a48ae1e89c186ae9676224e038f4287
  Deploying SupplyChain...
  ... 0xaa5a95d3e228c15ce6336b6e405d10960e643ff53d2aed32fb2237cdfb108ddd
  SupplyChain: 0x7d84c5ab4443f4b20ba6d6ba3b84f88f3f75a385
Saving successful migration to network...
  ... 0x5a160d38e53ead00551c374c9b331ef6dcbeeab2114e4d0b14b7999737be088f
```
