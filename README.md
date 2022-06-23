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

[Activity](./activity.png)

[Sequence](./sequence.png)

[State](./state.png)

[class](./project-6.svg)


## Deploy 
node  v12.0.0
Truffle v4.1.14 (core: 4.1.14)
Solidity v0.4.24 (solc-js)
web3

[etherscan link](https://rinkeby.etherscan.io/address/0x7d84c5ab4443f4b20ba6d6ba3b84f88f3f75a385#code)
```
 Replacing FarmerRole...
  ... 0xbaf118631cc20fedbf80aae53499e94c1ebbc42363eb856a99eb53f1c6523f88
  FarmerRole: 0xf74fbd483c73d9c148ce58232677f98ed54c9649
  Replacing DistributorRole...
  ... 0x3eb91909521309b89e1540e9232b2222d8e2b8dde3f69acb9ae2a00cfce2df71
  DistributorRole: 0x8feb6acb053680a82b57c1991753927b6c8df0a3
  Replacing RetailerRole...
  ... 0x7d4cba32b97a1697e9efae28971e618597a6ebdc1c57b80f6e4ca485e42738a4
  RetailerRole: 0xa3c8b0ec92769f81a8406a294f88e28132a3ff38
  Replacing ConsumerRole...
  ... 0xd23b72ce9fe80f44acda8d6d9810448191befa00d1b73322293a4a99c41d3b9a
  ConsumerRole: 0x0c450b74935dfbeb80a07383c17c956930b0f465
  Replacing SupplyChain...
  ... 0x0c2f5e8abb1162a7d652ba29b1a96cb844d100db76499781fbfe22a92fdb3987
  SupplyChain: 0x9e17fdb56b92dce7e5d5655cc60ef220301ba94b
Saving successful migration to network...
  ... 0xacb181f60419e7121604eeb335d404ccb4cec70ac18db3a527f74ad624cd49b8
```
