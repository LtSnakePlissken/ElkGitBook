---
description: >-
  Elk's innovative cross-chain architecture is built around a system of token
  “reservoirs” that are deployed on each supported chain.
---

# Cross-chain Reservoirs

Each reservoir holds in reserve the total supply of ELK tokens (\~42 million) minus the circulating supply on the corresponding chain. The ElkNet controls and coordinates movements of ELK tokens into and out of these reservoirs. For cross-chain transfers, ELK tokens enter the reservoirs on the origin chain,  which prompts  ElkNet to send a message to the reservoir on the destination chain to release ELK into the user’s wallet.

The reservoir system has multiple design and security advantages over the two prevailing methods for cross-chain bridging: **burn-and-mint** and **lock-and-release**. Let’s take a look at how ElkNet stands apart:

![ElkNet v2 vs. other cross-chain bridges](<../.gitbook/assets/image (5).png>)

ElkNet's reservoirs increase transparency, eliminate custodial risk, and reduce smart contract vulnerabilities all at once.

They reduce overhead by delegating multiple smart contract interactions to the generic messaging layer. By pre-minting the total supply of ELK on each chain, we’ve removed the risk of minting exploits, which are one of the primary ways that bridge security fails. Since there are no bridge tokens locked on either end, individual users are not trusting a custodial bridge operator to secure their funds.
