
# Coffee chain

Main purpose for this application is to record where the coffee is from, and when it is roasted and by who, onto the blockchain

# Libraries used

Truffle v4.1.14 (core: 4.1.14)  
Solidity v0.4.24 (solc-js)  
Node v17.3.1  
Truffle Assertions v0.9.2  
Web3 v0.20.6  

# Contracts address on Rinkeby
  FarmerRole: 0x177f000d1661ee1e0153fd26c266d94c7c3d7293  
  DistributorRole: 0x2b6e1f5edb59cbe912bb6066607ab43ccf4a5f9a  
  RetailerRole: 0x5f67b23bc01689c789e2f70c3937782cce7ddd38  
  ConsumerRole: 0x0e6f60c0639aad2ae5d933f6cd1c2fcea42d39f0  
  SupplyChain: 0x383bf4ff8de5ea1f3747e47b62c5fe5fbc8927ad  

  https://rinkeby.etherscan.io/address/0x383bf4ff8de5ea1f3747e47b62c5fe5fbc8927ad

# UML Diagram

### Activity Diagram

![Activity Diagram](./uml/Activity.png)

### Sequence Diagram

![Sequence Diagram](./uml/Sequence.png)

### State Diagram

![State Diagram](./uml/State.png)

### Data Diagram

![Data Diagram](./uml/Data.png)

# IPFS

IPFS is not used

# Supply chain & data auditing

This repository containts an Ethereum DApp that demonstrates a Supply Chain flow between a Seller and Buyer. The user story is similar to any commonly used supply chain process. A Seller can add items to the inventory system stored in the blockchain. A Buyer can purchase such items from the inventory system. Additionally a Seller can mark an item as Shipped, and similarly a Buyer can mark an item as Received.

The DApp User Interface when running should look like...

![truffle test](images/ftc_product_overview.png)

![truffle test](images/ftc_farm_details.png)

![truffle test](images/ftc_product_details_1.png)

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
