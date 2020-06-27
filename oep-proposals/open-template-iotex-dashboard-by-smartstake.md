# Open Grant Proposal: `IoTeX Dashboard by Smart Stake`

**Name of Project:**

**Proposal Category:** Infrastructure

**Proposer:** SmartStake

**Do you agree to open source all work you do on behalf of this RFP?:** No

# Project Description

Smart Stake, a staking validator, based on its experience, is looking to build tools to support the IoTeX ecosystem and provide user friendly features to assess network health, delegates’ performance, and voter related features.

The current tools in IoTeX ecosystem do not provide adequate tools to understand delegate performance or voter rewards in various time-frames. Smart Stake dashboard will introduce new performance metrics and build multiple visual charts to assess the performance of delegates in short to long term time frames. Performance metrics will allow absolute and relative performance assessment of delegates. Historical data for all aspects will be readily available to everyone.

## Value

Smart Stake dashboards make it very easy to understand delegate performance and reward returns. The toolset will allow ease in interpreting complex underlying process that affect performance. Based on the unique aspects of every blockchain project, there are several aspects that remain beyond the comprehension of large proportion of community members. Given Smart Stake's experience in developing similar tools previously, we are very confident of getting it right. The risk that can affect delivery of all features is not having an API that is necessary for obtaining/capture certain required data.

## Deliverables

- Module - Delegate Performance - Delegate performance module allows assessment of performance of each delegate in near real-time (1 epoch, 8 epochs), short term (1 day, 7 days), long term (21 days) windows. The tooling will allow individual coin holders to assess the performance of the delegates they stake with or want to stake with. These tools are also useful for monitoring of the delegate health by delegates, by IoTeX, and by community
  - Delegate list - listing of all delegates status, uptime, rewards, expected returns, expected returns index (a relative performance index). Allows marking delegates as favorite for easy access.
  - Delegate details screens - shows basic delegate details and includes epoch and daily performance data presented using visual charts and tables
  -	Provide summary stats for blocks, rewards earned by delegates per epoch/day. Provide historical views for all performance stats and relevant delegate details. Stake history for delegate – chart showing how the staking history has changed for delegate over time since launch
  -	Delegate events – tabular view of all events related to a given delegate e.g. new votes, un-stake, fee changes, rewards claim and the amounts involved. Unlike a typical transaction explorer, the key difference here will be use of delegate names to improve readability
  -	Notification on delegate home pages or delegate list screen for fee changes or degraded performance
  - Delegate voter list screen with basic rewards details
  -	Build a telegram bot with: Performance summary of all delegates. Performance/health details of favorite delegates
- Module – Coin Holder Tools - The following features will be assessed and implemented to provide various views for coin holders to assess how their staked coins are growing or have grown or are expected to grow in future.
  - Rewards — provide outstanding undistributed rewards for IoTeX addresses.
    - Provide anonymous access to individual rewards across devices without requiring users to re-enter their address on each use.
    - Provide breakdown by individual delegates used.
    - Support multiple addresses within one view.
    - Show just-in-time comparison of returns from each delegate
    - Show rewards/address details with current BTC/USD value
  -	Rewards history — historical listing of all rewards for given set of addresses.
    - Summarizes rewards at monthly/annual levels.
    - Provide breakdown by individual delegate.
    - Includes chart reflecting state of rewards at the end of each day (more like end-of-day rewards balance history)
  -	Overall Address details - show breakdown of an address by showing coins staked with individual delegates.
    - Show coins held that are not staked.
    - Show rewards/address details with current BTC/USD value
  -	Address stake history – visual chart showing address stake history
  -	Address events – tabular view of all events related to a given address e.g. voting, un-staking, rewards claim and the amounts involved. Unlike a typical transaction explorer, the key difference here will be use of delegate names to improve readability
  -	Rewards Calculator – Rewards calculator with calculations based on given delegates and their fee structure
  -	Add address and address rewards feature in the telegram bot
- Module – Network Stats - Smart Stake will develop the following features related to IoTeX network stats:
  -	Overall network stats – screen summarizing various high level stats for the network e.g. circulating supply, total supply, coins staked, %age staked, current mcap, current stake’s $/BTC value, overall expected return based on current staked amount and annual rewards
  -	Overall network richlist with named account – allows visual/simplified monitoring of whale accounts/exchanges
  -	Block production rate for network at epoch level
  -	Stake history for network – Chart showing how the staking history is progressing over time
  -	Overall rich list (staking n non-staking combined) - rank all active addresses with a non-zero balance based on coins held (including staked). Show 100, 1000 or all addresses. Allow search within loaded results

## Development Roadmap

Most of the features outlined in this document depend on a mature set of APIs exposed by the blockchain itself. The milestones outlined here can be met only if the foundational data can be obtained using IoTeX defined APIs in IoTeX Core or using REST/RPC/etc. kind of methods.
Smart Stake will commit to delivering 80%+ of the features within 8 weeks of entering the contract. It is assumed that up to 20% of the features mentioned above may be not relevant enough or not doable if appropriate/reliable API is not available. For every such feature, Smart Stake will work with IoTeX representative to build a comparable effort feature in the given timeline.

Milestones:
- Module - Delegate Performance
  - Scope - 80% of original features mentioned in Deliverables section for this module. Up to 20% replacement features depending upon specific needs of IoTeX blockchain.
  - Implementation date - 4 weeks after contract start
  - Funding - TBD
- Module – Coin Holder Tools -
  - Scope - 80% of original features mentioned in Deliverables section for this module. Up to 20% replacement features depending upon specific needs of IoTeX blockchain.
  - Implementation date - 7 weeks after contract start
  - Funding - TBD
- Module – Network Stats -
  - Scope - 80% of original features mentioned in Deliverables section for this module. Up to 20% replacement features depending upon specific needs of IoTeX blockchain.
  - Implementation date - 10 weeks after contract start
  - Funding - TBD

## Total Budget Requested

TBD

## Maintenance and Upgrade Plans

- New features will be added as the blockchain evolves and as the community needs change
- Blockchain/data sync up processes will be monitored for timely execution
- Security fixes, bug fixes, & performance improvements will be done as needed
- Library/dependency upgrades will be assessed/performed twice a year

# Team

## Team Members

- BigB

## Team Member LinkedIn Profiles

- N/A

## Team Website

https://www.smartstake.io

## Relevant Experience

Smart Stake builds easy to understand and user centric tools for all the network participants. The tools are geared towards stakers and delegates. We introduce new performance metrics to simplify assessment of a pool’s performance and rate of returns. We have already built a full featured dashboard for AION at https://tools.AionSmartStake.com. We have also built 3 other dashboards at https://harmony.smartstake.io, https://oasis.smartstake.io, and https://cs.smartstake.io.

BigB, the operator of Smart Stake has 20+ years of IT experience as a developer/architect in large scale enterprise implementations.

## Team code repositories

https://github.com/SmartStake

# Additional Information

Thanks for giving the opportunity to present this proposal. Feel free to reach out to us at https://t.me/bigb4ever if you have any questions.
