# Open Grant Proposal: `IoT Data Provenance`

**Name of Project:** DoTeX

**Proposal Category:** Open ended proposal

**Proposer:** `asgahier76`

**Do you agree to open source all work you do on behalf of this RFP?:** To be determined

# Project Description

IoT networks bring value by integrating data from different sources, which can be problematic due to network heterogeneity and dynamic nature. Questioning how to authenticate the sources of the data raises the concern of IoT network vulnerability and the possibility of manipulating and inserting inauthentic records along the data path. This problem can be addressed using the techniques of data provenance and verifiable claims.
Data provenance allows a verifying party to check datasets’ authenticity to the origin.
That can enable tracking the dataset throughout the data path from the source where it is gathered through all the processing pipeline and thus offer the capability to identify any
inauthentic data handling. Moreover, open data models are becomingvmainstream for distributing IoT datasets, which requires a mechanism that can provevdata derivatives authenticity, and ownership.

## Solution

The proposal suggests a new concept that builds a trusted data chain where datasets generated and processed are stamped using the actor DID signature and presented as verifiable credentials traced to its origin.

In describing the proposed concept, a smart vehicular network is used. It is assumed that the vehicles are equipped with a set of sensors that collect information for use by internal subsystems or external entities in vehicle-to-vehicle (V2V) or vehicle-to-infrastructure (V2X) data exchanges.

Building a verifiable vehicular network data path combines a set of components that include first the vehicular network elements (which in general can be any IoT and sensor network) and the components responsible for maintaining data provenance (which will be the IoTeX blockchain and the iotex did method).

## Verifiable DID/VC Data Paths

In this proposalm DIDs and VCs are the cornerstones for establishing secure and provenant data chains. To achieve global provenance, each sensor with processing capability is assigned a unique DID at manufacturing, and each processing unit, including the vehicle itself, is also assigned a DID. DIDs are also assigned to infrastructure elements in case of V2X data exchange, and to complete the path also entities and processing engines (a data pre-processing or ML algorithm) should be assigned their respective DIDs,

Generating a verifiable data path is achieved through a series of steps that create a verifiable claim (VC) for each data record or set of records. Deciding on the number of records that
share a VC depends on the data record size and frequency of data generation. Each VC has a size of a few hundred bytes, thus adding a VC for each data record might constitute
a significant overhead. The generation of a VC for a set of data records utilizes DIDs, Blockchain, and cryptography functions represented by hashing and digital signature.

## Verifying Claims

On the consuming side, once a dataset is obtained by an entity, the origin and authenticity of the data are verified by first hashing the dataset and verifying it against the latest
VC. For a transformed dataset, multiple VCs exist, and the process requires verifying the signature of the proof of each VC against the DID of the corresponding actor.
To ensure that the data throughout the path has not been manipulated, a VC shall contain a link to the previously issued VC represented by the transaction hash. Thus,
by verifying all the transactions, it ensures that the trail of transformation is authentic.
So, each VC ensures that the action performed is actually performed by the same actor according to the DID, while the chain of transactions hashes confirm that the path is intact.

## Linked Data Proofs

The proposed concept will utilize the iotex did method and by generating VC to build a provenance trace and a data chain that enables linking the verifiable claims issued for the data set and its derivatives. The suggested approach allows the extraction of the provenance trace by linking the data proofs using the hash of the previous VC. Upon querying the blockchain for a specific VC hash, the returned object contains the previous VC id, which is a URL to access the VC. Repeatedly, the verifier pulls the dataset using the id record in the credentialsSubject field hash it and verifies it against the VC proof.
The process continues until reaching the original dataset for which the corresponding VC record on-chain has a null value for the URL, indicating it is the genesis VC.
Since certain datasets may propagate through different actors while remaining the same, building a trace of data provenance requires the capability to authenticate the integrity
and ownership of the dataset with a compact representation. A VC representation, in this case, can include instead of the proof field a proof chain field. A proof chain is useful to
allow validating a data set that has been signed by multiple entities while the order of proofs generation is important

## Deliverables

The main deliverable is to build a system that uses the iotex did method and blockchain to deliver the above mentioned concept.
The system will have the capability to issue dids based on iotex did method and enable generating and verifying iot data provenance records.

## Development Roadmap

* Analysing the IoTeX method
  * Building the acquintance ot the iotex did method
  * Define the integration aaproach

* Build backend system
  * A backend system that integarates the iotex did method
  * Provide all APIs endpoints for the suggested functionalities

* Build a frontend
  * Building a dashboard to show how to integrate the APIs in a use case

## Total Budget

Total Budget for the project is 9,000,000 IOTX

Analysis Phase - 250K IOTX
First Phase: Build Backedn System -5M IOTX
Second Phase: Build Frontend and Use Case - 3M IOTX
Testing and Documentation - 400K IOTX
Build DevOps Tools - 350K IOTX


## Maintenance and Upgrade Plans

- A detailed explanation of the proposed concept will be defined.
- Use open source tools for DevOps to enable easy deployement and upgrade of the system. 

# Team

## Team Members

- Ahmad Sghaier Omar

## Team Member LinkedIn Profiles

https://www.linkedin.com/in/ahmad-sghaier-2619a645/

## Team Member Experience

- Ahmad Sghaier Omar: 
Ahmad is an expereiced Blockchain developer with over 4 years of experiece in the domain. He built many Blockchain tools, including LibraMask a browser exgension for the Libra Blockchain, KinConnect a browser extension for the KIN Blockchain, MOBEOS a mobile app toolkit for the EOS Blockchain. Ahmad has also developed smart contracts based on ERC20 and ERC721 tokens and mobile wallets that integrate with major cryotcurrency exchanges (e.g., Gemini). He also wroked on building chaincode on Hyperledger Fabric for Financial Markets products. Ahmad initally comes from Telecom and IT background with over 14 years of experince in technoligy and management positions, he moved into the domain of IoT and Blockchain when he started his PhD studies at the University of Waterloo, Canada. Ahmad has his phd in building IoT-related smart contracts for IoT device Idenity management and Authentication and Authorization in addition to the introduction of W3C DID and Verifiable Credentials for IoT.

## Team Github Repos and Projects

- LibraMask, a browser extension for Libra Blokchain, https://github.com/upright-vc/libraMask (https://www.youtube.com/watch?v=Xu03cpyLgA8)
- KinConnect (This plugin is not yet an open source, so this is a link to a video showing KinConnect in action) (https://www.youtube.com/watch?v=JpQn616v8wI)
- MOBEOS, a mobile toolkit for EOS Blockchain, https://github.com/Takafuly/mobeos
- 0xO a browser plugin that integrates both Torus social login and 0x Instant to enable users to buy ERC20 tokens easily and send ETH and ERC20 tokens to other users using only their email address. https://github.com/asghaier76/0xo, https://www.youtube.com/watch?v=gW6uhEgsdCg

