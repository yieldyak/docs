# Impermanent Loss

When a farmer provides liquidity on an AMM, the two assets are deposited at a 50:50 ratio of their value to each other (at the time of depositing). The AMM protocols are controlled by complex mathematical formulas that adjusts the ratios of the underlying assets in the pool whilst also determining their prices. As the value of AVAX and ETH fluctuates the AMM will adjust the LP farmers ratio to ensure they remain at a 50:50 value. This means that a farmer can lose out on gains from a deposited asset that outperforms.&#x20;

So, for the purposes of this example let’s assume 1 ETH = 100 AVAX & 100 AVAX = 1 ETH. The farmer provides liquidity on an AMM and deposits 100 AVAX and 1 ETH and receives the ‘receipt’ (LP) token which can then be deposited on Yield Yak to auto-compound. In the event that the price of AVAX starts to increase as more and more people are purchasing AVAX. In this event, the pool adjusts the ratio to ensure the value remains split 50:50 across AVAX and ETH.&#x20;

Now 1 ETH is suddenly only worth 50 AVAX because of the price jump in AVAX. But because the protocol automatically adjusted the amount of tokens in the pool, the farmer lost out on the AVAX rally.&#x20;

This is impermanent loss. If the price of ETH and AVAX fluctuate in line with each other then no IL is realised. But if one of the two assets price increases substantially then the farmer loses out.

In the example above the farmer would have been better off simply hodling their AVAX/ETH if they removed their liquidity from the AMM pool.&#x20;

However, if the farmer stays in the pool and the value of AVAX goes back down to its original value then the value of the farmer's overall holdings will go back to the original value also and they would have 100 AVAX & 1 ETH (or even more if they deposited their LP tokens on Yield Yak!).\


![](../../.gitbook/assets/il-graph.png)

Remember, Impermanent Losses only become permanent once you remove your liquidity.&#x20;

## How to protect yourself against IL?

One way in which you can reduce your exposure to IL is to provide liquidity for pairs where the relative price of each asset remains fairly constant. For example, a stablecoin pair like DAI-USDT would give you very little exposure to IL.

The downside of these pools however, is, you gain no benefit from price increase, the number of these pools are fewer and the returns may not be as attractive as other pools.
