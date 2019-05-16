## Blockchain Developer

![](https://media.giphy.com/media/5Ko2Tcv5MGMuI/giphy.gif)

[![Build Status](https://semaphoreci.com/api/v1/ibrunotome/udacity-blockchain-developer-nanodegree/branches/master/badge.svg)](https://semaphoreci.com/ibrunotome/udacity-blockchain-developer-nanodegree)

### Projects

#### 1 - [Manage Your Blockchain Identity](https://github.com/2series/Blockchain/tree/master/project%201%20-%20Manage%20Your%20Blockchain%20Identity)

Learn to create your identity on the Blockchain and interact with an existing web service.

#### 2 - [Building your own Private Blockchain](https://github.com/2series/Blockchain/tree/master/project%202%20-%20Building%20your%20own%20Private%20Blockchain)

Building your own Private Blockchain utilizing Node.js with LevelDB.

#### 3 - [RESTful Web API with Node.js Framework](https://github.com/2series/Blockchain/tree/master/project%203%20-%20RESTful%20Web%20API%20with%20Node.js%20Framework)

Create a web API using a Node.js framework that will interact with your private blockchain to submit and retrieve blockchain data.

#### 4 - [Build A Private Blockchain Notary Service](https://github.com/2series/Blockchain/tree/master/project%204%20-%20Build%20A%20Private%20Blockchain%20Notary%20Service)

Utilizing your existing web API, you will create a star registry notarization service.

#### 5 - [Descentralized Star Notary Project](https://github.com/2series/Blockchain/tree/master/project%205%20-%20Descentralized%20Star%20Notary%20Project)

Build additional functionality with your smart contract and deploy it on the public testnet to create a DApp.

## Notes 

### Jargon 
* Ledger: A system of record for a business
* Transaction: An asset transfer onto or off the ledger
* Contract: Terms & Conditions for a transaction to occur
* Blockchain: A trusted distributed ledger with shared business processes

### Bitcoin
* An unregulated shadow currency
* Having property of anonymity
	* We don’t know who we are sending a bitcoin to
	* We don’t know whom we are receiving a bitcoin from
* Extremely computational resource intensive to make the bitcoin network work

### Using blockchain for business is different from using it in bitcoin
* We prioritize identity over anonymity
* We prioritize selective endorsement over proof of work (we get to choose who in the network will validate a particular transaction - it’s more computationally efficient than bitcoin
* We prioritize assets over cryptocurrencies

### Requirements for blockchain for business
* Shared ledger: Append-only distributed system of record shared across business networks
* Privacy: Ensuring appropriate visibility; transactions are secure, authenticated and verifiable
* Smart Contracts: Business terms embedded in transaction database & executed with transactions
* Trust: Transaction are endorsed by relevant participants, Independent Audits

## More depth

### Shared ledger
* Shared between participants
* Participants have their own copy through replication
* Permission: The participants only see appropriate transactions
* A shared system of record

### Smart contract
* A way of encoding & sharing the shared business process in blockchain
* You take the english contract & encode it into Solidity, a programming language
* Are verified
* Are signed

### Privacy 
* Transactions need to be authenticated
* Participants need an identity not linked to the transaction
* Participants need appropriate confidentiality between subsets of participants
* Making sure that blockchain is tamper-proof

### Trust
* Selected members from business network endorse the transactions
* When transactions are endorsed they are added to the blockchain
* This gives us the concept of Verifiable Audit Trail
	* Transactions cannot be modified, inserted or deleted
* The concept of trust is achieved via:
	* Consensus
	* Provenance
	* Immutability
	* Finality

## Blockchain for business has several advantages

* Saves time: Transaction processing time becomes instantaneous
* Reduces cost: Removes overheads & costly intermediaries
* Reduces risk: Tampering, fraud and cyber crime
* Increases trust: Through shared processes & record keeping

For example, a business network that runs on a blockchain can speed up transaction processes and audits. That in turn reduces costs and can lead to greater customer satisfaction. A business that runs a supply chain network can benefit from blockchain by reducing errors in shipments, have better tracking of materials and, reduce the risk of illicit tampering of records.

## Some notiable industry use cases for blockchain implementation

### Finance 
* Trade finance
* Foreign currency payments
* Mortgages

### Public sector
* Asset registration
* Citizen identification
* Medical records
* Medicine Supply Chain

### Retail
* SCM
* Customer Loyalty Programs
* Information Sharing (supplier - retailer)

### Insurance
* Claims processing
* Risk Provenance
* Asset usage history
* Claims file

### Manufacturing
* SCM
* Product part identification
* Maintenance tracking records

## There are 4 test words to discover whether or not an industry is a good blockchain use case
* Consensus
* Provenance
* Immutability
* Finality
These four are key elements to achieve trust in blockchain

## Patterns for customer adoption
Key to success: don’t try to boil the ocean, and don’t go for the big high powered, high impact use case first. Look for something small and a room for improvement. 

A hierarchy of different usages in listed below. As you move downward. It’s much easier to start with something on the compliance ledger and work your way up the stack than really trying to start higher.

### Compliance Ledger (easiest to implement)
* Real-time view of compliance, audit & risk data
* Provenance, immutability & finality are key
* Transparent access to auditor & regulator

### Consortium Shared Ledger
* Created by a small set of participants
* Share key reference data
* Consolidated, consistent real-time view

### Asset Exchange
* Sharing of assets (voting, dividend notifications)
* Assets are information, not financial
* Provenance & finality are key

### High Value Market (hardest to implement)
* Transfer of high value of financial assets
* Between many participants in a market
* Regulatory timeframes

So customers need to go through an awareness journey to understand what smart contracts can do for their business, and how can they improve the operations in their network using blockchain. 

## Key players for blockchain adoption

### Regulator
* An organization who enforces the rule of play
* E.g. bank

### Industry Groups
* Often funded by members of a business network
* Provide technical advice on industry trends
* Encourages best practice by making recommendations to members

### Market Maker
* The organization who innovates
	* Creates a new product or service, and business process 
	* Creates a new business process for an existing product or service

We can start with any of the aforementioned players or even with a combination of them

## Insights
Linux Foundation Hyperledger Project, which is an open source, collaborative effort that seeks to advance blockchain technologies. IBM also offers the IBM Blockchain Platform that can help you build and operate a complete business network. The Platform also provides tools to help you align the needs of developers and business leaders in your organization.

Transferring assets is the heart of blockchain. 

How can people buy and sell or transfer goods in a business network without any central governing body or policy?  (Look at web demo) [Hyperledger Composer](http://composer-playground.mybluemix.net/)

### Hyperledger Composer
* A suite of high level application abstractions for business networks
* Being model at the level of assets, participants and
* It enables a quick solution

### Features
* Model your business network, test and deploy
* Applications use APIs to interact with a business network
* Integrate existing systems of record using loopback/REST

### Benefits
* Increases understanding: from business concepts to blockchain
* Saves time: develop blockchain applications more quickly and cheaply
* Reduces risk: well tested, efficient design conforms to best practice
* Increases flexibility: higher level abstraction makes it easier to iterate

Hyperledger Fabric is like the operating system. Hyperledger Composer is like the API.

### Conceptual Components and Structure
Business network is defined by *Models*, *Script Files*, *ACLs* and *Metadata* and packaged in a *Business Network Archive*.

### Logic of business network is held in Script files
When a transaction is submitted, the blockchain run time is going to find the script functions that are interested in that transaction and then run them. Those script functions can have side effects on assets that are being managed in asset registries.

## Components in a Blockchain
* Ledger: A ledger is a channel’s chain and current state data which is maintained by each peer on the channel

* Smart Contract: Software running on a ledger, to encode assets and the transactions instructions for modifying the assets

* Peer network: A broader term overarching the entire transactional flow, which serves to generate an agreement on the order and to confirm the correctness of the set of transactions constituting a block

* Membership: Membership services authenticates, authorizes and manages identities on a permissioned blockchain network

* Events: Creates notifications of significant operations on the blockchain (e.g. a new block), as well as notifications related to smart contracts

* Systems management: Provides the ability to create, change & monitor blockchain components

* Wallet: Securely manages a user’s security credentials (Private Key)

* Systems Integration: Responsible for integrating blockchain bi-directionally with external systems. Not part of the blockchain

### Blockchain developer
Developers care about application and smart contracts
They don’t care about peers, consensus & security

### Ledger’s data structure
A ledger often consists of two data structures: blockchain and world state
Blockchain is:
* A linked list of blocks
* Each block describes a set of transactions
* Immutable - blocks cannot be tampered with or altered

And also we have world’s state:
What it does is to record the current state of all your assets

World State is:
* An ordinary database (e.g. key/value store)
* Stores the combined outputs of all transactions
* Not usually immutable

## Consideration for the blockchain operator
Operators’ interests are in the deployment & operation part of the blockchain:
* Peers
* Consensus
* Security

They don’t care about development concerns, such as:
* Application Code
* Smart Contract Code
* Events and Integration

Examples: 
* They make sure that peers are up to date
* Making them work together in the way that they should
* Ensuring that consensus is happening in the way that it should be taking place
* What security methods do we need? 

## How do we reach consensus
Consensus is the process of maintaining a consistent ledger

Consensus helps us to:
* Keep all peers up-to-date
* Fix any peers in error
* Quarantine all malicious nodes

Some examples of consensus algorithms:
* Proof of work
* Proof of stake
* Solo
* Kafka/Zookeeper
* Proof of elapsed time
* PBFT-based (Hyperledger fabric uses this)

## Public vs. Private blockchains
Public: 
	* For example Bitcoin
	* Transactions are viewable by everyone
	* Participant identity is almost impossible to infer
Private: 
	* For example Hyperledger Fabric
	* Network members are known, but transactions are secret

## Architect consideration
Architect should care about the following:
* Performance
	* Amount of data being shared
	* Number and location of peers
	* Latency and throughput
	* Batching characteristics
* Security 
	* Type of data being shared and with whom
	* How is identity achieved
	* Confidentiality of transaction queries
	* Who verifies transactions
Resiliency
	* Resource failure
	* Malicious activity
	* No-determinism
  
