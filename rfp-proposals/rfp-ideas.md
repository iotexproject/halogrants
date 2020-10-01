# RFP Ideas

## High Priority
- [Dashboard to Track Halo projects](#dashboard-to-track-halo-projects)
- [Token Minting Tools](#token-minting-tools)
- [Stable Coins](#stalbe-coins)
- [Innovative Assets](#innovative-assets)
- [Hardware Wallet Support](#hardware-wallet-support)
- [Browser Extention Wallet](#browser-extention-wallet)
- [IoTeX All-in-One For Dummies](#iotex-all-in-one-for-dummies)
- [Privacy-preserving Healthcare Applications](#privacy-preserving-e-health-applications)
- [Privacy-preserving XRC20 Tokens](#privacy-preserving-xrc20-tokens)
- [Privacy-preserving Swap of Regular XRC20 Tokens](#privacy-preserving-swap-of-regular-xrc20-tokens)
- [Digital Twin for Devices](#digital-twin-for-devices)
- [Antenna SDK for Arduino Boards](#antenna-sdk-for-arduino-boards)


## Low Priority
- Multi-language SDKs (Python, Ruby, Swift, Kotlin)
- Code labs: DIY creative Dapps

**Note that projects tagged with `WIP` indicating a team is working on it.**

We also accept **Open-ended Proposals** where you can suggest your own project idea.

*Have a question about any of these RFPs? Email support@iotex.io*

&nbsp;

------

### Dashboard to track Halo Projects (WIP)

While we track progress of every Halo projects on Github to achieve the highest transparency, it would be great to have a nice dashboard to track projects visually and user-friendly. The required features are
- automatic tracking and visualization of applications
- automatic tracking and visualization of milestones of projects
- automatic tracking and visualization of project traction, e.g., DAU, daily active txs and so on


&nbsp;

### Token Minting Tools (WIP) ###
Build a user-friendly web service for user to mint XRC20 tokens on top of IoTeX, e.g., https://tokenmint.io/, where user can mint a new token within a few clicks.

&nbsp;

### Stable Coins ###
Stablecoins are cryptocurrencies designed to minimize the volatility of the price of the stablecoin, relative to some "stable" asset or basket of assets. There are couple of ways to develop a stable coin on IoTeX and we are open to all:
- crosschain-transferring of stable coins from Ethereum (and other blockchains) to IoTeX blockchain
- natively issue a stable coin on IoTeX blockchain which can be pegged to a cryptocurrency, fiat money, or to exchange-traded commodities (such as precious metals or industrial metals). This one can be asset-backed or seigniorage-style.

&nbsp;

### Innovative Assets ###
Minting and issuing new innovative assets as financial experiments is welcomed! IoTeX provides the smart contracts and tools, decentrealized exchange [mimo](https://mimo.finance), edge oracle (upcoming), hardware devices as well as an active and encouraging community to support innovation in #DeFIoT space!

&nbsp;


### Hardware Wallet Support ###
A hardware wallet is a special type of cryptocurrency wallet which stores the user's private keys in a secure hardware device. They have major advantages over standard software wallets: private keys are often stored in a protected area of a microcontroller, and cannot be transferred out of the device in plaintext. While core-dev is working with Ledger closely to lauch IOTX wallet for nano S/X wallets, we desire to support native IOTX on other hardware wallets such as Trezor, KeepPay and many others. Help us develop firmwarre for mainstream hardware wallets!

&nbsp;

### Browser Extention Wallet (WIP) ###
IOTX wallet such as ioPay (https://iopay.iotex.io/) comes with two flavours - desktop version (supporting Windows, MacOS and Linux) and mobile version (iOS and Android). Having a wallet as a browser extention will hugely invcentive Dapps to integrate with IoTeX blockchain and be beneficial for the ecosystem. This browser extention should coome with all features similar to ioPay, e.g., account management, send/review transaction, invoke smart contract, safe and easy to use.

&nbsp;

### IoTeX All-in-One For Dummies ###
[Dummies Book Series](https://www.dummies.com) is a popular collection of books that always taking on concepts and making them easy to understand. Dummies helps everyone be more knowledgeable and confident in applying what they know. We aim to have an educational website called "IoTeX All-in-One For Dummies" that covers all IoTeX vision, techonology and products for all users, developers and investors.

&nbsp;

### Privacy-preserving e-Health Applications ###
Despite the potential gains, there are several obstacles that limit the wider development of e-health applications. Among these are the perceived threats to the security and privacy of patients' health data, and a widely held belief that these cannot be adequately addressed. We would recommend developers to implement privacy-preserving e-health applications based on customizable hardware such as [e-Health Sensor Platform V2.0 for Arduino and Raspberry Pi](https://www.cooking-hacks.com/documentation/tutorials/ehealth-biometric-sensor-platform-arduino-raspberry-pi-medical.html) and IoTeX platform.

&nbsp;

### Privacy-preserving IOTX and XRC20 Tokens ###
Privacy-preserving XRC20 tokens are preferred in some use cases. Implementing such a token using zk-SNARK such as [Aztec Protocol](https://www.aztecprotocol.com/) or [Zether](https://crypto.stanford.edu/~buenz/papers/zether.pdf) will be an impact initiative! Comparing to Ethereum, we do have the plan to support additional instructions for EVM to promote the usage of ZK.

&nbsp;

### Privacy-preserving Swap of IOTX and XRC20 Tokens ###
While pivacy-preserving XRC20 tokens are important, the privacy-preserving "swap" of regular XRC20 tokens are interesting too! The academic researchers we are working with have already finished the design of such a scheme called [PrivateEx](https://www.researchgate.net/publication/340270180_PrivateEx_privacy_preserving_exchange_of_crypto-assets_on_blockchain) and we are calling for a live implementation of it in the "Uniswap" fashion!

&nbsp;

### Digital Twin for Devices ###
A digital twin is a digital replica of a device which can be implemented as a DAO using smart contracts. Some sort of protocol needs to be designed to "bind" a device to its digital twin based on Decentralized Identity (DID). Once a device gets represented by a digital twin on chain, IFTTT can be implemented as a DAO, which could be a fun and profitable project! 

&nbsp;

### Antenna SDK for Arduino Boards ###
Arduino is a great platform for people & makers to experiment, learn and build IoT applications. Joining Arduino & IoTeX would take these IoT projects to the next level, allowing people to effectively integrate an IoT-friendly Blockchain into their devices and applications. While IoTeX already provides some C++ examples (antenna-embedded), a comprehensive antenna-arduino library that implements IoTeX Antenna SDKs and is easily imported into Arduino projects is missing. Such a port should provide at least Account creation, Transaction signing, and gRPC communication with a IoTeX Full-Node to broadcast transactions (both token transfers and smart contract calls), query transaction status and accounts balance. This should run on the most popular Arduino boards, including the UNO, Nano & Mega.      

&nbsp;

