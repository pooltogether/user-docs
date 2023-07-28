---
description: This guide explains how to withdraw from the PoolTogether V4 Smart Contracts.
---

# Withdrawing from V4

To withdraw directly from the SmartContract navigate to the block explorer respective to the chain that you have your PoolTogether deposit on.

### **Step 1:**&#x20;

Use one of the links below to find the PoolTogether Smart Contract:

* [Ethereum (Etherscan)](https://etherscan.io/address/0xd89a09084555a7D0ABe7B111b1f78DFEdDd638Be#writeContract)
* [Optimism (Optimistic Etherscan)](https://optimistic.etherscan.io/address/0x79Bc8bD53244bC8a9C8c27509a2d573650A83373#writeContract)
* [Polygon (Polygonscan)](https://polygonscan.com/address/0x19DE635fb3678D8B8154E37d8C9Cdf182Fe84E60#writeContract)
* [Avalanche (Snowtrace)](https://snowtrace.io/address/0xF830F5Cb2422d555EC34178E27094a816c8F95EC#writeContract)

### **Step 2**:&#x20;

Make sure you are on the Contract tab and select Write Contract. Connect your wallet.

### **Step 3:**&#x20;

Scroll to `18. withdrawFrom`.

* Input your address into the **`_from`** field
* Input the amount you want to withdraw in the **`_amount`** field
* Click `Write`

{% hint style="info" %}
**Note**:\
USDC has 6 decimals, so you have to add 6 0's at the end of the amount. Example: To withdraw 10 USDC, input 10000000 into the \_amount field.
{% endhint %}

