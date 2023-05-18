---
description: >-
  The Deposit Delegator is a powerful tool to enable others to win prizes on
  your behalf!
---

# Deposit Delegator

### Delegation

Delegation means you're giving another wallet additional chances to win prizes without losing custody of the underlying deposit. You share your odds with others but keep the funds.

Example: If I deposit $1,000 USDC, I can then "delegate" my deposit to any other wallet address. The wallet I delegate to will be able to check and claim prizes even if that wallet has no deposit.

### Deposit Delegator

[The Deposit Delegator](https://tools.pooltogether.com/delegate) is a feature that allows to easily delegate portions of a PoolTogether deposit (_in the form of PTaUSDC tickets_) to multiple wallets (_Delegatees_). This increases the Delegatees chance of winning prizes by the delegated amount.

A Delegator can delegate to an unlimited amount of different wallets with individual amounts each.

![](<../../.gitbook/assets/image (9).png>)

<details>

<summary>Use Cases: Why delegate?</summary>

* Protocols can deposit treasury funds and delegate to their users or token-holders
* Delegate to anyone holding a certain NFT or POAP
* Delegate to any wallet that does a certain onchain action in the last week (i.e. makes a trade on uniswap)
* Delegate to friends and family to effectively onboard them to DeFi
* Delegate to winners of your raffle
* Delegate to your contributors of the month
* Delegate to people who have never used crypto and hold no tokens but have a wallet address!

</details>

### Roles

There are three roles within the Deposit Delegator feature:

<details>

<summary><strong>Delegators</strong></summary>

Delegators are accounts (_wallets_) that delegate their chance to win to other wallets.

</details>

<details>

<summary><strong>Delegatees</strong></summary>

Delegatees are those who have tickets delegated to them. The Delegatee’s odds to win a prize increase, but they don't have access to the underlying funds.

</details>

<details>

<summary><strong>Representatives</strong></summary>

Delegators can appoint representatives to manage delegations on their behalf. Representatives can create and update the delegations, but cannot withdraw any funds. A representative can be an individual person or a smart contract. If you want to set a Representative you can [follow the instructions below](deposit-delegator.md#undefined).

</details>

## Using the Deposit Delegator

To use the Deposit Delegator you have deposit [into PoolTogether first](https://app.pooltogether.com/).&#x20;

1\) Open the [Deposit Delegator UI](https://tools.pooltogether.com/delegate) and click on `+ New Delegation` to create the (first) delegation.

![](<../../.gitbook/assets/Kopie von Community Schedule (1281 × 721 px).png>)

2\) A pop up to create a delegation will open. Enter the details as explained click on `Queue Creation`. The delegation will be queued, meaning you can batch multiple delegations into on transaction to save on gas.

![Disclaimer: If a lock duration is entered the Delegatee cannot be changed, and the funds cannot be withdrawn until the lock has expired.](<../../.gitbook/assets/Deposit Delegator 2 (1).png>)

3\) You can now either:

* Click on `Save Changes` to finish the delegation, or
* add another delegation and repeat the previous process.

![](<../../.gitbook/assets/Deposit Delegator 3.png>)

4\) Clicking on `Save Changes` will open a pop up to review & confirm your delegation(s). Once you sign the transaction in your wallet and confirm the contract interaction you are done. The delegation is live!

![](<../../.gitbook/assets/Deposit Delegator 4 (2).png>)

### Editing Delegations

Each delegation is handled by a so-called “delegation slot”. Each delegation slot corresponds to a smart contract on the blockchain. This contract holds the tickets and delegates the chance of the held tickets to the Delegatee.

Instead of creating a new delegation slot every time, you can re-use existing slots by editing them. Only delegations without active time lock can be edited.

1\) To edit existing delegation slots click on `edit` on the bottom right and choose a delegation you want to update, by clicking on its 📝 icon.

![](<../../.gitbook/assets/Deposit Delegator 5.png>)

