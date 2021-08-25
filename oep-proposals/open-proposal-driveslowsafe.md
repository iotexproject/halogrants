# Open Grand Proposal: `Drive Slow/Safe`

**RFP Category:** `trusted devices`

**Name of Project:** `Drive Slow/Safe`

**Proposer:** `nicky-ru`

**Do you agree to open source all work you do on behalf of this RFP and dual-license under MIT and APACHE2 licenses?:** Yes

# Project Description

Imagine a city, where people drive vehicles without hurry, carefully, as if they
transport something precious. Imagine these people are happy to drive their cars
safely. Sounds good, but how to realize it?

In this project we introduce a new paradigm that is called Drive and Earn. Drive and
Earn allows people to stake their IOTX (or another collateral) through our Smart Contract
and in addition to stacking rewards be incentivized for their safe drive.

How do we know that the User drives safe? Smart Contract can receive the driving behavior
data from IoTeX Pebble Trackers installed into users' vehicles and make decisions based on
this data. The following sensors will be used: motion (speed and shake), location (GPS
data to check allowed speed at the datapoint) and environment (gas emission).

The source of incentives are "fines" from unsafe riders.

## Deliverables

The final product is a working Dapp, where users can add/register new Pebble Tracker,
stake IOTX, view their driving behavior and track their incentives (staking rewards and
safe ride bonuses).

Moreover we will set up a backend, that will facilitate the communication between
Pebble devices and the Smart Contract.

## Development Roadmap

Milestone 1 (Smart contract and basic UI):
- Smart Contract is tested locally with Ganache;
- Smart Contract is tested on IoTeX Testnet;
- Basic ui (using iotex dapp sample v2);
- User can add, register, remove device;
- User can see a dashboard with information about his driving behavior (speed, distance, gas emission);
- User can deposit/withdraw IOTX;
- Smart contract can check data integrity and signer of the message;
- Smart contract can fine unsafe riders and incentivize safe riders;
- Smart contract can stake/unstake IOTX;
- Smart contract records only unsafe riding;

Milestone 2 (Backend):
- Pebble tracker simulator send register request to AWS IoT;
- AWS IoT receives data from registered devices and stores it in S3 bucket;
- A server pulls data (frequency TBD, but approx once a minute) from S3 bucket
and calls Smart Contracts function "check data";
- If data contains information about unsafe driving, the server sends the message to
the Contract again, and consequently writes it into blockchain.

Milestone 3 (Production):
- Test scalability (tests with 1000, 10,000 and 100,000 simulated devices);
- Improve UI (should be simple, clean and fast);
- Deploy on IoTeX Mainnet;

---
| Number | Deliverable | Date | role | funding require |
| ------------- | ------------- | ------------- | ----------- | ---------- |
| 1.Smart contract and basic UI | Dapp on Testnet without backend  | 2021-10-01 | nicky-ru: fullstack | 100,000 IOTX |
| 2.Backend | Dapp on Testnet with backend | 2021-11-01 | nicky-ru: fullstack | 150,000 IOTX |
| 3.Production | Dapp on Mainnet with backend | 2021-12-01 | nicky-ru: fullstack | 100,000 IOTX |

## Total Budget Requested

Total funding required: 350,000 IOTX (7000 USD in the beginning of the August).

The use of funds:
- AWS EC2 for server and device simulators;
- AWS IoT for communication with devices;
- AWS S3 for storing device messages;
- Dapp hosting;

## Maintenance and Upgrade Plans

Possible upgrades:
- Deposits of coins other than IOTX;
- Add lending/insurance functionality;
- Issue special XRC20;

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
