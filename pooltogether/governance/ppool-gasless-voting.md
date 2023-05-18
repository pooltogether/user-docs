---
description: The POOL pool on Ethereum is a setup for gasless voting.
---

# pPOOL Gasless Voting

The POOL Pool Snapshot allows POOL pool token holders to participate in proposal voting without paying gas fees.

To vote gaslessly, you can deposit POOL tokens in the POOL pool on the [account tab in the PoolTogether app](https://app.pooltogether.com/account). You will receive pPOOL tokens which are eligible to vote [here](https://snapshot.org/#/poolpool.pooltogether.eth).

### How does it work?

The POOL pool’s voting power is delegated to a multi-sig whose signers are community members. The multi-sig votes according to the result of the POOL Pool Snapshot.

It works like this:

* All POOL that is held in the POOL pool (pPOOL) automatically delegates its voting power to a multi-sig.
* Whenever a PTIP is posted onchain, there is a corresponding vote in the [POOL pool Snapshot](https://snapshot.org/#/poolpool.pooltogether.eth).
* pPOOL depositors can vote on the snapshot without paying for gas.
* If the Snapshot reaches Quorum (20% of all pPOOL have voted), the multi-sig submits the outcome to the onchain vote.

{% hint style="info" %}
Due to technical limitations, the multi-sig must always vote with its full voting power.\
\
Example: If 20% of circulating pPOOL votes _for_ on a proposal, the full 100% of pPOOL votes will _for_.
{% endhint %}
