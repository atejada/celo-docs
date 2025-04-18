---
title: Celo Locked CELO Rewards
description: How to earn locked CELO rewards and adjust the rate for voting participation, target schedule, and deductions.
---

# Locked CELO Rewards

How to earn locked CELO rewards and adjust the rate for voting participation, target schedule, and deductions.

:::warning
As of block height 31,056,500 (March 26, 2025, 3:00 AM UTC), Celo is no longer a standalone Layer 1 blockchain—it is now an Ethereum Layer 2!
Some documentation may be outdated as updates are in progress. If you encounter issues, please [file a bug report](https://github.com/celo-org/docs/issues/new/choose).

For the most up-to-date information, refer to our [Celo L2 documentation](https://docs.celo.org/cel2).
:::

---

## Introduction to Locked CELO Rewards

Holders of Locked CELO that voted in the previous epoch for a group that elected one or more validators and have activated their votes are eligible for rewards. Rewards are added directly to the Locked CELO voting for that group, and re-applied as votes for that same group, so future rewards are compounded without the account holder needing to take any action. The voting process is described further [here](/what-is-celo/about-celo-l1/protocol/pos/epoch-rewards-locked-gold).

:::tip

Rewards to Locked CELO are totally independent from validator and validator group rewards, and are not subject to the **group share**.

:::

![](https://storage.googleapis.com/celo-website/docs/locked-gold-rewards.jpg)

## Adjusting the Reward Rate for Voting Participation

The protocol has a target for the proportion of circulating CELO that is locked and used for voting. An on-target reward rate is determined and then adjusted at every epoch to increase or reduce the attractiveness of locking up additional supply. This aims to balance having sufficient liquidity for CELO, while making it more challenging to buy enough CELO to meaningfully influence the outcome of a validator election.

The reward rate is adjusted as follows:

![](https://storage.googleapis.com/celo-website/docs/voting_reward_rate_adjustment_equation.png)

where $$rr$$ is the reward rate or voting yield, $$vf$$ is the voting fraction calculated as locked CELO for voting divided by circulating CELO supply, and $$af$$ is the adjustment factor. If the voting participation is below the target at the end of an epoch, the on-target reward rate is increased; if the voting participation is above the target at the end of an epoch, the reward is decreased.

## Adjusting the Reward Rate for Target Schedule and Deductions

Adjusting the on-target reward rate to account for under- or over-spending against the target schedule gives a baseline reward, essentially the percentage increase for a unit of Locked CELO voting for a group eligible for rewards.

The reward for activated Locked CELO voting for a given group is determined as follows. First, if the group elected no validators in the current epoch, rewards are zero. Otherwise, the baseline reward rate factors in two deductions. It is multiplied by the slashing penalty for the group, and by the average epoch uptime score for validators in the group elected in the current epoch. Finally, the group's activated pool of Locked CELO is increased by this rate.
