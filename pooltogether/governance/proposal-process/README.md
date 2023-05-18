# Proposal Process

## Overview

The community of POOL holders makes decisions through governance proposals. Proposals are accepted or rejected using an onchain voting process. Anyone, who holds or has delegated >10,000 POOL, can submit a proposal to PoolTogether governance.

All proposals should be submitted as one of the valid [proposal types](./#proposal-types) stated below and follow the outlined proposal process:

1. [Request for Comments \[RFC\]](./#1.-forum-post)
2. [PTIP / PTBR](./#2.-community-feedback)
3. [Onchain Proposal](./#4.-on-chain-proposal)
   * [Voting](./#voting)
   * [Implementation](./#implementation)
   * [Defeated Proposals](./#what-if-a-proposal-is-defeated)

### Recommended timeline

The following timeline is recommended and should be considered when creating a proposal.

* RFC: 5 days (_minimum_)
* PTIP/PTBR: 24 hours (_minimum_)
* Submit onchain: 5 days (_does not vary_)

_Note: This timeline can vary based on community approval._

### 1. Request for Comments \[RFC]

All major discussions should start on the governance forum to be reviewed by anyone in the PoolTogether community.&#x20;

* Submitted as a new [forum discussion](https://gov.pooltogether.com/) in the appropriate category.
  * New topics auto-populate with the corresponding proposal template
* Marked as Request for Comments by adding `[RFC]` to the title.
* Follow the forum title format as stated for the [proposal type](notion://www.notion.so/o/-M58QKDDuY724c-sqMF4/s/-MjVmQloS14HsmiACMUz-887967055/\~/changes/131/pooltogether/governance/proposal-process#proposal-types).

Once submitted, the forum discussion should be open for feedback from the community for at least **5 days** (assuming it is well-formed).

* If the proposal does not get explicit approval or is still highly contested, the proposer should -continue to seek feedback from the community and submit an amended proposal.
* If the proposal has strong support, the proposer can create a corresponding PTIP/TBR.

### 2. PTIP / PTBR

After applying potential community feedback to the proposal, the proposer should:

* create a new [forum discussion](https://gov.pooltogether.com/) in the [appropriate category](https://www.notion.so/626fb3991e824960a541fa6928c23420)
* flag the RFC-thread to be locked
* state the changes made to the initial RFC

and leave the topic open for at least **24 hours**, before submitting the proposal onchain and creating the corresponding Snapshot.

### 3. Onchain Proposal

When it comes time to create an onchain proposal, the proposer must:

1. Create a new [onchain proposal](https://vote.pooltogether.com/), matching the specification outlined in the forum post
2. Create a corresponding [POOL Pool Snapshot](https://snapshot.page/#/poolpool.pooltogether.eth) vote for the proposal
3. Update the forum post with links to the onchain proposal and snapshot vote

The details of the PoolTogether Governance system are described [here](../voting-and-delegation-101.md).

<details>

<summary>What is the POOL Pool Snapshot for?</summary>

The POOL Pool Snapshot allows POOL pool ticket holders to participate in proposal voting.&#x20;

This pool’s voting power is delegated to a multi-sig whose signers are community members. When there is an onchain proposal there must be a corresponding vote in the POOL Pool Snapshot. The multi-sig must vote according to the result of the POOL Pool Snapshot. [Learn more](../ppool-gasless-voting.md).

</details>

### Voting

After a proposal is submitted onchain a **5-day voting period** begins. A proposal succeeds, if after five days

* the majority of votes are in favor (approval threshold of 51%)
* **AND** at least 100,000 votes have been cast in favor (Quorum of 1%).

### Implementation

When a proposal succeeds, the proposer (or any other person) can queue Proposal.

There is a two day timelock before the proposal is actually implemented. After the timelock has expired, the proposal can be executed.

<details>

<summary>What if a proposal is defeated?</summary>

In case a proposal does not pass a governance vote, the proposal will not be executed. If the proposer wishes to iterate on a proposal that has been rejected, they should:

1. Create a new proposal thread on the Forum.
2. Include a link to the first proposal that did not pass.
3. Clearly identify what has changed in the new proposal.

</details>

### Footnotes

* If a proposer does not hold their votes throughout the full time of the onchain proposal, then the proposal can be canceled by anyone.
* Urgent, security-related PTIPs may progress to an onchain proposal immediately.

## Proposal Types

<table><thead><tr><th>Proposal Type </th><th>Forum Title Format</th><th>Description</th><th>Quorum</th><th>Approval Threshold</th><th data-hidden></th></tr></thead><tbody><tr><td><strong>PTIP</strong> <br>PoolTogether Improvement Proposal</td><td>PTIP-&#x3C;Id>: <br><em>eg. PTIP-89:</em></td><td>Process for changing the protocol </td><td>1% (100,000 POOL)</td><td>51%</td><td></td></tr><tr><td><strong>PTBR</strong> <br><a href="pt-budget-requests.md">PoolTogether Budget Request</a></td><td>PTBR-X: Project/Team Name</td><td>Process for coordinating treasury funds</td><td>1% (100,000 POOL)</td><td>51%</td><td></td></tr></tbody></table>

## **Acknowledgements**

The PTIP process is a modified version of [Badger Improvement Proposals](https://forum.badger.finance/t/about-the-bip-badger-improvement-proposals-category/20) and [Yearn Improvement Proposals](https://github.com/yearn/YIPS/blob/master/yip-X.md).
