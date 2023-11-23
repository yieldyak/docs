---
description: Unique pools which loop your deposits multiple times to maximise rewards
---

# ⚒ Single-Asset Leverage Strategies

Yield Yak offers one-click leveraged farming strategies for borrowing and lending markets like Aave, Benqi, and others.  These strategies optimise your single-asset deposits, automatically compound your returns, and save you time.

## Aave Incentives for Lending and Borrowing <a href="#a709" id="a709"></a>

Aave is a lending product where users who lend funds to Aave are eligible to receive interest payments by borrowers.

On top of native lending returns, Aave may offer additional incentives through various network incenetives programs. Let's take the case of Avalanche's Avalanche Rush program for this example.&#x20;

During this, Aave pays both borrows and lenders in WAVAX incentives. For most assets today, borrowers are paid to borrow because the incentives are worth more than the cost of borrowing.

<figure><img src="https://miro.medium.com/v2/resize:fit:1400/1*t-HRKtfZ85x-q9-aCJ7t6Q.png" alt="" height="221" width="700"><figcaption><p>Borrowing Incentives > Interest (<a href="https://app.aave.com/markets">Aave Markets</a>)</p></figcaption></figure>

In such conditions, Aave users may use low-risk leveraged lending strategies to maximize their APY. Yield Yak helps optimize these strategies and saves time.

## Yield Yak Strategy <a href="#d0b3" id="d0b3"></a>

YY uses leveraged farming which repeatedly lends and borrows the same asset. By doing so, YY earns the incentivized APY on deposits plus the incentivized APY on debt.

This is considered a low-risk leverage strategy because both lending and borrowing use the same asset, meaning the risk of liquidation is significantly easier to manage without exchange rate volatility.

## Leveraged Position Example <a href="#45cb" id="45cb"></a>

DAI has a 75% collateral factor, meaning borrowers can borrow up to 75% of the deposits and lend them again. Rolling up a hypothetical leveraged position:

* Deposit 100 DAI, borrow 75 DAI
* Deposit 75 DAI, borrow 56 DAI
* Deposit 56 DAI, borrow 42 DAI
* Deposit 42 DAI

After four steps, the original 100 DAI is now leveraged. The deposits are worth 273 DAI with 173 DAI worth of debt.

This position earns the incentivized lending APY on 2.73x the original deposit, plus 1.73x of the incentivized borrowing APY.

```
  273 x 10.79% APY (lend side)+ 173 x  1.36% APY (borrow side)----------------        32.45% APY, leveraged deposit
```

Compared to just depositing the original 100 DAI, this represents over a 3X return.

YY may leverage up to seven times. However, a lower leverage target provides benefits: at today’s TVL, going past four leverage steps has a low relative impact to the additional gas consumed. And by saving gas, YY enables more frequent reinvests which compound incentives faster and reset positions to their target leverage.

## When to Avoid Leverage <a href="#1a5f" id="1a5f"></a>

There are two scenarios where leverage should not be applied to today’s strategies:

1. The collateral factor of an asset is 0%, meaning it is not possible to borrow
2. The net borrowing APY turns significantly negative and the impact of a leveraged strategy is diminished.

YY may modify target leverage, meaning changing market conditions are automatically reflected in the yield for users.\
