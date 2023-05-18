---
description: The spending card for crypto natives
---

# PoolTogether Debit Card FAQ

<figure><img src="../../.gitbook/assets/gateway.ipfscdn.png" alt=""><figcaption></figcaption></figure>

### What is the PoolTogether Card?

The PoolTogether Card is a Debit Card powered by Juno. It allows you to spend your PoolTogether balance on everyday things.

### How does it work?

There are two ways to use the PoolTogether Debit Card. You can choose to use either a Push or the Pull Method.

<details>

<summary>Top-Up (Push Method)</summary>

Whenever a user tops up their card, their USDC is liquidated to USD and deposited into an FDIC-insured checking account to ensure the safety of their funds.&#x20;

Example: A user will convert PTaUSDC to USDC (say $500 at a time) and then spend that USDC when they make purchases.&#x20;

On a technical level:

* User cashes out their crypto from their Web3 Wallet to a FDIC-insured Checking Account
*   The Debit Card (MasterCard) that is linked to the Checking Account is used for spending on everyday items.&#x20;



</details>

<details>

<summary>Direct Spending (Pull Method)</summary>

With direct spending, PTaUSDC is withdrawn (pulled) from the Web3 wallet directly at point of sale.

On a technical level:

* User approves their PTaUSDC to be spent by the contract.&#x20;
* The withdrawFromPool() function is called, and it withdraws from the pool:&#x20;
  * Function burns PTaUSDC and withdraws USDC to the user's wallet.&#x20;
* User approves their USDC to be spent by the contract.&#x20;
* The function performTradeForSpecificAmount() is called, which deposits the USDC into the contract.&#x20;
* The USDC is auto-converted into the checking account

</details>

### Where can I use my card?

The PoolTogether Debit Card is accepted by over 40m merchants worldwide. It’s a Mastercard.

### Are there any country restrictions?

The Pilot will launch in the US with plans to expand to other countries in the coming months.

### Does Juno custody the deposits?&#x20;

No, you can spend your PoolTogether balance directly from a self-custody wallet of your choice.

{% hint style="info" %}
There is a daily transaction limit of $10,000.
{% endhint %}

### How does it relate to my wallet and my key?

In order to use this service you have to undergo a KYC process with Juno. We suggest creating a dedicated wallet to use for this service.

Reminder: Never share your private key with anyone.&#x20;

### What about fees? Withdrawing has fees.&#x20;

PTaUSDC to USDC to USD is always 1:1. You only pay the network (gas) fees for the withdrawal.&#x20;

### What chain/s are we talking about?

Spending works with deposits on Optimism, Polygon & Ethereum.

### Will there be rewards?

Yes, users will receive \<redacted> in addition to \<redacted> by spending with their PoolTogether card.

### How can I get access?

You can reserve your personal handle and save your spot on the waitlist for the PoolTogether Debit Card by Juno [here](https://juno.finance/pooltogether).

## Any open Questions?

Visit the [Juno Helpcenter](https://help.juno.finance/en/) or [join the PoolTogether community on Discord](https://pooltogether.com/discord).
