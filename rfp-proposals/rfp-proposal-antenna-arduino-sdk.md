# RFP Proposal: `Antenna SDK for Arduino boards`

**RFP Category:** `dev`

**Name of Project:** Antenna SDK for Arduino boards

**Link to RFP:** <https://github.com/iotexproject/halogrants/blob/master/rfp-proposals/rfp-ideas.md#antenna-sdk-for-arduino-boards>

**Proposer:** `as-iotex`

**Do you agree to open source all work you do on behalf of this RFP and dual-license under MIT and APACHE2 licenses?:** Yes

# Project Description

Arduino is a great platform for people & makers to experiment, learn and build IoT applications.  
Joining Arduino & IoTeX would take these IoT projects to the next level, allowing users to effectively integrate an IoT-friendly Blockchain into their devices and applications.   While IoTeX already provides some C++ examples (antenna-embedded), a comprehensive antenna-arduino library that implements IoTeX Antenna SDKs and is easily imported into Arduino projects is missing.  
This port will provide account creation, transaction signing, and JSON RPC communication with aIoTeX Full-Node to broadcast transactions (both token transfers and smart contract calls), query transaction status and accounts balance.  
The library will suport popular Arduino boards, including ESP32, ESP8266 and Arduino Nano 33 IoT  


## Deliverables

The final deliverable will be made up by an Arduino library with PlatformIO compatibility. The library will follow the Arduino code standards.  
Along with the library, a set of examples and documentation will be created for the supported Arduino boards.  

## Development Roadmap

### Milestone 1 - JSON-RPC over HTTPS

#### Scope

- **JSON-RPC parser/serializer**: Class with utilities to construct and parse JSON-RPC requests and responses. This will leverage a third party lightweight JSON library such as *JSMN* or *cJSON*
- **IConnection**: Interface for a HTTP/HTTPs connection. Possibly an mock implementation or an implementation for one board (eg. ESP32)
- **Api**: class/interface for the iotex JSON-RPC api. Will implement the following methods, which construct the payload using the JSON-RPC parser, send a request over HTTP using IConnection, parse the response and return it in an adequate struct/class. Implements the following methods (initially)
  - getAccount()
  - getNonce()
  - getTransactionByHash()
- **BigNumber**: there is a need to handle BigNumbers, in order to convert balances fro IOTEX to RAU and vice versa, and also possibly performing arithmetic operations with BigNumbers. This will be provided through the integration of a third party library such as *tiny-bignum-c*

#### Timing

15/05/2021 to 30/05/2021

#### Funding

750$

### Milestone 2 - Signature

- **Transfer**:  a class that represents a transfer. Holds the following data, as well as possibly some utility methods
  - amount
  - recipient
  - payload
  - gasPrice
  - gasLimit

- **Wallet**: a class that represents a wallet. Provides the following methods
  - getPrivateKey(): creates a new wallet and returns the private key
  - getIoTeXAddress(): returns the native IoTeX address
  - getEthereumAddress(): returns the address in the Ethereum format
  - signMessage(): hashes a message using the private key and returns the hash
  - signTokenTransferAction() this will construct the token transfer message then call the signMessage and return the signature. The message must be “constructed” in protobuf format  (version is 1, nonce can be obtained from milestone 1, action will be of type Transfer for token transfers, Execution for contract calls and fields are passed as arguments to the call). <https://github.com/iotexproject/iotex-proto/blob/28696168bf02b64a9fbf71edda0a68a4ad714c08/proto/types/action.proto#L205>

- **Api**: the following methods will be added to the Api class
  - sendTokenTransfer(Wallet, Transfer) will call the wallet.signTokenTransferAction(Transfer) to obtain the signature, will build the signed action, and send it over HTTPS as a test

- **Protobuf**: protobuf encoding is needed for sending actions to the server. This will be handled by integrating a lightweight third party library such as *NanoPb*

- **Signing**: signing of transactions will be done using the existing *antenna-embedded* signing module. This proposal assumes the code in `signer.c` and the existing crypto modules works properly and no modifications need to be done to them (except for minor ones)

#### Timing

01/06/2021 to 15/07/2021

#### Funding

750$

### Milestone 3 - Contract execution

- **Execution**: class that represents a smart contract. Holds the following data and methods
  - contractAddress
  - amount
  - Methods to generate contract data:
    - setupContractData()
    - getData()
  
- **Wallet**: add the following methods
  - signContractExecution(amount,execution)

- **Api**: add the following methods
  - sendContractExecution(wallet, execution)

#### Timing

15/06/2021 to 01/07/2021

#### Funding

750$

## Milestone 4 - Test boards, Examples & publish

Implement the existing interfaces for each of the supported boards:

- ESP32
- ESP8266
- Arduino Nano 33 IoT
- Cellular board - Possibly, depending on time

Create a set of examples and documentation  
Publish the library  


#### Timing

01/07/2021 to 15/07/2021

#### Funding
1250$

## Total Budget Requested

3500$

## Maintenance and Upgrade Plans

The team is committed to maintain and improve the library going forward
