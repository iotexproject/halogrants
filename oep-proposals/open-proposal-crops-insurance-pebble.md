# Open Grant Proposal: `Weather Insurance in Agriculture`

**Name of Project:** Weather Insurance in Agriculture

**Proposal Category:** Trusted Data

**Proposer:** [Firefox_IT](https://t.me/Firefox_IT)

**Do you agree to open source all work you do on behalf of this RFP?:** Yes

# Project Description

Every year, farmers insure their crops from bad weather: as I own fields of organic wine grapes and olive oil in Sicily, I myself subscribe to an insurance policy every year to protect against damages due to hail and frost. Most of the time, the final evaluation of the event is left to the word of the insurance company: although the evaluation should rely upon visual references of the damage, they are often missing, leaving claims to be driven by the experience of the consultant that is sent by the insurer to investigate. 

The idea is to build a proof of concept using **Pebble Tracker**, that would leverage verifiable IoT data provided by the device installed in my field to feed an insurance smart contract deployed on the IoTeX blockchain, that would eventually pay the farmer if conditions are met according to the terms of his insurance policy, and based on the trusted data received by Pebble. This concept could become the starting point for many other use cases both in insurance and other fields.

## Value

The iotex project is laying the foundations for exciting and innovative applications of the blockchain and verifiable data for the IoT. Yet as all frontier technologies, the creation of prototypes is necessary to verify the real "usability" of the technology for the users, especially when it involves **interaction with the real world**.

The process of clearing insurance premiums in agriculture today suffers from a huge **trust gap** as it is not only expensive but **not objective** and subject to **frauds**. 

This propotype will demonstrate how the use of Pebble Tracker devices can really lead to the solution of this type of problems, in a **win-win** fashion for all the parties involved. Specifically, it will show:

- How Pebble Tracker can be easily installed in a real use case
- The "flow" of the verifiable data from Pebble -> Backend server -> Smart contract
- How the verification of the insured event in the real world will trigger a payment on the IoTeX Blockchain
- [ Optional ] Professional video-documentation of the installation and "event simulation"


## Deliverables

We will deliver a fully working PoC that implements an example of a simple (yet effective) architecture where a **Pebble Tracker is installed** and **operated** nearby a Olive Trees, and will transmit verifiable data through an IoT backend to the IoTeX blockchain, contract where an **Insurance Contract** will manage the payment in the case of a specific "Bad weather event". While the concept of "Verifiable IoT Data" is easily expandable to any type of sensor, in this prototype we only include the "Frost" event using the temperature and humidity sensor integrated on Pebble tracker.

## Development Roadmap

Please break up your development work into a clear set of milestones. This section needs to be detailed.

```
Milestones          | Details                         | Manpower            | Duration   | Funding (IOTX)  |
___________________________________________________________________________________________________________
1.Projecty design   | - Idea and concept details doc  | 1x (project leader) | 2 weeks     | 200k IOTX.     |
                    | - Technical/Functionals docs    | 1x (Developer)      |             |                |
                    | - Smart contract design and     |                     |             |                |
                    |   functional model.             |                     |             |                |
                    |                                 |                     |             |                |
2.Development       | - Developement of the smart     | 1x (Developer)      |             |                |
                    |   contract                      |                     | 12 weeks    | 300k IOTX      |
                    | - Development of the data relay |                     |             |                |
                    | - Installation of the pebble    |                     |             |                |
                    |   backend                       |                     |             |                |                    
                    | - Tests.                        |                     |             |                |
                    |                                 |                     |             |                |
3.Installation      | - Design and realization of a   | 1x (project leader) | 8 weeks     | 300k IOTX      |
                    |   suitable whaterproof case     | 1x (Developer)      |             |                |
                    | - Arrangement and connection to |                     |             |                |
                    |   the power supply.             |                     |             |                |
                    | - Integration with the backend  |                     |             |                |
                    |                                 |                     |             |                |
4.Simulation & Main | - End-to-End integration        | 1x (project leader) |12 weeks     | 200k IOTX      |
tenance             | - Creation of insurance contract| 1x (Developer)      |             |                |
                    | - Real world event simulation   |                     |             |                |
                    | - Monitoring and ensuring opera |                     |             |                |
                    |   tion along the period with    |                     |             |                |
                    |   Backend visualizaion public   |                     |             |                |
                    |   access                        |                     |             |                |
                    |                                 |                     |             |                |
5.Optional          | - Professional video making of  | Third-party company |             | 200k IOTX      |
                    |   installation and event simul. |                     |             |                |

```
## Total Budget Requested

Total budget requested: 
 - 1,000,000 IOTX (100% of the fund will be spent on human resource)
 - Optional 200,000 IOTX for third-party marketing service.

## Maintenance and Upgrade Plans

According to previous Milestone 4.	

# Team

## Team Members

1. "Firefox_IT" (Project leader) 
2. "HologramX" (Developer)

## Team Website

N/A

## Relevant Experience

**Firefox_IT**
I am dental surgeon, Owner of Family Farm and also a Crypto Enthusiast. I’ve been a client of this type of insurance for 20 years. I know the parameters and algorithms on which they are based for the calculations, IOT Maker. 

**TheHologramX**
Computer Science Teacher at High School, Programmer Various Languages, IT_Admin, NET_Admin, Security_Admin, Crypto Enthusiast, IOT Maker and Programmer, Solidity developer


## Team code repositories
N/A

# Additional Information
N/A
