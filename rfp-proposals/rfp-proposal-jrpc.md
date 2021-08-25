# RFP Proposal: `WebOS JRPC Console`

**RFP Category:** `dev`

**Name of Project:** WebOS Console

**Link to RFP:** https://github.com/iotexproject/halogrants/blob/master/rfp-proposals/rfp-ideas.md#innovative-assets

**Proposer:** `jrynkiew`

**Do you agree to open source all work you do on behalf of this RFP and dual-license under MIT and APACHE2 licenses?:** Yes

# Project Description

This project focuses on developing a new XRC20 token blockchain network on the IoTeX blockchain. JRPC has been seeded with assets already and is tradeable on mimo. The token has been released with low supply on mimo (only several thousand) and the total supply is 1,000,000 JRPC. The concept behind this token is to implement a "mining" token on the Roll-DPoS based IoTeX network. This can be accomplished via a series of proofs of work done not by a computer per se, but instead by a miner, a developer, working on the IoTeX blockchain to solve complicated puzzles via a web console (or windows/linux binaries).

## Deliverables

1. A WebOS integrated antenna-js / iotex-antenna-embedded web version + ioctl type application. The app will provide full command user access to IoTeX mainnet.
2. A 3D/2.5D web interface hosting the command console - compiled in Emscripten, a cross compliation tool developed for golang/C++. The basic rendering is done by SDL2/OpenGLes.

## Development Roadmap

**Milestone 1: JRPC token roadmap - long term scope / whitepaper + investor acquisition.**

As part of this roadmap I will need to consult with IoTeX as to how far they are willing to push their project, to integrate into the JRPC space. I am willing to provide the JRPC token address to delegates to include it in airdrops / airdrips.

I will need to provide a proof of work mechanism for obtaining the JRPC token via Command Console available locally (via win32 / win64 binaries, Linux x86 / x64 binaries) and via Web Console.

This is a planning phase, no functionality yet. Documentation only.

People working on project: 1 (until further funding) - 2 weeks full time, 5 weeks part-time

**funding required: 5,000 IOTX**


**Milestone 2: WebConsole development and cross platform implementation** 

Implement JRPC Web Console available on demand on any continet on any device. Currently Windows/Linux/Mac computers running Chrome/Firefox/Opera/Edge are supported. Mobile versions are compatible with Chrome on Android (have not tested any other browsers on Android), but usage is clunky. Win32 binaries and Linux binaries are available, but I am working on a fully integrated web browser console which will integrate the iotex ioctl like functionality into it. This is the priority for me. Safari / iOS excluded from this milestone, as it is out of my control that they do not support WebGL content yet.

Deliverable: two seperate versions of WebOS - console only Desktop + Web and a Mobile version (web only). Basic console  functionality only on both

People working on project: 1 (until further funding) - 10 months part-time (further help can be found if funding for this project is achieved. Please let me know beforehand if you are interested in this scope, and if you would like to make it a priority)

**funding required: 10,000,000**


**Milestone 3: WebOS integration into the IoTeX space**

Full implementation of the iotex-antenna-js or iotex-antenna-embedded (cross compiled) into a web based command console. This console will allow for the development of smart contracts, creating accounts, deploying contracts, deleting accounts, all the possible features that IoTeX currently supports via command line interaction via ioctl and other simialr tools.

Deliverables: The same as above, including additional functionality of extended/full functionality of the web based ioctl implementation.

People working on project: 1 (until further funding) - 10 months full time

**funding required: 5,000,000**


## Total Budget Requested

15,005,000 IOTX

## Maintenance and Upgrade Plans

I will be developing this project further with funding or not, it doesn't matter, so upgrade and maintenance is a must - it is part of the long term goal. The Ioctl development commitment from IoTeX is required to make this long term commitment sustainable. SDL and Emscripten are being regularly maintained, so third party libraries should not be a problem.

# Team

## Contact Info

rynkiewicz.jeremi@gmail.com

## Team Members

Jeremi Rynkiewicz

## Team Member LinkedIn Profiles

https://www.linkedin.com/in/jrpcpl/

## Team Website

https://jrpc.pl

## Relevant Experience

I am a cross platform developer, as my web based applications must work smoothly both on linux and emscripten based cross compiled code on Windows native browsers. Windows native binaries are available if third party libraries support them (for now they do). I am a full stack developer, with experience in docker commands, nodejs, html, js, css + emscripten, c++.
I have experience in php and e-mail server setup. Server architecture, windows server administration, and linux networking is a must line my line of work.

## Team code repositories

https://github.com/jrynkiew/WebOS

# Additional Information

Benefit to the token economy and the ioctl promotion as a viable tool to use the blockchain, as very few people interact with the blockchain currently with full control.
