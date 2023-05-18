---
description: >-
  We encourage responsible disclosure of any vulnerabilities in the smart
  contracts and will pay up to $25,000 for those.
---

# Bug Bounties

We offer public security bug bounties to incentivize vulnerability disclosures by anyone. See Dework for the bounty details:

{% embed url="https://app.dework.xyz/pooltogether/pool-bounties?taskId=5502ecb8-83fc-4e05-813a-d0f33d348392" %}

## Past Bounties

### PermitAndDepositDai Contract: Unrestricted Sender

Severity: Medium / High\
Date: Thursday, October 22nd, 2020\
Reporter: Kevin Foesenek\
Payout: $20,000 USD of WETH ([transaction](https://etherscan.io/tx/0xdd9fcf07a29a376b811c775d34cef4ceddf6e720981da34ac7142a8c38e7e7a6))

**Vulnerability**\
Just prior to launch a security researcher discovered a flaw in the PermitAndDepositDai contract.  This flaw would have allowed an attacker to front-run the "deposit" transaction and take the deposited amount.  This would have affected any new deposits to the system.

**Mitigation**\
References to the contract were removed from the user interface, and a fix was immediately deployed to mainnet and published via NPM.
