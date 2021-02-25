---
kip: KIP-1
title: KEYFI Token Allocation on Binance Smart Chain
status: Passed
author: Ben Gervais (@altninja)
discussions-to: KeyFi Discord Server Channel: #proposal-forum 
created: 2021-02-19
---

<!--You can leave these HTML comments in your merged KIP and delete the visible duplicate text guides, they will not appear and may be helpful to refer to if you edit it again. This is the suggested template for new KIPs. Note that an KIP number will be assigned by an editor. When opening a pull request to submit your KIP, please use an abbreviated title in the filename, `kip-draft_title_abbrev.md`. The title should be 44 characters or less.-->

## Simple Summary
<!--"If you can't explain it simply, you don't understand it well enough." Simply describe the outcome the proposed changes intends to achieve. This should be non-technical and accessible to a casual community member.-->
In order to expand the KeyFi platform a greater number of users, we are proposing to allocate 1m KEYFI tokens into the Binance Smart Chain ecosystem including a staking and rewards contract.

## Abstract
<!--A short (~200 word) description of the proposed change, the abstract should clearly describe the proposed change. This is what *will* be done if the KIP is implemented, not *why* it should be done or *how* it will be done. If the KIP proposes deploying a new contract, write, "we propose to deploy a new contract that will do x".-->
If the proposal passes, we will either stake or burn (depending on the result of the vote) 1m KEYFI tokens, taken from the 8m KEYFI community rewards pool and use this to mint 1m KEYFI tokens using BEP20 standard.  Afer minting the new tokens, we propose to allocate 800,000 KEYFI tokens for community rewards and 200,000 treasury and development fund.

## Motivation
<!--This is the problem statement. This is the *why* of the KIP. It should clearly explain *why* the current state of the protocol is inadequate.  It is critical that you explain *why* the change is needed, if the KIP proposes changing how something is calculated, you must address *why* the current calculation is innaccurate or wrong. This is not the place to describe how the KIP will address the issue!-->
Gas prices on Ethereum are leaving many users unable to participate.  Deploying the KEYFI token as a BEP20 token on Binance Smart Chain will this help us reach a larger user base and reduce transaction costs for users, allowing more users the ability to access other KEYFI related smart contract deployments. 

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
We will implement the following: 
* A BEP20 Token Contract for KEYFI.  
* Either Burn or Stake 1m KEYFI on Ethereum (TBD in a proposal if this one is passed.  
* * Deploy a KEYFI Rewards contract for Liquidity Providers and other staking rewards and allocate 800,000 KEYFI for community reewards.  
* * Allocate 200,000 KEYFI for KeyFi treasury and development fund.  

### Rationale
<!--This is where you explain the reasoning behind how you propose to solve the problem. Why did you propose to implement the change in this way, what were the considerations and trade-offs. The rationale fleshes out what motivated the design and why particular design decisions were made. It should describe alternate designs that were considered and related work. The rationale may also provide evidence of consensus within the community, and should discuss important objections or concerns raised during discussion.-->
We want to allow users who cannot afford the high transaction fees on Ethereum as well as take advantage of any specific innovations possible on BSC platform.  This can be done with a low risk 2-way bridge, or by a simple burn and mint process.  

### Technical Specification
<!--The technical specification should outline the public API of the changes proposed. That is, changes to any of the interfaces KeyFi Finance currently exposes or the creations of new ones.-->
As BSC is compatible with Solidity smart contracts, there will only be minor technial changes from the current Ethereum deployment.  

### Test Cases
<!--Test cases for an implementation are mandatory for KIPs but can be included with the implementation..-->
All deployments will be tested on testnet prior to mainnet deployment.

### Configurable Values
<!--Add any variables here that could have an effect on the proposals implementation-->


## Copyright
Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0/).
