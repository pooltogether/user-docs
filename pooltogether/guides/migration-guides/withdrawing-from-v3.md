---
description: This guide explains how to withdraw from the PoolTogether V3 Smart Contracts.
---

# Withdrawing from V3

### **Step 1**:&#x20;

Find the Pool you are deposited to and browse to its contract on the block explorer of its respective network.

#### Ethereum

<table data-header-hidden><thead><tr><th width="199.00000000000003"></th><th></th></tr></thead><tbody><tr><td>DAI Prize Pool</td><td><a href="https://etherscan.io/address/0xEBfb47A7ad0FD6e57323C8A42B2E5A6a4F68fc1a">https://etherscan.io/address/0xEBfb47A7ad0FD6e57323C8A42B2E5A6a4F68fc1a</a></td></tr><tr><td>USDC Prize Pool</td><td><a href="https://etherscan.io/address/0xde9ec95d7708b8319ccca4b8bc92c0a3b70bf416">https://etherscan.io/address/0xde9ec95d7708b8319ccca4b8bc92c0a3b70bf416</a></td></tr><tr><td>UNI Prize Pool</td><td><a href="https://etherscan.io/address/0x0650d780292142835F6ac58dd8E2a336e87b4393">https://etherscan.io/address/0x0650d780292142835F6ac58dd8E2a336e87b4393</a></td></tr><tr><td>COMP Prize Pool</td><td><a href="https://etherscan.io/address/0xBC82221e131c082336cf698F0cA3EBd18aFd4ce7">https://etherscan.io/address/0xBC82221e131c082336cf698F0cA3EBd18aFd4ce7</a></td></tr><tr><td>GUSD Prize Pool</td><td><a href="https://etherscan.io/address/0x65C8827229FbD63f9de9FDfd400C9D264066A336">https://etherscan.io/address/0x65C8827229FbD63f9de9FDfd400C9D264066A336</a></td></tr><tr><td>POOL Prize Pool</td><td><a href="https://etherscan.io/address/0x396b4489da692788e327e2e4b2b0459a5ef26791">https://etherscan.io/address/0x396b4489da692788e327e2e4b2b0459a5ef26791</a></td></tr><tr><td>Aave USDT Prize Pool</td><td><a href="https://etherscan.io/address/0xc7d56c06F136EFff93e349C7BF8cc46bBF5D902c">https://etherscan.io/address/0xc7d56c06F136EFff93e349C7BF8cc46bBF5D902c</a></td></tr><tr><td>Sushi Prize Pool</td><td><a href="https://etherscan.io/address/0xc32a0f9dfe2d93e8a60ba0200e033a59aec91559">https://etherscan.io/address/0xc32a0f9dfe2d93e8a60ba0200e033a59aec91559</a></td></tr><tr><td>USDT Prize Pool</td><td><a href="https://etherscan.io/address/0x481f1BA81f7C01400831DfF18215961C3530D118">https://etherscan.io/address/0x481f1BA81f7C01400831DfF18215961C3530D118</a></td></tr><tr><td>Uniswap POOL LP Prize Pool</td><td><a href="https://etherscan.io/address/0x3AF7072D29Adde20FC7e173a7CB9e45307d2FB0A">https://etherscan.io/address/0x3AF7072D29Adde20FC7e173a7CB9e45307d2FB0A</a></td></tr></tbody></table>

#### Celo

<table data-header-hidden><thead><tr><th width="224"></th><th></th></tr></thead><tbody><tr><td>cUSD Prize Pool</td><td><a href="https://explorer.celo.org/address/0x6F634F531ED0043B94527F68EC7861B4B1Ab110d">https://explorer.celo.org/address/0x6F634F531ED0043B94527F68EC7861B4B1Ab110d</a></td></tr><tr><td>cEUR Prize Pool</td><td><a href="https://explorer.celo.org/address/0xbe55435BdA8f0A2A20D2Ce98cC21B0AF5bfB7c83">https://explorer.celo.org/address/0xbe55435BdA8f0A2A20D2Ce98cC21B0AF5bfB7c83</a></td></tr></tbody></table>

#### Polygon

<table data-header-hidden><thead><tr><th width="226"></th><th></th></tr></thead><tbody><tr><td>USDC Prize Pool</td><td><a href="https://polygonscan.com/address/0xEE06AbE9e2Af61cabcb13170e01266Af2DEFa946">https://polygonscan.com/address/0xEE06AbE9e2Af61cabcb13170e01266Af2DEFa946</a></td></tr><tr><td>USDT Prize Pool</td><td><a href="https://polygonscan.com/address/0x887E17D791Dcb44BfdDa3023D26F7a04Ca9C7EF4">https://polygonscan.com/address/0x887E17D791Dcb44BfdDa3023D26F7a04Ca9C7EF4</a></td></tr></tbody></table>

If you don’t know which of the above pools you might be deposited into, you can follow the trace of the receipt token that’s in your wallet.

### **Step 2**:&#x20;

Navigate to the Contract tab, click on write contract and connect your wallet

<figure><img src="../../../.gitbook/assets/image (20).png" alt=""><figcaption></figcaption></figure>

### **Step 3**:&#x20;

Find the function `withdrawInstantlyFrom`

<figure><img src="../../../.gitbook/assets/image (21).png" alt=""><figcaption></figcaption></figure>

The parameters explained:

| Parameter Name  | Parameter Description                                                                                                                           | What to enter                                                                                                                                                                                                                                          |
| --------------- | ----------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| from            | <p>The address to withdraw from.<br>This means you can withdraw on another user's behalf if you have an allowance for the controlled token.</p> | Your wallet address                                                                                                                                                                                                                                    |
| amount          | The amount to withdraw                                                                                                                          | <p>The amount formatted as uint256. This means the amount has to include all decimals.<br><br>Eg: To withdraw 100 DAI, the amount is <code>100000000000000000000</code></p>                                                                            |
| controlledToken | The controlled token to withdraw from                                                                                                           | The address of the ticket token, eg: [PcDAI](https://etherscan.io/address/0x334cBb5858417Aee161B53Ee0D5349cCF54514CF) to withdraw the underlying DAI, [PcUSDC](https://etherscan.io/token/0xd81b1a8b1ad00baa2d6609e0bae28a38713872f7) to withdraw USDC |
| maximumExitFee  | The maximum early exit fee the caller is willing to pay.                                                                                        | Enter `0`                                                                                                                                                                                                                                              |

### **Step 4**:&#x20;

Click Write and confirm the transaction to withdraw your tokens.