2\) The process of editing is the same as [creating a delegation](deposit-delegator.md#using-the-deposit-delegator). You can change the Delegatee (delegation receiver), the delegated amount and have the option to add a time lock.

3\) The updated delegations are queued until you click on `save changes` and confirm them with an onchain transaction.

### Withdrawing Delegations

Multiple delegations can be withdrawn in batches.  Withdrawing from a delegation slot will add the tickets back to the balance of the Delegator.

1\) In the Deposit Delegator click on `Withdraw`.

2\) You can now choose which delegations you want to withdraw by checking the boxes in front of the Delegatee address. Once you selected all the delegation slots click on `Withdraw` to confirm.

![](<../../.gitbook/assets/Deposit Delegator 6.png>)

3\) A pop up opens to review your withdrawals. Click on Confirm updates and confirm the onchain transaction in your wallet.&#x20;

![](<../../.gitbook/assets/Deposit Delegator 7.png>)

After withdrawing, the delegation slots remain with a balance of 0. You can re-use them for future delegations to other Delegatees by [editing them as explained above](deposit-delegator.md#editing-delegations).&#x20;

### Bulk Delegations

Bulk Delegation allows delegating to many addresses at once by uploading a CSV with delegations. No more manually editing all your delegations.&#x20;

You can access Bulk Delegations within the Deposit Delegator or by following [this link](https://tools.pooltogether.com/delegate/bulk).

![](<../../.gitbook/assets/image (17).png>)

1. Download a [template CSV](https://tools.pooltogether.com/bulk-delegation-template.csv).
2. Edit the template.\
   **Delegatee** is the address to delegate to.\
   **Lock duration** is the amount of time (in seconds) until the delegator or representative can revoke the delegation. Set this value to 0 for no lock duration.\
   **Amount** is the amount of the token to delegate.
3. Upload the CSV.
4. Submit delegation transaction(s).

Uploading a new CSV will overwrite all current onchain delegations.

Bulk Delegation may require multiple transactions. If they are not confirmed in your wallet in the proper order some transactions may fail.

_This feature is in beta and may run slow when delegating to hundreds of addresses._

### Setting Representatives&#x20;

By setting an account representative you are able to appoint a manager for your delegations. Account representatives can edit your delegation positions while you maintain full custody of your deposit. That means they can create and update the delegations, but cannot withdraw any funds.

You can set or remove Representatives within the Deposit Delegator.

<div align="left">

<img src="../../.gitbook/assets/image (7).png" alt="">

 

<img src="../../.gitbook/assets/image (16).png" alt="">

</div>

## Delegation FAQ

<details>

<summary>How do I delete a Delegation?</summary>

You don't. This tool is representing the state of the contracts, so the delegations you make will persist onchain forever, even with a balance of 0.

If you want to delegate to a new address, you can edit that old one rather than click "New Delegation" to save gas.

</details>

<details>

<summary>Can I edit a locked delegation?</summary>

If a lock duration was entered the Delegatee cannot be changed, nor funding withdrawn until the lock has expired. The transaction will revert if the delegation is still locked.&#x20;

</details>

<details>

<summary>Can the Deposit Delegator be used with a Multi-Sig?</summary>

Yes, the Deposit Delegator supports multi-sigs.&#x20;

</details>

<details>

<summary>Do the prizes need to be claimed?</summary>

Yes, they do. Prizes can be claimed by the delegatees [here](https://app.pooltogether.com/prizes).

You can also claim prizes on behalf of other accounts via Smart Contract. The claimed prizes are added to the Delegatee's PTaUSDC balance and will remain in their wallet, even if you take the delegation back.

</details>

<details>

<summary>Are delegations transitive? I.e. if A delegates to B, and C delegates to A, does B receive the delegation from C?</summary>

No, Delegations can’t be delegated. Users can only delegate their own balance.

</details>

<details>

<summary>Where can I find the technical documentation?</summary>

[Follow this link](https://dev.pooltogether.com/protocol/contracts/v4-twab-delegator/).

</details>
