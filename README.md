Project description
Introduction
The food supply chain is a complex but necessary food production arrangement needed by the global community to maintain sustainability and food security. The supply chain has been extended geographically involving many more stakeholders, making the supply chain longer and complicated and thus involving many challenges.

Some of the challenges that are commonly faced in food supply chains are

Lack of traceability and communication.
Rising supply chain costs.
Supply of fraudulent food products.
Failure in monitoring warehouses.
Objectives
The project aims to design a decentralized food supply chain to trace products from end to end and provide a smart and reliable way of providing information to the customers.
Features

Platform to trace food products worldwide.
Restricting duplicate and unauthentic products.
Proper food distribution.
Reducing the supply chain costs.
System Architecture
The application follows the layered architecture where components which similar functionality are organized into horizontal layers and each layer has a specific role within the application.
The system architecture consists of three layers:

Application Layer
Blockchain Layer
Infrastructure Layer


Methodology
The project is build on three core modules: Traceability System, Trading Mechanism and Reputation System.

Traceability System

Each product is marked with unique serial code which is onwed by an externally owned account on Ethereum.
Every product transaction is recorded and stored in smart contract and linked with product's serial code.
This comes with Access Control Strategy which allows only authentic users to make specific transactions.
Trading Mechanism



The process of delivering goods from one entity to another is tracked and recorded on the blockchain.
The consumers first register themselves on the system and request to purchase the product with a serial number.
The purchase request is sent to the product owner who updates the product ownership with the new owner.
This process ensures that retailers do not sell products with duplicate serial codes.
Reputation System



This system adds a layer of trust between customers and retailers.
This mechanism allows only actual customers of the product to post feedback about the product.
The reviews on the blockchain are immutable which does not allow any merchant or retailer to delete or update bad reviews to increase their overall ratings.
And in this way this mechanism maintains the complete integrity of the retailer and let the customer know about the seller before making the transaction.
Development Setup
Requirements
NodeJS >= 10.16 and npm >= 5.6 installed.
Git installed in the system.
Truffle, which can be installed globally with npm install -g truffle
Metamask extension added to the browser.
Ganache development network.
Clone the repository

git clone https://github.com/lakshya-20/supply-chain
Setting Up Truffle Project
Smart contracts or blockchain codes are necessary config files for developing, testing and deploying application business logic are present inside src/Smart-Contract directory.

Checkout smart contracts directory

cd src/Smart-Contract
Install Truffle

npm install -g truffle
Compile Smart Contracts

truffle compile
Deploy Smart Contract on Ganache's development Network

truffle migrate --reset
Run Test Coverage

truffle test
Setting up Client Application
Create .env file to setup environment variables

REACT_APP_NFT_STORAGE_APIKEY=<https://nft.storage APIKEY>
Install Dependencies

npm install
Start Client

npm start
