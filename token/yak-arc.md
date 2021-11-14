---
description: Yield Yak allows anyone to distribute platform revenues
---

# 🆕 Yak ARC

## Fee Collection and Distribution

The Yield Yak platform collects fees in the `YakFeeCollector` contract.

Anyone can convert and distribute fees to designated payees.

* `MasterYak`: 33.34%
* `Treasury`: 33.33%
* `Contributors`: 33.33%

{% hint style="info" %}
YY fees are paid mostly WAVAX, although other tokens may also be collected. The conversion of these tokens into WAVAX is not currently included in the scope of YakARC.
{% endhint %}

## MasterYak (Staking Rewards)

When AVAX is distributed to MasterYak, they will be distributed over a 7-day period. In this way, staking rewards are layered and smoothed, based on recent earnings.

**Staking Rewards Layering Example**

| Collection Date | Amount   | Ends        | Per Day |
| --------------- | -------- | ----------- | ------- |
| November 1      | 70 AVAX  | November 7  | 10 AVAX |
| November 2      | 140 AVAX | November 8  | 20 AVAX |
| November 3      | 70 AVAX  | November 9  | 10 AVAX |
| November 4      | 140 AVAX | November 10 | 20 AVAX |

Staking rewards will vary, based on each layer of rewards starting and ending:

| November  | 1      | 2      | 3      | 4      | 5      | 6      | 7      | 8      | 9      | 10     |
| --------- | ------ | ------ | ------ | ------ | ------ | ------ | ------ | ------ | ------ | ------ |
| 1st       | 10     | 10     | 10     | 10     | 10     | 10     | 10     |        |        |        |
| 2nd       | 20     | 20     | 20     | 20     | 20     | 20     | 20     |        |        |        |
| 3rd       |        | 10     | 10     | 10     | 10     | 10     | 10     | 10     |        |        |
| 4th       |        | 20     | 20     | 20     | 20     | 20     | 20     | 20     |        |        |
| **Total** | **10** | **30** | **40** | **60** | **60** | **60** | **60** | **40** | **30** | **10** |

