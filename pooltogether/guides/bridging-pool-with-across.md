---
description: >-
  The POOL token exists on multiple chains. Across allows to bridge POOL between
  Ethereum and L2s.
---

# Bridging POOL with Across

_This guide explains how to use Across, a third-party cross-chain bridge for L2s and rollups secured by UMA's optimistic oracle._&#x20;

### **Step 1: Enter bridge details**

Head to [across.to/bridge](https://across.to/bridge) and connect your wallet on the top right corner. Enter the bridge details accordingly.&#x20;

The different fields explained:

* **Send**: Select the POOL token and enter the amount of tokens you want to transfer
* **From**: Select the chain you want to send your tokens from
* **To**: Select the destination chain

<figure><img src="https://lh5.googleusercontent.com/AxRoQyUxnI5kKoJ-xayeDw30O7GQ9kuLe7Ed3vlwdWedb8dOYihKlFQwPndAYBWqbnx8TJPenZhVY-BRTCfven6uRysAW7f3hJx-L5f63hsT58UwXsLUgwoMKB_2Yg6_eR0IqCXuYRXdKJAKG2VLU6w" alt=""><figcaption><p>Enter bridge details</p></figcaption></figure>

### **Step 2: Approve the contract**

Before bridging you need to allow the smart contract to access your POOL tokens. Click the approve button and verify the transaction in your wallet.

<figure><img src="https://lh4.googleusercontent.com/LGYO9hRLXF101YlpJiAJVVal_JY7jC6lPWlZcgTp-nacV7oqQ5CkA5rpVbBvXIAALrxUME5-tGBCgJ9F9Eh8xYI9EBxdpVv_bYSB-q4LMq3WyVBAf55GifMMgHFfEdrCuxSU5sureQUO5KXTtYOs-tc" alt=""><figcaption><p>Approve the contract</p></figcaption></figure>

### **Step 3: Confirm the transaction**

This step will send your tokens to the bridge’s smart contract. After verifying that all data you entered is correct (amount, tokens, source-, and destination chain) you can click the send button. Confirm the transaction in your wallet and your assets are on the way!

<figure><img src="https://lh6.googleusercontent.com/KwSAkiJbFBrQoHOu88lvQnxVp_-ZmMMtDOoqjjGFQTwn3u--LUrPLNEPypJBtrQzraxw2RksD0f_cjzaCDFMNgBEqfCX8tXACRdtRxFYv3o3xvWWJqtHnVCitBYorMwdVRCLSPb-kpghD11QLvsAxAQ" alt=""><figcaption><p>Confirm the transaction</p></figcaption></figure>

### **Step 4: Wait for the receipt**

After the transaction has been confirmed in your wallet your POOL tokens should arrive on the destination chain shortly.&#x20;

You can review the details of the transaction on the confirmation page and monitor its progress on the [transaction page](https://across.to/transactions).&#x20;

<figure><img src="https://lh6.googleusercontent.com/eTiRSM9CD4BuZRLQuMA3_ye59wi8U2gsdMwMBIoxluLTvGq0M2n4WreOniwrK1JdtQT-CBOiceVW9eXXLHsBOt4s_geOnoybKTJ1OlluKdrkIXq0aHVu7_AwCTAG_jVzPDPyjXlEFNxvpWDXnFDzM_E" alt=""><figcaption><p>Wait for the receipt</p></figcaption></figure>

## **Fees**

In addition to the transaction fee for sending your tokens to the bridge the Across protocol charges two fees:

<details>

<summary><strong>Destination Gas Fee</strong></summary>

To deliver the tokens to the user on the destination chain, the Across protocol submits a transaction on behalf of the user. The destination gas fee covers the gas costs associated with this transaction on the destination chain.

</details>

<details>

<summary>Bridge Fee</summary>

In order to send their tokens instantly across networks, users pay a small [bridge fee](https://docs.across.to/how-across-works/fees) to incentivize relayers and liquidity providers.&#x20;

Relayers give out short-term token loans to Users in exchange for fees. This is to incentivize them to promptly relay a transaction. Relayers fulfil deposit requests by sending the depositor their desired token on their requested destination chain.&#x20;

Liquidity Providers provide the capital that enables relayers to have flexibility about where they want to take a refund in exchange for fees. Their capital is also available to fulfil deposits in the case that no relayers can fast-fill a deposit.

As a user, you don’t have to care about all of that! Because of this incentive design, you’re able to quickly bridge your tokens while the relayers take on the risk for you.&#x20;

</details>

## Additional Resources

* [How Across works](https://docs.across.to/how-across-works/overview)
* Learn more about Fees in the [Across Documentation](https://docs.across.to/how-across-works/fees)
* Learn more about Bridges & Bridge Risk in the [Ethereum documentation](https://ethereum.org/en/developers/docs/bridges/)
