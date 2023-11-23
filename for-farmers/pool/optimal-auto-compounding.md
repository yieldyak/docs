---
description: Yield Yak leverages Yak Swap's smart routing to maximise every single reinvest
---

# 💪 Optimal Auto-Compounding

Historically, auto-compounding platforms use fixed routing when reinvesting the socialised rewards in an auto-compounding pool.  An example:&#x20;

User deposits in an ETH-USDC pool that accumulates $ARB rewards.  When enough rewards accumulate for a reinvest, the auto-compounder would be configured to use a fixed Decentralised Exchange, such as Uniswap, which upon every reinvest would swap half the ARB rewards for ETH, and half for USDC on.&#x20;

In most cases this does not cause a problem as the liquidity source is deep enough.  However, what happens if liquidity is removed from the Uniswap pool or another DEX offers a better price?  Users in the pool sacrifice returns and lose out on potential yield. &#x20;

Enter Yield Yak.

## Harnessing the Power of Yak Swap

<figure><img src="../../.gitbook/assets/Powered by Yak Swap (1).jpeg" alt=""><figcaption><p>Yak Swap's integration into Yield Yak's Pools ensure rewards are always maximised</p></figcaption></figure>

Yield Yak has uniquely integrated its zero-fee DEX aggregator, Yak Swap, into its reinvest functionality.  Every time a reinvest is triggered, Yield Yak's smart contracts use Yak Swap to check that rewards are optimised for pool depositors. &#x20;

Using the same example of an ETH - USDC pool earning $ARB rewards: &#x20;

Yield Yak:&#x20;

* Checks for the best $ARB - $ETH price across all available liquidity.  I.e. The swap may be routed through Trader Joe, instead of Uniswap, if Trader Joe offers best price. &#x20;
* Checks for best $ARB - USDC price.  The swap may be routed through WooFi, instead of Uniswap, if WooFi offers best price. &#x20;

Other Auto-Compounders:&#x20;

* Sells all $ARB rewards on Uniswap, regardless of price.

While on any given transaction, the additional rewards may be small, overall these small optimisations add up.&#x20;

Yield Yak users simply earn more.

#### Gas Optimisation Balance

Using Yak Swap for reinvests does incur higher gas fees, so in some cases where a rewards-pair has deep & reliable liquidity, routes may be fixed to this liquidity source if the gas-savings are greater than the benefit of using Yak Swap. \


[Yak Swap Overview](https://docs.yieldyak.com/for-traders/swap)&#x20;
