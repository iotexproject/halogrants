
# Open Grant Proposal: `Machine learning on IoTeX`

**Name of Project:** Trusted end-to-end Machine Learning on IoTeX

**Proposal Category:** Dev

**Proposer:** `danielzak` from Scaleout

**Do you agree to open source all work you do on behalf of this RFP?:** Yes

# Project Description

Data is the world's most valuable asset, and machine learning is the main method to extract value from data. Most machine learning today is done by a single entity that control the entire chain from data to the end use case. There are several reasons for this, but one major reason is that companies need to trust the data that is used to train the resulting machine learning model. Wih the IoTeX platform, it is possible to challenge this concept and enable collaboration on trusted data available through the IoTeX platform.

In summary, this project aims to bring trusted machine learning to the IoTeX platform. A fully trusted end-to-end solution for trusted machine learning will be a long term effort, and the project will be done in several phases. This first phase will develop a solution to jointly train machine learning models on trusted and verifiable data from Pebble devices, and then provide a solution to serve predictions from these models on- and off chain to end users.

The long term objective of the IoTeX and Scaleout collaboration is to bring machine learning capabilities (tools and APIs) to the IoTeX platform and to enable fully trusted end-to-end machine learning pipelines.

## Scope

This first project aims to be a 3 month project which will address the following areas, aiming for TRL level 6 (technology demonstrated) according to the EU technical readiness levels.

### Introducing machine learning collaboration networks
We will enable collaboration between peers and devices that generate trusted data for training machine learning models. This will require infrastructure and tools to access the data and train the machine learning models. The developed solution will enable the creation of new demonstrators and experimentation by providing boilerplate code and examples. 

### Off-chain infrastructure to build, train, validate and service machine learning models
Machine learning is generally expensive and uses a lot of compute, storage and network resources. It is not feasible (or even wanted) to do everything on-chain, so bridges between on- and off-chain resources will be developed. These resources will be standardized and containerized. These systems will provide some level of security and will be able to mitigate some security concerns, but this phase will provide models with some safeguards from security scrutiny and abuse

### Integrate models into production systems 
With explicit and defined methods to participate in model training and access models through on-chain and off-chain methods.


## Deliverables

### Deliverable 1 - Toolkit to launch machine learning collaborative networks
* Tools to build and train machine learning models using on-chain IoTeX trusted data
* Tools to deploy and run machine learning models built on IoTeX data
* Tools to deploy and run service endpoints with access and compliance rules such as access, distribution and model inference rate-limit policies

### Deliverable 2 - Framework to integrate models in production systems
* Tools to serve machine learning models as API endpoints
* Frameworks to provide models with attached incentive mechanisms
* Services to engage with published model service registries and model providers
* Tools to govern the machine learning pipelines and machine learning alliances on the IoTeX platform

### Deliverable 3 - Air quality demonstrator
* Interface to register Pebble trackers in a model-specific machine learning alliance
* A local air quality prediction machine learning model using Pebble data
* Deployed model with API endpoints

### Limitations
* Security is an open research area and our solution will address security to the best extent possible. Learnings will be summarized in an end of phase report.
* Privacy is an open research area and our solution will do our best to implement privacy preserving mechanisms applicable and known to date. However from the project summarization there may be further work required pending new research discoveries.


## Development Roadmap

The first phase will focus on the ends of a typical machine learning pipeline - data in and predictions out. Pebble trackers and the IoTeX platform enable the use of trusted data in, and this project will develop a secure and trusted way to train, govern and access machine learning models.

The project is planned to start March 1st, 2021 and be finished by the end of May, 2021. It is scoped to be 3 man months of work.

### Milestone 1 - Foundation for model training invocation/and propagation via smart contracts
**Start/Duration**

April 1st, 1 month

**Functionality**

Access Pebble data through the IoTeX platform through a data acquisition adapter

Define a container deployment and pipeline for model training

Define a container deployment for model inference

Provide a smart contract template for model inference (direct to model)

<img src="https://github.com/danielzak/halogrants/blob/master/img/oep-scaleout-phase1-mlst1.png" width="500" height="500">

### Milestone 2 - Demonstrator for managing model inference via smart contracts
**Start/Duration**

May 1st, 3 months

**Functionality**

Defining containers and environments for model deployment and serving

Build a sidecar proxy service for model endpoints which can handle inference request events from smart contracts

Smart contract templates for model access, inference and licensing

Smart contract execution integration services for off-chain model deployment and serving

<img src="https://github.com/danielzak/halogrants/blob/master/img/oep-scaleout-phase1-mlst2.png" width="500" height="500">

# Team

## Contact Info

This project is led by Scaleout [contact@scaleoutsystems.com](mailto:contact@scaleoutsystems.com) 

## Team Members

* Morgan Ekmefjord (CTO, co-founder of Scaleout)
* Daniel Zakrisson (CEO, co-founder of Scaleout)
* Jens Frid (COO, co-founder of Scaleout)
* Salman Toor (co-founder of Scaleout, Associate Professor in distributed computing at Uppsala University)

## Team Member LinkedIn Profiles

* [Morgan Ekmefjord](https://www.linkedin.com/in/morganekmefjord/) 
* [Daniel Zakrisson](https://www.linkedin.com/in/danielzakrisson/) 
* [Jens Frid](https://www.linkedin.com/in/jensfrid/) 
* [Salman Toor](https://www.linkedin.com/in/salman-toor-1104b84/) 

## Team Website

[www.scaleoutsystems.com](https://scaleoutsystems.com/)

## Relevant Experience

Scaleout is a team of data scientists, machine learning engineers, software engineers, and entrepreneurs. Experienced from both industry and academic research in AI, cloud and fog computing, and scientific computing from top-ranked Uppsala University in Sweden.

Areas of expertise include AI and machine learning, cloud-native computing, data science & engineering, scientific computing & HPC. Collectively the team has authored 100+ peer-reviewed articles in AI/ML, scientific computing, and systems biology.

We’ve worked with some of the largest and most reputable organizations in the world, including AstraZeneca, SAAB Defence Systems, Swedish National Space Agency, Autodesk, Raysearch Laboratories, GE Healthcare, Swedish National Infrastructure for Computing (SNIC).

Scaleout is pioneering federated learning to overcome the data-sharing challenge, building collective intelligence from distributed data at scale, while preserving data privacy and security. Our open source solution FEDn enables federated machine learning, data partnerships, and joint machine learning ventures. FEDn is built for creating commercial machine learning alliances where data owners can build strong machine learning models together.

## Team code repositories

* [FEDn](https://github.com/scaleoutsystems/fedn) framework for federated learning
* [STACKn](https://github.com/scaleoutsystems/stackn) framework for distributed cloud MLOps

# Additional Information

* [AICHAIN](https://www.aichain-h2020.eu/) EU-project for blockchain supported federated learning in the aerospace industry
* A platform for privacy-preserving machine learning using federated learning and blockchain ([Vinnova funded](https://www.vinnova.se/en/p/a-platform-for-privacy-preserving-machine-learning-using-the-ethereum-blockchain-and-smart-contracts/))
* Academic research on distributed storage (IPFS) performance with federated learning (in pre-print)
* Collaboration and incentive design work for federated learning (e.g. [this presentation](https://www.youtube.com/watch?v=uSG2T2d3hiQ) from the Federated Learning Conference in 2020)
