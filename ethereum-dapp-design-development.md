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
5. Web3 Javascript API
  1. Web3 JS Overview
  2. Development Enviroment
  3. Sample DAPP
  4. Connecting to the Node
  5. Getting Node Information
  6. Account List & Balance
  7. Sending Ethers in a Transaction
  8. Solidity Code Compilation
  9. Deploying a Contract
  10. Invoking Contract Methods
  11. Ethereum Events and Logs
  12. Filter, Logs & Watch
  13. Contract Instance Watch & Get
6. Getting Ready to Write Solidity Contracts
  1. Tools for Contract Development
  2. Setting Up a Truffle Project
  3. Coding and Testing
  4. Deploying Contract to Network
7. Ethereum Smart Contract Development With Solidity
  1. Solidity Contract Layout
  2. Solidity Basic Datatypes
  3. Memory Management
  4. Arrays
  5. Special Arrays
  6. Introduction to Functions
  7. Conversions, Globals & THrows
  8. Complex datatypes
  9. Object Orientation
  10. Function and Variable Visibility
  11. Constants & Receiving Ethers
  12. Function Modifiers
  13. Events 

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
*Total Time: 40:38*
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

Web3 Javascript API
==============================
*Total Time: 2:00:13*
-------------------

# Web3 JS Overview - 2:49
  * Overview of web3 API
    - eth
    - net
    - personal
    - db
    - ssh
  * Asynchronous calls
  * Big numbers
    - Manage account balances in Wei

# Development Environment - 8:12
  * Sample Web3 app
    - Created with HTML/Javascript
    - Developed against Geth client
  * Installing NodeJS tools/components
    - Yeoman
    - Gulp
    - Bower

# Sample DAPP - 4:08
  * Walking through a sample decentralized application
  * thedapps.com
  * Running a sample DAPP

# Connecting to the Node - 6:07
  * Navigating through the sample dapp
  * how web3 is injected onLoad

# Getting Node Information - 5:37
  * web3 version object
    - How to set the web3 version
  * web3.net
    - listening / getListening
    - peerCount / getPeerCount
  * Syncing
    - web3.isSyncying(callback)
    - web3.syncing/getSyncing
  * Mining
    - web3.mining/getMining

