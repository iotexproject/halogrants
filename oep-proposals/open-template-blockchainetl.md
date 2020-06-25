To submit a proposal, please create a PR against this template in this repo. Please title your file `open-proposal-title.md`, replacing `title` with the name of your project.

# Open Grant Proposal: `Blockchain ETL`

**Name of Project:** IoTeX Blockchain ETL on GCP

**Proposal Category:** Infrastructure

**Proposer:** `tnlee`

**Do you agree to open source all work you do on behalf of this RFP?:** Yes

# Project Description

Blockchain technology has captured the imagination of technologists, financiers, and economists. Perhaps even more intriguing are the long-term, diverse applications of the technology. By increasing the transparency of blockchain systems, the contained data becomes more accessible and useful. With this in mind, our immediate project objective is to make the IoTeX blockchain data available for exploration with BigQuery. All historical data can be found in the IoTeX blockchain data set, which updates daily (and eventually in real-time). We hope that by making the data more transparent, users of the data can gain a deeper understanding of how IoTeX’s blockchain systems function and how they might best be used for the benefit of the ecosystem. 

The IoTeX network properties provide a basis for fundamental valuation of the network. For example, the total number of IoTeX transactions in a day indicates economic activity on-network. The other properties, such as the number of funded accounts and frequency of transactions may also be of fundamental economic importance. 

## Value

While the IoTeX blockchain provides OLTP capabilities (atomic transactions, data durability), it has very limited OLAP (analytics) capability for regularly required short time-scale reporting on specific or aggregated money flows stored in the ledger. The inability to easily build reports from the blockchain can reduce transparency and increase the difficulty of price discovery and other fundamental metrics of valuation such as the NVT Ratio.

In contrast, BigQuery has strong OLAP capabilities. We built a software system on Google Cloud that:

1. Performs a real-time extraction of data from the IoTeX blockchain ledger
2. Stores the data to BigQuery and de-normalizes it to make exploration easier
3. Derives insights from the extracted data with Data Studio

## Deliverables

Please describe in details what your final deliverable for this project will be. Include a specification of the project and what functionality the software will deliver when it is finished.

Daily loads - export and load blockchain data into BigQuery on a daily basis
Real-time ingestions - export and load blockchain data into BigQuery in real-time
GCP Marketplace listing - IoTeX public dataset to be listed on GCP Marketplace

## Development Roadmap

Please break up your development work into a clear set of milestones. This section needs to be detailed.

| Milestones | Details | Manpower | Date | Funding (IOTX) |
| --------------- | --------------- | --------------- |
| Daily loads | - IoTex schema draft - Blockchain node setup - Cloud Composer setup and Airflow jobs - BigQuery tables | 2 developers | 7/1 - 7/31 | 20,960,000 |
| GCP Marketplace listing | - Create production project - Coordinate with Google representatives to list public datasets  | 1 business liaison | 7/17 - 7/31 | 0 |
| Real-time ingestions | - Data ingestion from blockchain nodes to Pub/Sub - Dataflow jobs for moving data from Pub/Sub to BigQuery | 2 developers | 8/1 - 8/15 | 11,000,000

## Total Budget Requested

Total budget requested: 31,960,000 IOTX (100% of the fund will be spent on human resource).

## Maintenance and Upgrade Plans

The team will be adapting and leveraging systems developed in-house for this project, the mentioned system has been thoroughly tested and was running in production for over a year. Besides that, unit and integration tests will be implemented for the system components. The system is designed with minimal maintenance requirements in mind.	

# Team

## Team Members

1. Evgeny Medvedev
2. TN Lee

## Team Member LinkedIn Profiles

[https://www.linkedin.com/in/evgemedvedev/](Evgeny)
[https://www.linkedin.com/in/tnlee/](TN)

## Team Website

[https://www.helixtechnologies.xyz/](Helix Technologies)

## Relevant Experience

Evgeny is an experienced data scientist with over 10  years of software development experience. He is the creator of Blockchain ETL (over 900 stars) and his accreditation includes Google Cloud GDE, Google Professional Cloud Architect, and AWS Certified Solutions Architect. 

TN was a founding team member of Kyber Network and oversaw its business development efforts, which included partnerships with notable blockchain projects, such as MyEtherWallet, Coinbase, and CoinGecko. 

## Team code repositories

[https://github.com/blockchain-etl](Blockchain ETL)

# Additional Information

Please include any additional information that you think would be useful in helping us to evaluate your proposal.
