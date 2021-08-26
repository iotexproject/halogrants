# Open Grand Proposal: `Drive Slow/Safe`

**RFP Category:** `trusted devices`

**Name of Project:** `Drive Slow/Safe`

**Proposer:** `nicky-ru`

**Do you agree to open source all work you do on behalf of this RFP and dual-license under MIT and APACHE2 licenses?:** Yes

# Project Description

Imagine a city, where people drive vehicles carefully, without hurry and
get bonuses for their safe driving. Sounds good, but how to realize it?

In this project we introduce a new concept that is called Drive and Earn. Drive and
Earn allows people to earn SAFM (SAFe Mile) tokens while driving their cars.

SAFM in combination with Pebble tracker and Drive Slow/Safe smart contract is a perfect
mixture where people can earn while driving and get verifiable data of their
driving behavior.

## Tokenomics

### Overview

Drive Slow/Safe is fueled by SAFM (SAFe Mile) token, which is designed to
incentivize safe drivers and to use Dapp functionality. SAFM is pre-mined.

- Total supply: `1,500,000,000,000 burnable`
- SAFM Utility:
  - Request proof of track (with or without speed values)
  - Request proof of speed (or proof of not exceeding speed limitation)

The 90% amount of issued tokens will be locked in Drive Slow/Safe contract, 10% of it
stays by development team for Maintenance;
The only way to emit this coins is through incentives for safe driving.

### Roles and rewards

There are two roles in Drive Slow/Safe Dapp:

| Roles         | How to become          | Benefits             |
| ------------- |:----------------------:| --------------------:|
| Miners        | Drive and earn rewards | SAFM incentives      |
| Users         | Request proofs         | Verified data, alibi |

**Miners**: Each new participant of the current Dapp is a "Miner" by default. Each Miner will
get rewards 10 SAFM/mile. Possible industries, who will be interested in mining
SAFM: Taxi, Cargo, Delivery and so on.

**Users**: Any holder of Pebble tracker will have access to the live state of his device:
in UI he can see real-time information about motion, location and environment.
Nevertheless this data is just taken from S3 bucket, and it is still not verified by default.
The participant can request to verify some bunch of data, becoming a User. The verified
data will be written to blockchain, and as a result can be used to prove location or speed of the
User.

These two roles provide supply and demand of the token accordingly.

### Examples

Scenario 1:
Bob is Uber taxi driver, he wants to increase his income. He buys and installs Pebble Tracker
into his car and register this device in Drive Slow/Safe dapp. He starts to get SAFM
for each driven mile. Any time he can claim his rewards and sell it in some DEX or even
participate as liquidity provider in pairs with SAFM.

Scenario 2:
Alice has just bought her brand new Pebble tracker to try it out. She also registered in
Drive Slow/Safe dapp just for fun. In one sunny day she was by mistake accused in speeding,
but in reality she is a safe driver and she has never been at the place where the speeding
occurred. She is lucky to have her account in Drive Slow/Safe, because with this Dapp she
can get the proof of riding within speed limit and being absolutely in other place that time.
But at that moment she has not enough SAFM to request proof yet. She goes to her favorite DEX
and buys some SAFM. Now she can request proof and defend herself.

### SAFM Token

SAFM is XRC20 Token. There is two ways of acquiring it:
- By earning rewards while driving;
- Buy from other participants (Miners) in DEX;

The value of the token will be maintained by limited liquidity and burning.

**Limited liquidity:** the Drive Slow/Safe smart contract will issue tokens only through rewards.
**Burning:** the coins paid for each request of proof will be partially burned and partially returned to the Smart Contract.

Burn to Return ratio is TBD, under consideration is the related to the date circulating supply and Users activity.

## Deliverables

The final product is a working Dapp, where users can add/register new Pebble Tracker,
view their driving behavior (data from Pebble Tracker sensors) and claim their rewards.

Moreover we will set up a backend, that will facilitate the communication between
Pebble devices and the Smart Contract.

## Development Roadmap

Milestone 1 (Smart contract and basic UI):
- Smart Contract is tested locally with Ganache;
- Smart Contract is tested on IoTeX Testnet;
- Basic ui (using iotex dapp sample v2);
- User can add, register, remove device;
- User can see a dashboard with information about his driving behavior (motion, GPS, environment);
- User can view accumulated SAFM rewards;
- User can claim SAFM Rewards;
- Smart contract can check data integrity and signer of the message;
- Upon incoming request from a User the Smart contract can combine a bunch of verified datapoints into a verified track;
- Smart contract can distribute SAFM rewards to the whitelisted users;

Milestone 2 (Backend):
- Pebble tracker simulator send register request to AWS IoT;
- AWS IoT receives data from registered devices and stores it in S3 bucket;
- UI can access data in S3 bucket to feed dashboard with it;
- Testing Project with simulated data (pebble simulator uses data from pre-generated CSV);

Milestone 3 (Production):
- Test scalability (tests with 1000, 10,000 and 100,000 simulated devices);
- Improve UI (should be simple, clean and fast);
- Deploy on IoTeX Mainnet;

---
| Number                        | Deliverable                     | Date       | role                | funding require |
| ----------------------------- | ------------------------------- | ---------- | ------------------- | --------------- |
| 1.Smart contract and basic UI | Dapp on Testnet without backend | 2021-10-01 | nicky-ru: fullstack | 100,000 IOTX    |
| 2.Backend                     | Dapp on Testnet with backend    | 2021-11-01 | nicky-ru: fullstack | 150,000 IOTX    |
| 3.Production                  | Dapp on Mainnet with backend    | 2021-12-01 | nicky-ru: fullstack | 100,000 IOTX    |

## Total Budget Requested

Total funding required: 350,000 IOTX (7000 USD in the beginning of the August).

The use of funds:
- AWS EC2 for server and device simulators;
- AWS IoT for communication with devices;
- AWS S3 for storing device messages;
- Dapp hosting;

## Maintenance and Upgrade Plans

Maintenance:
- Active searching for new usability of the SAFM;

Posible upgrades:
- Add lending/insurance functionality;
- Add decentralized governance;

# Team

## Contact Info

email: nikitkaruban@gmail.com;

discord: sea_of_zhou

## Team Members

- nicky-ru

## Team Member LinkedIn Profiles

- [nicky-ru: LinkedIn](https://www.linkedin.com/in/nikita-r-41122887)

## Team Website

Don't have at the moment

## Relevant Experience

nicky-ru has bachelor's degree in Computer Science and Technology. His hobby is
dapp development He's got some valuable experience with Pebble Tracker from "Power
Your DApp With Verifiable Real-World Data" bounty which can accelerate the development
of the current project. This project is mainly
derived from his [original project - Drive Slow/Safe](https://github.com/nicky-ru/drive-slow-safe),
but with some design improvements;

## Team code repositories

[Drive Slow/Safe](https://github.com/nicky-ru/drive-slow-safe)

# Additional Information

Our last project was mentioned in the [Winners showcase](https://medium.com/iotex/iotex-gitcoin-gr10-hackathon-winners-showcase-256b1a4b23e2) under Honorable Mentions;

We hope that this new use case will bring new users to the IoTeX community, increase
demand for Pebble devices and make the situation on the roads safer.
