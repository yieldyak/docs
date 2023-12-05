---
description: >-
  Reinvests are incentivised so that you never have to worry about compounding
  yourself.
---

# 🔁 The Reinvest Button

## Do I need to press the reinvest button?

No. Someone else will press it for you to earn the reward.

## How does it work?

The reinvest button takes all pending rewards from a pool, converts them into the farm asset, and reinvests them back into the pool to compound deposits for everyone in the farm.

There is a variable reward to incentivise users to press that button. Whoever is first to press the button, earns the reward and compounds everyone's deposits.

## When should I press it?

The reinvest button is optional. You do not need to press it. However, you might be motivated to press it to earn the reward.

If your goal is to net gain in AVAX or ETH, then you need to consider the reward token / AVAX price ratio, transaction cost for reinvesting for that particular pool, the transaction cost for swapping the reward token into AVAX, etc.

You do not need to participate in the pool to be able to receive the reinvest reward. Anyone pressing the button and completing the transaction will receive the reward. With that in mind, it can be competitive, so be sure to be quick.

## Example of the Reinvest Process

So for example, let's say you're in the below pool for GMX's liquidity token GLP.&#x20;

<figure><img src="../.gitbook/assets/Screenshot 2023-10-06 at 14.25.25.png" alt=""><figcaption><p>Example for illustrative purposes only</p></figcaption></figure>

By participating in this pool, you have deposited your GLP tokens into the Yield Yak farm. Those LP tokens are then staked on GMX and the rewards for this pool are given in AVAX.

A reinvestor presses the button when there is a pending balance of **100 AVAX**.

* The reinvestor collects 0.05 AVAX (given a 0.05% reward)
* Yak's ARC contract collects 9.95 AVAX (given 10% fee including reinvest reward)
* 90 AVAX are reinvested

The remaining AVAX (or ETH) are sold for GLP and then deposited back in the pool.

## More information

### Protection Mechanism

The reinvest function contains a protection mechanism in order to limit how quickly two reinvests may happen in a row. By design, the second transaction (which receives almost no reward) should fail at a very low gas cost (\~0.03 AVAX) instead of being executed with the full gas usage.

If you receive almost no reward because someone else was slightly faster and your transaction was successful, please suggest a change to this configuration to our team.

### Transaction Failure

If you encounter a transaction failure after pressing the reinvest button, this is normally for one of two reasons:

1. Somehow you managed to submit a transaction when the token reward was below the minimum threshold. The fee (gas) is relatively low, however. (\~0.03 AVAX).
2. Somehow the default gas limit for reinvest is not sufficient for the transaction. You may need to manually increase the gas limit. Failure due to this may end up costing you the entire default gas limit.

### Fees

Fees are collected each time a farm is compounded, from the reward tokens.

Fees are usually between 5-10% of the reward tokens. Fees are variable and change with network conditions to optimize rewards. There are two categories of fees:

1. **Reinvest Reward** - paid to reinvestor who presses the button
2. **Admin fee** - collected by Yield Yak and automatically redistributed to YAK Holders, its treasury, and contributors.

Yield Yak enforces no deposit or withdraw fees (although the underlying farms may).

