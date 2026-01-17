---
title: Governance v0 User Guide
description: User guide for the governance system.
icon: landmark
---

This guide will explain how to participate in the Orca Governance program v0, hosted through the Solana Program Library web portal known as Realms.

A realm is a Solana program launched by any DAO to support its governance through proposals and voting.

*Note that Orca may or may not adopt Realms for the next iteration of the Orca Governance program; Orca is using Realms for Governance v0 to prototype and gather feedback!*

**Realms for Orca Governance v0** can be accessed here:https://governance.orca.so/

**Forum to discuss proposals for Orca Governance v0** ca be accessed here https://forums.orca.so/

#### Deposit Tokens

To participate in governance activity, such as voting or submitting proposals, all tokenholders must first deposit their ORCA to the program to claim voting power. Only when ORCA has been deposited to the holder’s unique governance account will the voting power be acknowledged.


The deposit button can be found in the “Your Account” section of the DAO page. Clicking “Deposit” will initiate a transaction tosend ORCA to a new Governance account in the tokenholder’s control.


Once deposited, the Account window will reflect the voting power under “ORCA Votes”:

#### Submit a Proposal

Prior to submitting an on**-** chain proposal through the Governance UI, the proposer must post a detailed outlined on the Forum page using the template guideline. This will allow the community to provide feedback and discuss the proposal prior to any on-chain voting. If the proposal receives positive feedback from the community, it may be moved to on-chain voting.

100,000 ORCA or more deposited in the program will be required to submit a Governance Proposal. If a user has the required ORCA amount, the Proposal creation button will be enable on the Proposals page:


This "New" button will take the user to a dedicated Proposal creation page with specific fields to fill out, including Title, Description, and Instructions.

In the Description field, the proposer is expected to following the following format:

* Summary (one or two sentence explanation)
* Description (longer in depth description of proposal)
* Specification (explanation of how proposal will be carried out)
* Motivation (outline of benefits to the community)


By default, the instructions are set to “Offchain Instructions”. In v0, it is expected that all proposals will be “Offchain Instructions” unless they are Governance Upgrade requirements.

For “Governance”, the user should always chose the first option: “J9uWvULFL47gtCPvgR3oN7W357iehn5WF2Vn9MJvcSxz”


Once filled out, the user can hit Add Proposal to complete the process through a transaction:


#### Voting on a Proposal

All proposals will be visible in the front page of the application under “Proposals.” This will include Proposals in states: Voting, Succeeded, Defeated, Completed and Executed. A filtering function is available to help narrow down the selection.

A tokenholder can click any proposal to see more details and participate in Voting. Once in a Proposal page, a proposal in Voting state will display the breakdown of votes, approval quorum, and the user’s voting power.

To submit a vote, follow the “Cast your community vote” section in a proposal page:


Once selected, a comment can be included on top of the vote which will be displayed in the Comments section of the proposal for all other tokenholders to read. The action can be confirmed with a transaction.

#### Voting Period

During the voting period, all funds used to vote in any proposals are locked in the governance program until the voting period has been completed. The time remaining is displayed in the proposal page:


Once completed, the proposal will move to either Succeeded or Defeated state based on the approval quorum having been met or not. In either case, the tokenholder is now able to release their tokens from the voting lock. This release token button can be found in the previous Voting section of the proposal page:


This will also trigger a transaction to be signed.

**Note:** Releasing tokens does not remove the tokens from Governance, it only unlocks the token from proposal involvement which in turn allows for Withdrawing.

In the event that a voter needs access to their tokens immediately or wishes to relinquish their vote for whatever reason, this can be accomplished by submitting a transaction under “Withdraw your vote”:


The vote will no longer be counted towards the proposal, and the tokens will be unlocked from the proposal and enabled for Governance withdrawal.

#### Withdrawing Governance Tokens

Assuming no tokens are locked in a live Voting period or in a Completed proposal that needs releasing, the tokenholder can withdraw their voting power to return the underlying ORCA to their wallet. This can be done in the same Deposit section by choosing Withdraw:


#### Executing Proposals

If a proposal passes, the specification outlined in the proposal will be executed by the Orca team to the best of their ability. Later on, it will be possible to make proposals that include code that will executed on-chain.

#### Admin Token

The admin token is a special token minted specifically for use in the Orca Governance program. Currently, only one Admin token has been minted and the mint authority is controlled by the Governance program. This means any additional tokens will need to be minted through a Proposal.

This token has the ability to create Proposals outside of standard ORCA voting requirements, allowing it to pass proposals alone.

The token is held by a member of the Orca team as a last resort failsafe measure to protect the Governance Program from any technical or malicious failures with the program. The token will only be used in the event of disaster recovery needs.

### FAQ

* **Will the on-chain governance system stay live after the first (or first few) proposals?**

  + We’ll decide depending on the community’s response and the learnings received from this trial. Eventually, Orca may choose to build a custom own governance portal that inherits Orca’s human-centered DNA.

* **How was the threshold for proposals determined?**

  + Participating in governance takes time and energy, so Orca strives to ensure that any effort invested is spent on well-thought-out proposals. This threshold ensures that proposals come with the support of a reasonable % of token holders.