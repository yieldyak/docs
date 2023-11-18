---
description: Yield Yak allows anyone to distribute platform revenues
---

# 🏧 Yak ARC

{% hint style="info" %}
**Avalanche Only**

The following details only apply to Avalanche. There is a similar, but different mechanism available on Arbitrum.
{% endhint %}

## Fee Collection

Yield Yak fees are collected by the [**Yak Fee Collector**](treasury.md#yak-fee-collector), a special treasury wallet which allows anyone to see the platform earnings in one place and distribute them according to the network configurations.

<figure><img src="../.gitbook/assets/Screenshot 2023-10-06 at 14.40.42.png" alt=""><figcaption><p>YAK ARC distributed YIeld Yak's Platform Fees via a transparent and decentralised mechanism.</p></figcaption></figure>

## Fee Distribution

Fees in the Yak Fee Collector contract can be distributed by anyone using [**Yak ARC**](https://yieldyak.com/arc). Yak ARC automatically converts and distributes fees to designated payees.

#### Payee Settings

* `Yak Stakers`: 70%
* `Treasury`: 15%
* `Contributors`: 15%

#### Multi-Currency Support

Fees are collected mostly in WAVAX, although other tokens may also be collected. The conversion of these other tokens into WAVAX is not currently handled by Yak ARC. Rather, an admin account handles token conversion on a regular basis.

## Staking Rewards

When AVAX is distributed to MasterYak, they will be distributed over a 7-day period. In this way, staking rewards are layered and smoothed, based on recent earnings.

**Staking Rewards Layering Example**

<table><thead><tr><th width="188.7142857142857">Collection Date</th><th width="150">Amount</th><th width="150">Ends</th><th>Per Day</th></tr></thead><tbody><tr><td>Day 1</td><td>70 AVAX</td><td>Day 7</td><td>10 AVAX</td></tr><tr><td>Day 2</td><td>140 AVAX</td><td>Day 8</td><td>20 AVAX</td></tr><tr><td>Day 3</td><td>70 AVAX</td><td>Day 9</td><td>10 AVAX</td></tr><tr><td>Day 4</td><td>140 AVAX</td><td>Day 10</td><td>20 AVAX</td></tr></tbody></table>

Staking rewards will vary, based on each layer of rewards starting and ending:

<table><thead><tr><th width="150">Day</th><th width="150">1</th><th width="150">2</th><th width="150">3</th><th width="200">4</th><th width="150">5</th><th width="150">6</th><th width="150">7</th><th>8</th><th>9</th><th>10</th></tr></thead><tbody><tr><td>1st</td><td>10</td><td>10</td><td>10</td><td>10</td><td>10</td><td>10</td><td>10</td><td></td><td></td><td></td></tr><tr><td>2nd</td><td></td><td>20</td><td>20</td><td>20</td><td>20</td><td>20</td><td>20</td><td>20</td><td></td><td></td></tr><tr><td>3rd</td><td></td><td></td><td>10</td><td>10</td><td>10</td><td>10</td><td>10</td><td>10</td><td>10</td><td></td></tr><tr><td>4th</td><td></td><td></td><td></td><td>20</td><td>20</td><td>20</td><td>20</td><td>20</td><td>20</td><td>20</td></tr><tr><td><strong>Total</strong></td><td><strong>10</strong></td><td><strong>30</strong></td><td><strong>40</strong></td><td><strong>60</strong></td><td><strong>60</strong></td><td><strong>60</strong></td><td><strong>60</strong></td><td><strong>40</strong></td><td><strong>30</strong></td><td><strong>20</strong></td></tr></tbody></table>

