---
description: This guide explains how to withdraw from the PoolTogether V2 Smart Contracts.
---

# Withdrawing from V2

### **Step 1**:&#x20;

Navigate to the [Prize Pool contract on Etherscan](https://etherscan.io/address/0x29fe7d60ddf151e5b52e5fab4f1325da6b2bd958#writeProxyContract).

### **Step 2**:&#x20;

Make sure you are on the contract tab and you are writing as Proxy. Click "Connect to Web3".

<figure><img src="../../../.gitbook/assets/image (18).png" alt=""><figcaption></figcaption></figure>

### **Step 3**:&#x20;

Scroll down to 37 `withdrawCommittedDeposit`

<figure><img src="../../../.gitbook/assets/image (19).png" alt=""><figcaption></figcaption></figure>

The \_amount field requires you to enter the amount formatted as uint256. DAI has 18 decimals.

{% hint style="info" %}
Example: \
To withdraw 10 DAI, the uint256 number is `10000000000000000000`
{% endhint %}

### Step 4:

Click on Write and sign the transaction in your wallet. Done!
