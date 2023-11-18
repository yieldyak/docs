---
description: >-
  Get the best price leveraging multi-step routes, low price slippage, and
  execute with one click.
cover: ../.gitbook/assets/YY Swap Logo_V7 (1).png
coverY: 20
layout:
  cover:
    visible: true
    size: hero
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
---

# 👉 Why use Yak Swap?

## Best Price Search

Even for the same pair of token swap, say buying $YAK using $AVAX or $ETH, there are many Decentralised Exchange’s on Avalanche and Arbitrum to choose. Although the existence of the arbitrage may help converge the price ratio on different DEX’s, there may still be a difference. Yak Swap compares the prices available on most DEX’s and finds out the best one for you.

## Price Slippage

Price slippage could be viewed as a punishment of reducing the liquidity of the token you are swapping to in a trade. Usually, a large swap in a DEX with low liquidity of the to-token would result in high price slippage and therefore significantly reduce the amount of received token. Yak Swap takes price slippage into account and offers you the best execution route.

## One-Click Execution

Sometimes, you may be exchanging two tokens that do not have liquidity on the same DEX simultaneously. For example, you want to trade from $YAK to $yyAVAX.  Liquidity pairs involving $yyAVAX may be on KyberSwap, Trader Joe, WooFi etc. However, these exchanges have minimal $YAK liquidity. A direct swap from $yyAVAX to $YAK on these platforms would result in a huge loss. Most liquidity for $yyAVAX is on Trader Joe and most liquidity for $YAK on Pangolin.  A two-path swap from $yyAVAX to $AVAX on Trader Joe first and then from $AVAX to $YAK on Pangolin avoids the huge loss.

Yak Swap detects all these possible multi-step execution routes for comparison. We offer you the best price available and you can execute it just by one click on Yak Swap. The transaction would pass through the required smart contracts and finish the swap.

## Minting complex assets like GLP, sAVAX, and yyAVAX <a href="#5d4b" id="5d4b"></a>

Yak Swap has built-in integrations with complex assets, which will check whether it is better to purchase the asset through a traditional swap venue, or directly mint the asset instead. This goes for liquid staking tokens like Benqi’s sAVAX and Yield Yak’s yyAVAX, where Yak Swap will always get you the best price when purchasing said asset and minting them when it is cheaper.

With GMX’s GLP, Yak Swap will uniquely take into account minting fees and slippage, and route your trade through the cheapest and most efficient asset to purchase GLP. No other aggregator does this, creating savings for the user and helping GMX reach target weighting for their GLP product.&#x20;

## 100% uptime, no maintenance cost, anyone can use it and add to it <a href="#d400" id="d400"></a>

Because Yak Swap is fully on-chain and works via contract calls, it has 100% uptime and there is no proprietary API or server required to use it (so no external points of failure). Any trader can query the best price no matter who or where they are (no blacklisting) and protocols can even deploy their own Yak Swap router and enjoy on-chain price aggregation.

This approach also means no maintenance costs, making it sustainable to upkeep without having to charge high fees or take a cut on the price offering. Integrating Yak Swap is extremely simple and takes only a few minutes. And if you want something custom, simply fork Yak Swap and add whatever you’d like extra yourself. It’s an open tool to benefit builders and the Avalanche community.

An overview of how Yak Swap smart contracts work and how to integrate them is in our [**Github repo**](https://github.com/yieldyak/yak-aggregator). It’s so simple! And if you do need assistance, you can reach out to the Yield Yak team for assistance on any of our Community channels.
