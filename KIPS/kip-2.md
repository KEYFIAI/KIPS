---
kip: KIP-2
title: KEYFI Staking Deposit Fee Management
status: Pending
author: Ben Gervais (@altninja)
discussions-to: KeyFi Discord Server Channel: #proposal-forum 
created: 2021-08-07
---

<!--You can leave these HTML comments in your merged KIP and delete the visible duplicate text guides, they will not appear and may be helpful to refer to if you edit it again. This is the suggested template for new KIPs. Note that an KIP number will be assigned by an editor. When opening a pull request to submit your KIP, please use an abbreviated title in the filename, `kip-draft_title_abbrev.md`. The title should be 44 characters or less.-->

## Simple Summary
<!--"If you can't explain it simply, you don't understand it well enough." Simply describe the outcome the proposed changes intends to achieve. This should be non-technical and accessible to a casual community member.-->
In order to being implementation of the long term token economic model, we are proposing to manage the current deposit fees collect from the v2 staking contracts according to the methods described in this post: [KEYFI Token Economic Model 1/3](https://medium.com/keyfi-news/keyfi-staking-and-reward-pools-keyfi-token-economic-model-updates-part-1-3-f936020843b).

## Abstract
<!--A short (~200 word) description of the proposed change, the abstract should clearly describe the proposed change. This is what *will* be done if the KIP is implemented, not *why* it should be done or *how* it will be done. If the KIP proposes deploying a new contract, write, "we propose to deploy a new contract that will do x".-->
If the proposal passes, we will follow the methods defined in the specifications including the burning of KEYFI tokens.

## Motivation
<!--This is the problem statement. This is the *why* of the KIP. It should clearly explain *why* the current state of the protocol is inadequate.  It is critical that you explain *why* the change is needed, if the KIP proposes changing how something is calculated, you must address *why* the current calculation is innaccurate or wrong. This is not the place to describe how the KIP will address the issue!-->
The management of deposit fees will create a self-funding and self-sustaining mechanism for ongoing rewards. This will ensure that the foundations are in place for long-term community growth, and a fair allocation of the resources.  This will for the time being be implemented as a manual & community governed process.  If it is successful, the processes will be programmed into future v3 staking and kTokens smart contracts.

## Specification
<!--The specification should describe the syntax and semantics of any new feature, there are five sections
1. Overview
2. Rationale
3. Technical Specification
4. Test Cases
5. Configurable Values
-->

### Overview
<!--This is a high level overview of *how* the KIP will solve the problem. The overview should clearly describe how the new feature will be implemented.-->
The proposed actions for each deposit fee are below:

For KEYFI
* 50% KEYFI Burned
* 50% KEYFI sent to seed fund for new DEX LP pools

For KEYFI LP Tokena
* 50% Sell the non-KEYFI token for KEYFI then all KEYFI is Burned
* 50% Sell the non-KEYFI then send to seed fund for new DEX LP pools

For Network Native Token (ETH/BNB/MATIC etc.)
* 50% Send to Gas Fund (Contract Deployments / KeyFiDAO Transactions / Testing Integrations etc.)
* 50% Send to KeyFi Treasury / Dev Pool

For Non-KEYFI Token with Existing Pool
* 50% Buy KEYFI and send it to the Reward Pool
* 50% Send to KeyFi Treasury / Dev Pool

For Non-KEYFI Token without Pool
* 50% Send to seed fund for new DEX LP pools
* 50% Send to KeyFi Treasury / Dev Pool 

### Rationale
<!--This is where you explain the reasoning behind how you propose to solve the problem. Why did you propose to implement the change in this way, what were the considerations and trade-offs. The rationale fleshes out what motivated the design and why particular design decisions were made. It should describe alternate designs that were considered and related work. The rationale may also provide evidence of consensus within the community, and should discuss important objections or concerns raised during discussion.-->
The proposal will create a long-term, deflationary, self-sustaining model for ongoing incentivization of KeyFi smart contract usage. The deposit fees which are burned will reduce the overall supply of KEYFI, while the other management processes will help the reward pool and prepare for a new DEX liquidity pool.

### Technical Specification
<!--The technical specification should outline the public API of the changes proposed. That is, changes to any of the interfaces KeyFi Finance currently exposes or the creations of new ones.-->
Within 48 hours of a successful vote result, the team will manually execute the transactions required to follow the processes outlined above, including both the Ethereum and BSC deposit fee wallets, .   

### Test Cases
<!--Test cases for an implementation are mandatory for KIPs but can be included with the implementation..-->
There are no test cases for this proposal.

### Configurable Values
<!--Add any variables here that could have an effect on the proposals implementation-->
The values will follow what is defined in the specifications.

## Copyright
Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0/).