# Account List & Balance - 7:06
  * web3.eth.getAccounts(function(error,result) {//callback function} )
  * web3.eth.coinbase
    - miner rewards account
  * web3.eth.defaultAccount
  * web3.eth.getBalance
    - balance in wei
    - web3.fromWei(balance_in_wei, 'ether')

# Sending Ethers in a Transaction - 14:00
  * Unlocking and Locking API
    - web3.personal.unlockAccount(account, password, function(error, result) {//callback function})
    - web3.personal.lockAccount(account, function(error, result) {//function code})
    - result = true if successful
    - web3.personal.unlockAccount(account, password, duration)
    - web3.personal.lockAccount(account)
  * Send Transaction
    - web3.eth.sendTransaction(transactionObject, function(error, result) {//callback function})
    - result = transaction hash
  * Transaction Object
    - from (default is web3.eth.defaultAccount)
    - to
    - value (in wei)
    - gas
    - gas price (in wei)
    - data (in hex)
    - nonce

# Solidity Code Compilation - 9:15
  * Compilation Output
    - Bytecode / EVM Code
    - Application Binary Interface
  * Introduction to SOLC
  * SOLC Compiler options
    - solc --bin sample.sol (bytecode)
    - solc --abi sample.sol (application binary interface)
    - solc --combined-json abi,bin... sample.sol (comma seperated list of output components)
    - after this command you can set output with '> ./sol/sample.bin' <-- example

# Deploying a Contract - 11:05
  * web3.eth.contract(abiDefinition array)  - creates contract object
    - Deploying the contract
    - Invoking a contract function
    - Watch for events from contract instance
  * Synchronous deployment
    - var contractInstance = contract.new(constructor_param1, constructor_param2, ..., {transaction object})
    - transaction object data is set to the bytecode of the contract
    - contractInstance.transactionHash << transaction created
    - contractInstance.address >> filled after transaction is mined
  * Asynchronous
    - contract.new(constructor_param1, constructor_param2, ..., {transaction object}, callback(error, result) {})
    - callback function gets called twice in case of success
      1. result = transaction hash
      2. result = contract instance address
  * Deploy using sendTransaction
    - var conData = contract.new.getData(constructor_param1, constructor_param2, ..., {data: bytecode})
    - create transaction object with data set to conData
    - web3.eth.sendTransaction(transactionObject, function(error, result) {//callback function})
    - result will be transactionHash
    - web3.eth.getTransactionReceipt(transactionHash, function(error, result) {//callback function})
    - will return the contract address

# Invoking Contract Methods - 13:42
  * Contract Instance
    - var contractInstance = contract.at(address)
  * Method Invocation
    - contractInstance.Method.call(...)
    - contractInstance.Method.sendTransaction(...)
  * Method.call(...) vs Method.sendTransaction(...)

# Ethereum Events & Logs - 7:13
  * How events are emitted and how logs are created
    - All event logs available on all nodes
    - If watching the dapp gets notified of the event
  * Event/log uses
    - Receive data for transaction
    - Asynchronous trigger
    - Cheap data storage
  * Receive Data for transaction
    - Once mined, the contract sends back the data in an event
    - The event data has the return value for the method that was invoked
  * Asynchronous Notifications
    - Use events to notify a dapp that the contract has been invoked
  * Data Storage
    - Events make logs and you can use those logs to store data
    - Log storage is cheaper than contract storage however logs are not accessible from contracts

# Filter, Logs & Watch - 19:27
  * Watch listens for incoming events
  * Get gets the log data
  * Filter API
    - var filter = web3.eth.filter(options_object_json)
      - strings
        - "latest" - result = block hash of latest block
        - "pending" - result = transaction hash of latest transaction
      - for options_object
        - block range
        - specific contract instance
        - event data to filter
    - filter.watch(callback_func) result = array of events
    - filter.stopWatching()
    - filter.get(callback_func) result = event data

# Contract Instance Watch & Get - 11:32
  * Topics is indexed or topics option
  * fromBlock toBlock and address is additional options
  * contractEvent
    - var contractEvent = contractInstance.allEvent(additionalOptions)
    - var contractEvent = contractInstance.NumberSetEvent(indexedOptions, additionalOptions)
  * Event JSON
    - address
    - block and transaction info
    - removed
    - type of event
    - args json
  * Filter get/watch vs Event get/watch

Getting Ready to write Solidity Contracts
=========================================
*Total Time: 36:55*
-------------------

# Tools for Contract Development - 12:15
  * Downloading an IDE
    - Enabling Solidity Plugin
  * Ethereum client and compiled contract
  * Using Ethereum simulator to testing compiled contracts
  * How to install testrpc
  * Introduction to dapp frameworks
  * Truffle
  * Mocha
    - describe(...)
    - it(...)
    - before()
    - beforeEach()
    - after()
    - afterEach()
  * Chai
    - assert
    - expect
    - should

# Setting Up a Truffle Project - 6:58
  * Initializing Truffle project
    - Create directory
    - truffle init
  * Creating a contract
    - truffle create contract ContractName
  * Deploying contract
    - Add contract to migrations/deploy_contracts.js
    - Run testrpc
    - truffle migrate

# Coding and Testing - 7:35
  * Contract development cycle
    1. Add test cases
    2. Code contract
    3. Compile contract
    4. Test contract
    5. Repeat 2-4 until all test cases pass
  * Coding a calculator contract
  * Creating a test file
    - truffle create test ContractName
    - truffle test pathToTest

# Deploying Contract to Network - 10:07
  * Proper development deployment order
    1. testrpc
    2. testnet
    3. live
  * truffle migrate options
    - --reset
    - -f number
    - --network name
    - --compile-all
    - --verbose-rpc

Ethereum Smart Contract Development with Solidity
=================================================
*Total Time: 2:08:00*
---------------------

# Solidity Contract Layout - 7:18
  * Code layout
    - pragma solidity ^0.4.6 (rejected with compiler version 0.5.x)
    - contact name {
      state/storage variables
      events
      functions
    }
  * Source files can contain multiple contracts
    - Invocation
    - Inheritance
    - Creation
    - Last contract in file gets deployed
    - Can import contracts
      - import "./Account.sol";

# Solidity Basic Datatypes - 12:04
  * Value types are passed by value
  * boolean
    - bool varName;
    - initialized to false
  * integer
    - int num1;  // signed
    - uint num2; // unsigned
    - initialized to 0
    - size specified in 8 bit increments
      - eg. int8, int16, uint32
    - default size is 256
  * Implicit type conversions
    - Compiler allows if no loss of information
      - eg. uint16 -> uint8
  * Explicit type conversions
    - Potential loss of information
      - uint32 x32 = 20;
      - uint24 x24 = uint23(x32);
  * Deduction type conversion
    - Compiler automatically infers type
      - var someVar = x32;
    - useful for receiving multiple values from functions
  * Address value type
    - represents the 20 bye Ethereum address
    - address.balance (in wei)
    - address.transfer(num)
  * Variable Initialization
    - No special keyword to check for uninitialized variable
    - depending on datatype, check for 0 values
      - eg. flag = (owner == address(0x0));
      - flag = (dynamicArray.length == 0);

# Memory Management - 8:41
  * Data Location
    - Storage
      - State variables
      - Local variables
    - Memory
      - Functions
      - Arrays
        - uint[] memory memoryArray;
      - Structs
    - Call data
      - Temporary
      - Managing function calls
      - Is a stack

# Arrays - 6:08
  * Static arrays
    - Fixed size arrays
    - Missing Elements not declared with be initialized to 0
  * Dynamic arrays
    - Size can be changed at runtime
    - dynamic storage arrays can have its size changed (eg. array.length = 6;)
  * Storage arrays
    - uint8[3] arr = [1,2,3]
    - int8[3] arr = [1,2,3] // compilation fails, interpreted as uint8
    - int8[] arr = [int8(1),2,3] // compiles
    - array.push(5); // appends to the array

# Special Arrays - 12:41
  * byte type
    - byte[15] data; // static
    - byte[] data; // dynamic
    - bytes[1-32] data;
    - bytes data; // dynamic
    - bytes32 data; // 32 byte
    - fixed size bytes array is read only
  * byte[] data
    - data = new byte[](4);
    - data = [byte(1),2,3,4];
    - can read/write
    - data.length = 10;
  * bytes data
    - data = new bytes(4);
    - data = [byte(1),2,3,4]; // compilation error
    - can read/write
    - data.length = 10;
  * Strings
    - Dynamically sized
    - similar to bytes array
    - string data = string(bytes_array); // is valid
    - bytes data = bytes(string_data); // is valid
    - hex literals prefixed with hex (eg. hex"001122")
    - Supports escape character
    - Index access is not allowed
    - No string function out of the box but can use external StringUtil libraries
    - Complex string operations may be costly. Can use bytes

# Introduction to Functions - 9:54
  * Return
    - Use keyword returns(...)
    - Multiple return parameters
    - You may name the return parameters
  * Input parameters
    - Declare the arguments with type/name
    - may omit argument name if unused
  * Redeclaration of a variable in a function is not allowed
  * Variables initialized to defaults in the beginning of the function
  * When a function receives multiple values from another function's return, the function gets it as a tuple
  * Tuple
    - List of objects
      - eg. var(name, age) = getOwnerInfo();
    - You may skip a variable in tuple
      - eg. var(name, ) = getOwnerInfo();
  * Function overloading
    - Functions with same name but different input parameters
  * Constructor
    - Constructor function name = name of the contract
    - Only one constructor is allowed
    - deploy eg. (deployer.deploy(Funcs, "Nelson", 31)); // where Funcs(string name, uint8 age) {}

# Conversions, Globals & Throw - 12:46
  * Ether units
    - wei (default)
    - ether
    - finney
    - szabo
  * Time
    - now - global variable returns block time in seconds (from 1970)
    - conversion by suffixing literal with the time units
      - seconds (default)
      - minutes
      - hours
      - days
      - weeks
      - years
  * Block
    - block.number - current block number
    - block.number - address of current blocks miner
    - block.timestamp - block time (same as now)
    - block.difficulty - current blocks difficulty
    - block.gaslimit - gas limit
    - block.blockhash(uint blkNum) returns(bytes 32)
      - hashes of most recent 256 blocks (excluding current)
  * Msg
    - msg.data - call data in bytes
    - msg.sender - caller's address
    - msg.sig - function identifier (first 4 bytes of call data)
    - msg.value - # of wei sent in the message, only available in payable function
  * tx
    - tx.gasprice - gas price for the transaction
    - tx.origin - address that originated the transaction (shouldn't use)
  * throw;
    - aborts the transaction execution
    - all state changes are reverted
    - no ethers are sent out
    - ethers received in transaction is returned
    - gas is spent (i.e there is a cost)
    - transaction is recorded on the chain; nonce is valid and recorded
    - no catch (as in try/catch)
  * assert(condition)
    - throws if condition is not met
  * Cryptography hash functions
    - deterministic
    - quick
    - infeasible
    - any change will change the hash
    - collision resistant
  * Crypto functions
    - takes multiple bytes parameters and produces bytes32
      - keccak256(...)
      - sha3(...)
      - sha256(...)
    - takes multiple bytes parameters and produces bytes20
      - ripemd160(...)

# Complex datatypes - 15:51
  * Mapping type
    - Hashtable like structure
    - Allowed only as storage or state variable
    - mapping(address -> uint) balances;
    - key can be any type except mapping
    - value type can be mapping
    - value exists for all keys (default given to uninitialized)
    - keccak256(Key data) hash is stored
    - by default is not iterable
    - No concept of length (can do it by a separate counter)
  * Enums
    - Create custom types with finite set of values
      - eg. enum TransferType {Domestic, Foreign} // no semicolon
    - not part of the ABI definition
    - explicit conversion to/from all integer types
  * Struct
    - Cannot have a member of its own type
    - Can be contained in arrays and mappings
    - not part of the ABI definition
    - external function calls cannot send/receive struct types
    - internal function calls can send/receive struct types
      - eg. function someFunc(country ctry) internal {}
    - Default for struct type local variable is Storage type

# Object Orientation - 8:11
  * Solidity supports
    - function overloading
    - inheritance
      - abstract Contracts
      - supports multiple inheritance
    - polymorphism
  * Abstract contract
    - no keyword for abstract contracts
    - functions declared but no body provided
    - inheritance relation created using the keyword 'is'
      - eg. contract ObjectOrientation is AbstractContract, UtilContract {}
    - Derived contract constructor need to provide the arguments for all the base contracts
      - eg. function AbstractContract(string name) {}
            function ObjectOrientation(string agentName, uint8 rate) AbstractContract(agentName) {}

# Function and Variable Visibility - 13:32
  * Visibility Overview
    - public
      - part of contract interface
      - automatic getter for state variable
      - public function calls are internal and external
    - private
      - available only within the contract only
      - not even available in a derived contract
    - internal
      - can invoke function internally in contract
    - external
      - can be invoked by other contracts as long as they have the address and function information
      - can be invoked internally using 'this.'
  * Functions can be created as types
    - eg. function(string memory) internal returns(uint) lengthFunctionVar;

# Constants & Receiving Ethers - 9:25
  * Constant variable must be initialized at compile time
    - Cannot be initialized in the constructor
    - Structs cannot be declared constant
    - Constant functions promises not to change state
      - not enforced by a compiler
  * Fallback function
    - an un-named function in the contract
    - invoked without the data i.e., the function signature
    - restrictions:
      - no arguments
      - cannot return anything
      - maximum gas spend = 2300 gas
  * Receiving ethers
    - contract can receive ethers by way of payable fallback function
    - Invoked when ethers are received (msg.value) without data
    - Exceeding the gas in fallback function will
      - throw exception
      - send back the ethers
      - best practice is to log an event in the fallback function
    - a function must be marked payable to received ethers
      - ethers are held in the contract not the function

# Function Modifiers 5:34
  * Modifiers changes the behavior of a function
  * Can make modifiers
    - A throw in modifier halts the execution
    - A return in modifier returns from modifier body
    - Modifiers can take arguments
      - passed from the argument of the function
    - Local variables from within modifiers not available in functions
    - Multiple modifiers may be applied to functions
    - The order that modifiers are executed is left to right
    - May be inherited and may be overridden by child contract

# Events - 5:55
  * Declaration of event looks like a function without a body
    - eg. event NewHighBid(address indexed who, string, name, uint howmuch);
  * Events are invoked in functions, like functions
    - eg. func {
      NewHighBid.(msg.sender, name, msg.value);
    }
