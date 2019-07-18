# flowchain-ledger
> Flowchain distributed ledgers in JavaScript

![](https://flowchain.co/static/logo-text@128.png)

[![Build Status](https://travis-ci.org/flowchain/flowchain-ledger.svg?branch=master)](https://travis-ci.org/flowchain/flowchain-ledger)

Flowchain-ledger is a distributed ledger technology (DLT) for the Internet of Things (IoT) devices (aka. IoT Blockchain). The Flowchain software framework is designed from the ground up to fit current IoT needs.

This is the **official** Flowchain distributed ledger library, which provides the following APIs:
* Create data transactions
* Submit data transactions

# About Flowchain

Flowchain is a software framework for the IoT blockchain to provide a distributed ledger programming framework for peer-to-peer IoT networks and real-time data transactions, and ```flowchain-ledger``` is the Node.js distribution for heterogeneous hardware devices, such as MediaTek LinkIt Smart 7688, Raspberry Pi, laptops, smart phones and etc.

# Abstract

Flowchain aims to implement a blockchain that can provide near real-time transactions for the IoT. The Flowchain technology can ensure chunked data (data streams) transactions by using the *virtual blocks* concept which is proposed by Flowchain acamedic papers. The virtual blocks can be combined with emerging public blockchains, such as Ethereum and Hyperledger which is optimized specifically for the use case of off-chain transactions. If you need such "Hybrid Blockchain" network for the IoT, please refer to [flowchain-hybrid](https://github.com/flowchain/flowchain-hybrid).


The FlowchainCoin (symbol: FLC) is the Ethereum ERC20 token for tokenized assets that use in the Flowchain network. Tokens offer can support the transfer of assets from one trusted party to another.

# Features

* Mining-based Proof-of-Stake (PoS)
* Run on every IoT node
* RPC over the Websocket protocol
* Distributed Hash Table (DHT) by the Chord protocol
* The device server in Web of Things (WoT) architecture

# Getting started

Use `flowchain-ledger` to submit transactions.

```
var PeerNode = require('flowchain-ledger').PeerNode;
var node = new PeerNode();;
node.submit(data);
```

Please use [flowchain-hybrid](https://github.com/flowchain/flowchain-hybrid) which is the blockchain application built on flowchain-ledger.

## SDK and Prerequisite

* Node.js v8+
* [See Flowchain Documentation](https://github.com/flowchain/flowchain-ledger/wiki)

# Publication

## Presentation

* [Flowchain: A Case Study on Building a Blockchain for the IoT in Node.js - Jollen Chen, Flowchain.co
](https://lc3china2017.sched.com/event/Aedw/flowchain-a-case-study-on-building-a-blockchain-for-the-iot-in-nodejs-ce-jollen-chen-flowchainco), LinuxCon + ContainerCon + CloudOpen (LC3), Beijing, China, June 19-20, 2017.

## Bibliography

This work is based on the research papers.

[1] Chen, J. (2017). [Flowchain: A Distributed Ledger Designed for Peer-to-Peer IoT Networks and Real-time Data Transactions.](https://sites.google.com/site/lddleswc17/program) In: 2nd International Workshop on Linked Data and Distributed Ledgers. Portoroz.

[2] Chen, J. (2017). [Devify: Decentralized Internet of Things Software Framework for a Peer-to-Peer and Interoperable IoT Device](https://sites.google.com/view/aiotas2017/program?authuser=0) In: Advances in IoT Architecture and Systems. Toronto, Canada.

## How to Cite

```
@article{flowchain_2017,
title={Flowchain: A Distributed Ledger Designed for Peer-to-Peer IoT Networks and Real-time Data Transactions},
journal={Proceedings of the 2nd International Workshop on Linked Data and Distributed Ledgers (LDDL2)},
author={Chen, Jollen},
year={2017}
},

@article{devify_2017,
title={Devify: Decentralized Internet of Things Software Framework for a Peer-to-Peer and Interoperable IoT Device},
journal={Proceedings of the Workshop on Advances in IoT Architecture and Systems (AIoTAS2017)},
author={Chen, Jollen},
year={2017}
},
```

# License

Copyright (C) 2016-present Jollen. The source code is licensed under the MIT license found in the [LICENSE](LICENSE) file.
