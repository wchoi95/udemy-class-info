**Ethereum : Decentralized Application Design & Development**
=============================================================

**Note: Both development and marketing staff would benefit from learning
section 1.1 - 2.7 as it introduces blockchain basics and gets them familiar
with Ethereum. Please note that these sections only cover P2P networking,
blockchain, Ethereum and smart contracts. Marketing staff may need to learn
extra material if they are working with other use cases for blockchain.
Section 2.8 and onwards will be specifically targeted towards Solidity
developers. It will get them familiar with the Geth environment and guide them
through making a dapp on the Ethereum network.**

## Index
1. Blockchain Foundational Concepts
  1. Introduction
  2. Blockchain Foundational Concepts
  3. Blockchain 101
  4. Ethereum 101
2. Ethereum Blockchain - Using the wallet for interacting with the network
  1. Ethereum Decentralized Applications
  2. Ethers, Gas, EVM
  3. Ethereum Networks
  4. Consensus Models
  5. Ethereum Wallet
  6. Ethereum Wallet Account Types
  7. Managing Contracts in a Wallet
  8. Meta Mask
  9. Developing Contracts using Remix
3. Ethereum Clients, Network and Geth
  1. Ethereum Client or Node
  2. GoLang Ethereum Client
  3. Setting up the client testnet
  4. Setting up RPC for the geth client
  5. Working with console options and commands
  6. Account and Mining
4. Geth Javascript Management API
  1. Geth Console API
  2. Geth Javascript API (Admin)
  3. Geth Javascript API (Personal)
  4. Geth Javascript API (Miner)
  5. Geth Javascript API (Transactions)
  6. Geth Javascript API (Debug)

**Please note that the notes taken below only outline the topics in detail.
For learning content please watch the videos and only use this as a guideline
for the topics covered in the Udemy class**

Blockchain Foundational Concepts
================================
*Total Time: 31:35*
-------------------

# Introduction - 2:54
  * Introduction to the course

# Blockchain Foundational Concepts - 7:21
  * Introduces peer to peer network
  * Introduces Bitcoin and its history
    - Decentralized
    - Open source
    - Public ledger
    - Fees
    - Miners
    - Satoshi Nakamoto
    - Blockchain

# Blockchain 101 - 13:01
  * Introduces blockchain
  * Centralized vs decentralized nodes
  * How an Ethereum contract is stored on the blockchain
  * Traditional ledger vs distributed ledger
  * Immutability of the ledger
  * Cryptography
    - Public/private key

# Ethereum 101 - 8:19
  * Difference between Bitcoin and Ethereum
  * History of Ethereum
  * Introduction to smart contracts and how they work
  * Introduction to ether
  * Introduction to wallets and dapps


Ethereum Blockchain - Using the wallet for interacting with the network
=======================================================================
---------------------

# Ethereum Decentralized Applications - 6:38
  * Web apps vs dapps
  * Introduction to how dapps work
    - Gas/fee
    - Miners
    - Transaction validation
  * Process of a dapp smart contract
  * Coding language that create dapps

# Ethers, Gas, EVM - 9:23
  * Introduction to ether
    - Denominations (different value types)
    - How ether is created
  * Introduction to the Ethereum Virtual Machine
  * Introduction to gas and how it is calculated
    - Opcodes and gas cost
    - gasUsed, gasPrice, startGas & transaction fee
    - Escrow and how refunds are calculated
    - What happens when not enough gas is provided

# Ethereum Networks - 10:34
  * Live network vs test-net vs private network
    - Different types of networks such as Ropsten & Kovan
  * Reasons to use a private network
  * Network interactions with:
    - Wallet
    - Dapp
    - Block explorer
  * Introduction to blockchain explorer
    - How to use etherscan.io
  * Etherparty explorer for private networks

# Consensus Models - 13:43
  * Introduction to consensus
    - How blocks get created
    - Proof of work and proof of stake
    - Incentives
  * How proof of work is done
    - Hashing functions
    - example of a puzzle
    - How difficulty of puzzles are set
    - Ethereum proof of work process
  * How proof of stake is done
    - Ethereum's plan to switch to proof of stake
    - Benefits in switching to proof of stake

# Ethereum Wallet - 9:35
  * How to install and use the official Ethereum wallet
    - How to mine
    - How to send funds
  * How to reset your wallet
  * Ether faucets

# Ethereum Wallet Account Types - 14:59
 * Account vs Contract Account
 * Contract Account
   - Single owner vs MultiSig
 * How to create wallet contracts
 * How MultiSig contracts work

