---
description: >-
  We encourage responsible disclosure of any smart contract vulnerabilities and
  will pay up to $22,727 for those.
---

# Bug Bounties

Generation Software Inc. collaborates with Immunefi on a public bug bounty program to incentivize vulnerability disclosures by anyone. Please adhere to the PoolTogether bug bounty program overview on Immunefi to learn all about the rules and details for the bug bounty, including assets and impacts in scope, out-of-scope activities, limitations, etc.

{% embed url="https://immunefi.com/bug-bounty/pooltogether/" %}

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
