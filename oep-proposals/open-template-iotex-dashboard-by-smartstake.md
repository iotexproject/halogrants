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

- Performance Dashboard - Delegate performance dashboard allows assessment of performance of each delegate in near real-time (1 epoch, 8 epochs), short term (1 day, 7 days), long term (21 days) windows. The tooling will allow individual coin holders to assess the performance of the delegates they stake with or want to stake with. These tools are also useful for monitoring of the delegate health by delegates, by IoTeX, and by community. Features included are:
  - Delegate list - listing of all delegates status, uptime, rewards, past returns, past returns index (a relative performance index), expected returns, expected returns index. Allows marking delegates as favorite for easy access.
    -	Returns Index –  is a ratio of the returns (past/expected) of a delegate as compared to the average returns of all delegates in a given time window. A ratio of 1 means that a delegate is performing (or expected to perform) at an average level. A value <1 means worse than average and a value >1 means better than average. This allows relative assessment of all delegates based on the past or expected returns.
    - Visual indicators on delegate list and details screens for delegate performance and returns
  - Delegate details screens - shows basic delegate details and includes epoch and daily performance data presented using visual charts and tables
  - Voter list screen per delegate with vote amount and basic rewards details
  - Breakdown/details for the expected returns and expected returns index - The idea is to show details for transparency and building understanding of the inner workings of the rewards system for the community
  - Basic Telegram Bot - Build a telegram bot with basic summary of all validators, favorite validators. The details provided will include key data made available in the web application.

## Development Roadmap

Most of the features outlined in this document depend on a mature set of APIs exposed by the blockchain itself. The milestones outlined here can be met only if the foundational data can be obtained using IoTeX defined APIs in IoTeX Core or using REST/RPC/etc. kind of methods.
Smart Stake will commit to delivering all features within 6 weeks of the start date. If a feature cannot be built because of lack of availability of appropriate API, an alternative/equivalent effort feature will be built after discussing with IoTeX representative.

Milestones:
- Performance Dashboard
  - All features mentioned in deliverables
  - Implementation date - within 6 weeks after start
  - Funding - 1.2 million IOTX


## Total Budget Requested

1.2 million IOTX

## Maintenance and Upgrade Plans

- Blockchain/data sync up processes will be monitored for timely execution
- Security fixes, bug fixes, & performance improvements will be performed as needed
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
