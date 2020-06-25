# RFP Proposal: `IoTeX Online IDE`

**RFP Category:** `dev`

**Name of Project:** IoTeX Online IDE

**Link to RFP:** https://github.com/iotexproject/halogrants/blob/master/rfp-proposals/rfp-ideas.md#online-ide

**Proposer:** `bhaskarSingh`

**Do you agree to open source all work you do on behalf of this RFP and dual-license under MIT and APACHE2 licenses?:** Yes!

# Project Description

We plan to make/upgrade IoTex Online IDE with features that map completely to a smart contract developer lifecycle which looks like the following: 
1. Writing contract code. 
2. Compiling smart contract code. 
3. Deploying smart contract (to testnet/mainnet). 
4. Testing smart contract code. 
5. Exploring/interaction with deployed contract to change contract storage state.  

The vision is to create a one stop integrated platform that fulfill all developer needs, especially core-dev needs. 


## Deliverables


We will extend IoTeX online IDE with the following features under each lifecycle stage: 

1. Writing Contract code: 
    * Add functionality to connect online IDE to local filesystem by integrating [remixd](https://remix-ide.readthedocs.io/en/latest/remixd.html)
    * Add suitable and contextual error messages. 

2. Compiling smart contract code: 
    * Support for Solidity 0.6.0

3. Deploying contract: 
    * Fixing bugs if any with other injected providers like IoPay. 
    * Use iotex-antenna for deploying bytecode to testnet/mainnet. 

4. Integrate [Remix plugin manager](https://remix-ide.readthedocs.io/en/latest/layout.html#plugin-manager) to play well with IoTex IDE to benefit from all of Remix plugins. Specific functionalities that we want to highlight that this will enable: 
   * Unit testing of smart contract code. 
   * Solidity static analysis. 
   * Gas profiler. 
   * Control flow graph. 

5. Exploring/interaction with deployed contract to change contract storage state.
    * An output panel that shows deployed contract state. 
    * User can then trigger calls to deployed contract to change contract state. 


6. Add templates.  
    * Templates: 
        * This will act as quick start guide for users to load some generic templates to start onboarding. 
        * Examples can include simple DApps. 
        * User will be able to see a list of all templates and then load that template into the IDE. 


7. Add storing/sharing scripts functionalities: 
    * Inspired by [ETHFiddle](https://ethfiddle.com/), users will be able to: 
        * store/retrieve their work from local storage. 
        * share links with friends/colleagues for debugging sessions. 





## Development Roadmap

Tentative Start: July 1, 2020

### Milestone 1: Init

* Software functionality that the community can expect after completion of this milestone: 
    * Working IDE with the following features: 
        * Add functionality to connect online IDE to local filesystem by integrating [remixd](https://remix-ide.readthedocs.io/en/latest/remixd.html)
        * Add suitable and contextual error messages. 
        * Support for Solidity 0.6.0
        * Deploying contract: 
        * Fixing bugs if any with other injected providers like IoPay. 
        * Use iotex-antenna for deploying bytecode to testnet/mainnet. 

* People Involved: 
    * Lead Developer. 
    * Backend Developer
    * Project Manager. 

* Milestone details: 
    * Total time required in execution: 6 weeks
        * 4 weeks execution. 
        * 2 weeks Q/A. 
    * Completion ETA: August 11th
    * Funding Required: $15,720


### Milestone 2: Finishing off 

* Software functionality that the community can expect after completion of this milestone: 
    * Working IDE with the following features: 
        * Integrate Remix Plugin Manager. 
            * Test + bugfixing to ensure existing plugins work.  
        * Output panel that shows deployed contract state. 
            * User can then trigger calls to deployed contract to change contract state. 
     * Templates: 
        * Create scaffolding structure for templates that include solc version the template works in. 
            * This scaffolding structure will enable the community to make PR's to Github repo and add templates easily  
        * Building functionality to load templates into IDE. 

    * Add storing/sharing scripts functionalities: 
        * store/retrieve their work from local storage. 
        * share links with friends/colleagues for debugging sessions. 



* People Involved: 
    * Lead Developer. 
    * Backend Developer
    * Project Manager. 

* Milestone details: 
    * Total time required in execution: 6 weeks
        * 4 weeks execution. 
        * 2 weeks Q/A. 
    * Completion ETA: September 23
    * Duration: 6 weeks. 
    * Funding Required: $15,720


## Total Budget Requested


 | Milestone | Budget |
 |-----|---------:|
 | 1 | $15,720 | 
 | 2 | $15,720 | 
 |**Total**| $31,440 |


## Maintenance and Upgrade Plans

### Maintenance: 
1. After project completion, maintaining and iterating on user feedback on the system actively for the next 1  month. Bug fixes, if any.
2. For next 3 months: support if the system goes down.

### Upgrade Plans: 

We are inspired by the following projects: 
1. [Cryptoverse Wars](https://cryptocodeschool.in/tezos) - an interactive code school to onboard newcomers to the [Tezos](https://tezos.com/) ecosystem. 
    * This project is built by our team. 
3. [Flow Playground](https://play.onflow.org/) - IDE to onboard newcomers to the [Flow](https://www.onflow.org/) ecosystem. 


We want to use the IDE created in this proposal as a core building block for an interactive code school that onboards potential smart contract developers to the IoTeX community. The idea would be to provide an immersive experience that triggers newcomers thought process of the potential applications they can build on IoTeX. 



# Team

## Contact Info

Email: bhaskar@buidllabs.io


## Team Members

- Lead Dev: Bhaskar 
- Backend Dev: Sahil
- Project Manager: Prastut

## Team Member LinkedIn Profiles

* Bhaskar: https://www.linkedin.com/in/bhaskar-singh-55a535b9/
* Sahil: https://www.linkedin.com/in/sahil-nanda-8b1b88143
* Prastut: https://www.linkedin.com/in/prastut/


## Team Website
https://buidllabs.io/

## Relevant Experience

Our team comprises of people having background in building ed-tech startups and developer adoption tools for the blockchain space. We are currently heads down in building key projects and infrastructure tools that help protocols of tomorrow solve the problem of user adoption. 


Brief info about the team members:


- IoTeX Researcher + Lead Dev: Bhaskar Singh
  - Led development for [Cryptoverse Wars](https://cryptocodeschool.in/tezos).
  - Previously built and shelved 2 startups. Led frontend for them.
  - [GitHub.](https://github.com/bhaskarSingh)


- Backend Developer: Sahil

  - Lead dev for [YieldScan](https://github.com/buidl-labs/yieldscan-backend-ts)
  -  Previously programmed algorithmic trading strategies for a crypto hedge fund.
  - [GitHub](https://github.com/sahilnanda1995)

- Project Manager: Prastut
    - Currently spending mindspace in observing and understanding incentives for participation for core actors involved in upcoming projects that use PoS. Eager to deep dive into IoTeX in detail during the project.
    - Have 5+ years of product-dev experience across multiple startups, research labs and companies.
    - [Github](https://github.com/prastut)

## Team code repositories

Similar projects: 
1. [Cryptoverse Wars](https://github.com/buidl-labs/crypto-code-school-inside-tezos) - an interactive code school to onboard newcomers to the [Tezos](https://tezos.com/) ecosystem. 


You can check out our [Github profile](https://github.com/buidl-labs) as well for info on all of our projects that we have built/and building in the blockchain space. 
