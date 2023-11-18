---
cover: ../.gitbook/assets/one yak to rule them all copy.jpeg
coverY: 0
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

# 🐃 YAK Token

YAK is the native token to Yield Yak. YAK is a fixed-supply token that can be staked to earn platform fees (currently 70% of all platform fees are distributed to YAK holders every 24 hours).&#x20;

* Only 10,000 YAK can ever exist. No additional YAK may be minted now or in the future
* Anyone can distribute platform revenue via [**Yak ARC**](https://yieldyak.com/arc)

{% content-ref url="using-yak.md" %}
[using-yak.md](using-yak.md)
{% endcontent-ref %}

## Token Details

* Chain: `Avalanche`
* Name: `Yak Token`
* Symbol: `YAK`&#x20;
* Decimals: `18`&#x20;
* Address: `0x59414b3089ce2AF0010e7523Dea7E2b35d776ec7`&#x20;
* Total Supply: `10,000`

### CoinGecko

[https://www.coingecko.com/en/coins/yield-yak](https://www.coingecko.com/en/coins/yield-yak)

## Bridged YAK

The canonical chain for YAK is Avalanche, where it was originally deployed. Today, YAK can be bridged to Arbitrum as an OFTv2 token from [**LayerZero**](https://layerzero.network/).

{% hint style="success" %}
**Bridge and YAK Tokenomics**

YAK tokenomics are not affected by the availability of a bridge. Only 10,000 YAK can ever exist with the fixed-supply accounting handled on Avalanche.

* YAK must be locked on Avalanche before it can be minted on Arbitrum
* YAK must be burned on Arbitrum before it can be unlocked on Avalanche
{% endhint %}

### Token Details

* Chain: `Arbitrum`
* Name: `Yak Token`
* Symbol: `YAK`
* Decimals: `18`
* Address: `0x7f4dB37D7bEb31F445307782Bc3Da0F18dF13696`

#### **Proxy OFTv2 Address**

* Chain: `Avalanche`
* Address: `0x656D33bfB74863E7aB1F5496a7a86a717A18a8D9`

## YAK Tokenomics

### **Inflation Policy**

YAK is a fixed-supply token. No additional YAK can be minted.

### Circulating Supply

{% hint style="info" %}
**Entire Supply Circulating**

YAK was originally deployed in 2021. All initial vesting has expired. The information provided below is for reference only.
{% endhint %}

The vast majority of the YAK token supply entered circulation following the initial distribution. On the first day,

* Circulating: 7,350 YAK
* Non-circulating: 2,650 YAK
  * Team: 1,500 YAK
  * Ecosystem: 1,150 YAK

Tokens will move from non-circulating to circulating based on team tokens vesting and ecosystem tokens being used for community initiatives.

{% content-ref url="treasury.md" %}
[treasury.md](treasury.md)
{% endcontent-ref %}

### Initial Distribution

YAK was originally deployed in 2021 with the initial distribution heavily weighted towards early users:

* 50% Depositors (airdrop)
* 15% Reinvest pushers (airdrop)
* 15% Team (vested)
* 15% Ecosystem
* 5% Community (airdrop)

### Airdrop Recipients

The full list of airdrop recipients is available [here](https://github.com/yieldyak/airdrop).

### Unclaimed Airdrop Tokens

Airdrop recipients were provided a 30-day window to claim tokens. Following the deadline, the remaining tokens were returned to the treasury.

## Mini Yak

Mini YAK (mYAK) is a wrapped version of YAK. Mini Yak introduces no changes to the YAK supply or tokenomics. Read more about Mini YAK:

{% embed url="https://yieldyak.medium.com/mini-yak-a022c2e607d7" %}

### Conversion Rate

mYAK is pegged at a 1,000,000:1 ratio with YAK. The conversion rate is always available in a smart contract for both directions, although you may find better rates with [**Yak Swap**](https://yieldyak.com/swap).

### Token Details

* Chain: `Avalanche`
* Name: `Mini YAK`
* Symbol: `mYAK`
* Decimals: `12`
* Address: `0xdDAaAD7366B455AfF8E7c82940C43CEB5829B604`
* Total Supply: `10,000,000,000` (maximum)