# Managing Contracts in a Wallet - 8:07
  * Different types of contracts
  * Introduction to custom contracts
    - How to deploy a custom contract on the mist wallet
    - How to use the functions
    - How to add a custom contract

# Meta Mask - 7:43
  * Benefits and purpose for using Meta Mask
  * How to install and use Meta Mask
    - Exporting/Importing accounts
    - Sending and receiving funds
    - web3 object to browser app / creating a single page application
    - Limitations to Meta Mask compared to a wallet

# Developing Contracts using Remix - 7:47
  * Introduction to Remix
  * Browser Solidity
    - How to use with Meta Mask
  * How to use functions on contracts that are already deployed

Ethereum Clients, Network & Geth
================================
*Total Time: 49:27*
-------------------

# Ethereum Client or Node - 7:16
  * How Ethereum clients or nodes interact with each other and dapps
  * Technologies used between communication to/from the node

# GoLang Ethereum Client - 7:35
  * How to install Geth
  * Introduction to Geth
  * Different Geth terminal commands
    - options
    - command options
    - args

# Setting up the client testnet - 8:53
  * Configuration options
    - --identity "MyTestNode"
    - --datadir "/data-dir"
    - --keystore "/key-dir"
    - --networkid "value"
    - --testnet
    - --fast
    - --dev
  * Creating a script to efficiently start a node
  * Creating a node on the testnet

# Setting up RPC for the geth client - 6:12
  * IPC-RPC
  * Connecting from dapp to client over the network
    - JSON-RPC
    - WS-RPC
  * JSON-RPC
    - --rpc
    - --rpcapi
    - --rpcaddr "host"
    - --rpcport "port"
    - --rpccorsdomain
  * WS-RPC
    - --ws
    - --wsapi
    - --wsaddr "host"
    - --wsport "port"
  * Using JSON-RPC to connect to a port

# Working with console options and commands - 8:03
  * API & Console Options
    - --preload "files,.,."
    - --jspath "loadscript"
    - --exec "JS statement"
  * Console interface commands
    - console
    - attach "pipe address"
  * How to preload javascript files
  * Using exec to execute javascript in a non interactive way

# Account and Mining - 11:28
  * Account commands
    - account new
    - account list
    - account update
    - account import
  * Creating a new account with keystore file
  * Account options
    - --unlock "comma seperated list of address/index"
    - --password "password file"
  * Mining options
    - --mine
    - --minerthreads
    - --etherbase
    - --gasprice "value"
    - --extradata "somedata"
    - --targetgaslimit "value"

Geth Javascript Management API
==============================
*Total Time: TBD*
-------------------

# Geth Console API - 6:07
  * Javascript API
    - Supports web3 dapp API
    - Go-Ethereum supports additional API
  * WEB3 API Commands
    - eth - Ethereum blockchain related methods
    - net - Node's network status
    - db - Get/put for local LevelDB
    - ssh - P2P messaging using Whisper
  * Management API Commands
    - admin - node management
    - personal - account management
    - miner - miner management
    - txpool - transaction pool
    - debug - node debugging

# Geth Javascript API (Admin) - 6:58
  * Admin Commands
    - admin.nodeInfo
    - admin.datadir
    - admin.peers
    - admin.addPeers(url)
    - admin.startRPC(host, port, listOfAPI)
    - admin.stopRPC()
    - admin.startWS(...)
    - admin.stopWS()
    - admin.setSolc('pathToSolidityCompiler')

# Geth Javascript API (Personal) - 5:34
  * Personal Commands
    - personal.newAccount("password")
    - personal.listAccounts
    - personal.importRawKey(keydata, paraphrase)
    - personal.unlockAccount()
    - personal.lockAccount()
    - personal.sendTransaction(txn_object, "paraphrase")

# Geth Javascript API (Miner) - 3:08
  * Miner Commands
    - miner.start(num_threads)
    - miner.stop()
    - miner.setEtherbase(addr)
    - miner.setGasPrice(num)
    - miner.setExtra(data)

# Geth Javascript API (Transactions) - 10:53
  * Nonce explained
  * txpool commands
    - txpool.status
    - txpool.inspect
    - txpool.content

# Geth Javascript API (Debug) - 7:58
  * Debug commands
    - debug.verbosity(level)
    - debug.dumpBlock(number)
    - debug.traceBlockByNumber(number)
    - debug.traceBlockByHash(hash)
    - debug.traceTransaction(txHash)
    - debug.gcStats()
    - debug.memStats()
    - debug.cpuProfile(file, seconds)
    - debug.startCPUProfile(file)
    - debug.stopCPUProfile()
    - debug.goTrace(file, seconds)
    - debug.stacks()
    - debug.vmodule(string)
