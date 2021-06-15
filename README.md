
# Udacity Blockchain Supply Chain

### UML Diagrams
  ![enter image description here](https://raw.githubusercontent.com/GoodKelvin/udacity-project-blockchain-supply-chain/main/images/Udacity_Blockchain_Supply_Chain_1.png)
  ![enter image description here](https://raw.githubusercontent.com/GoodKelvin/udacity-project-blockchain-supply-chain/main/images/Udacity_Blockchain_Supply_Chain_2__.png)
  ![enter image description here](https://raw.githubusercontent.com/GoodKelvin/udacity-project-blockchain-supply-chain/main/images/Udacity_Blockchain_Supply_Chain_3.png)
  
  
  ### Libraries
  Dependencies in my `packages.json` file are as follows:

     "dependencies": {
    	"truffle": "^5.1.51",
    	"truffle-assertions": "^0.9.2",
    	"truffle-hdwallet-provider": "^1.0.17",
    	"web3": "^1.3.0",
     "web3-provider-engine": "^14.1.0"
    }

**Why I used these libraries**:
-   `truffle`: truffle is a development framework for Ethereum that makes it easy to compile, test, and migrate solidity contracts to Ethereum networks. 
-   `truffle-assertions`: Contains convenient functions designed for solidity assertions inside of truffle tests.
-   `truffle-hdwallet-provider`: enables my truffle deployments on the Rinkeby network and spend test coins
-   `web3`: API for interacting with blockchain
-
### IPFS (InterPlanetary File System)
I did not use IPFS.

# Deployed to Rinkeby Network*

**Transaction Hash**: 0x47e07eb6b852236e17829de0006f5ff326ec80b98ff8b33d4e373f21d17bb55c

**Contract Address**: 0x4b3f185ebd94b5ff403fd2dd538bedfb9fd7b5d5

**Etherscan url**: https://rinkeby.etherscan.io/tx/0x47e07eb6b852236e17829de0006f5ff326ec80b98ff8b33d4e373f21d17bb55c

![enter image description here](https://raw.githubusercontent.com/GoodKelvin/udacity-project-blockchain-supply-chain/main/images/deploy.JPG)

# Instructions
### Prerequisites

Please make sure you've already installed ganache-cli, Truffle and enabled MetaMask extension in your browser.

```
Give examples (to be clarified)

```

### [](https://github.com/galen211/udacity-blockchain-developer/blob/master/project3/INSTRUCTIONS.md#installing)Installing

A step by step series of examples that tell you have to get a development env running

Clone this repository:

```
git clone https://github.com/GoodKelvin/udacity-project-blockchain-supply-chain

```

Change directory to  `app`  folder and install all requisite npm packages (as listed in  `package.json`):

```
cd app
npm install
```
Launch Ganache Desktop:

     Update the from value in ***truffle-config *rinkeby object***

In a separate terminal window, Compile smart contracts:

```
truffle compile
```
This will create the smart contract artifacts in folder `build\contracts`.
Migrate smart contracts to the locally running blockchain, ganache-cli:

```
truffle migrate
```
Test smart contracts:

```
truffle test

```
![enter image description here](https://raw.githubusercontent.com/GoodKelvin/udacity-project-blockchain-supply-chain/main/images/test.png)
All 11 tests should pass.

 In a separate terminal window, launch the DApp:

```
npm run dev
```

