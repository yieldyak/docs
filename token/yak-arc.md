---
description: Yield Yak allows anyone to distribute platform revenues
---

# 🏧 Yak ARC

## Fee Collection

Yield Yak fees are collected by the [**Yak Fee Collector**](treasury.md#yak-fee-collector), a special treasury wallet which allows anyone to see the platform earnings in one place and distribute them according to the network configurations.

## Fee Distribution

Fees in the Yak Fee Collector contract can be distributed by anyone using [**Yak ARC**](https://yieldyak.com/arc). Yak ARC automatically converts and distributes fees to designated payees.

#### Payee Settings

* `MasterYak`: 33.34%
* `Treasury`: 33.33%
* `Contributors`: 33.33%

#### Multi-Currency Support

Fees are collected mostly in WAVAX, although other tokens may also be collected. The conversion of these other tokens into WAVAX is not currently handled by Yak ARC. Rather, an admin account handles token conversion on a regular basis.

## Staking Rewards

When AVAX is distributed to MasterYak, they will be distributed over a 7-day period. In this way, staking rewards are layered and smoothed, based on recent earnings.

**Staking Rewards Layering Example**

| Collection Date | Amount   | Ends   | Per Day |
| --------------- | -------- | ------ | ------- |
| Day 1           | 70 AVAX  | Day 7  | 10 AVAX |
| Day 2           | 140 AVAX | Day 8  | 20 AVAX |
| Day 3           | 70 AVAX  | Day 9  | 10 AVAX |
| Day 4           | 140 AVAX | Day 10 | 20 AVAX |

Staking rewards will vary, based on each layer of rewards starting and ending:

| Day       | 1      | 2      | 3      | 4      | 5      | 6      | 7      | 8      | 9      | 10     |
| --------- | ------ | ------ | ------ | ------ | ------ | ------ | ------ | ------ | ------ | ------ |
| 1st       | 10     | 10     | 10     | 10     | 10     | 10     | 10     |        |        |        |
| 2nd       |        | 20     | 20     | 20     | 20     | 20     | 20     | 20     |        |        |
| 3rd       |        |        | 10     | 10     | 10     | 10     | 10     | 10     | 10     |        |
| 4th       |        |        |        | 20     | 20     | 20     | 20     | 20     | 20     | 20     |
| **Total** | **10** | **30** | **40** | **60** | **60** | **60** | **60** | **40** | **30** | **20** |

