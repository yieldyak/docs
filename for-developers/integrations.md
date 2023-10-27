# 👨💻 Integrations

## Background

Auto-compounders give small token holders the same compounding advantages as big token holders. Auto-compounders are more effective when they hold more deposits. For this reason, YY Strategies are designed to be primitives that any project can easily integrate.

## Example Integration

Compounding BAG: [https://cchain.explorer.avax.network/address/0xf487044eD85F2d47A8eAD6b86c834976B8c31736/read-contract](https://cchain.explorer.avax.network/address/0xf487044eD85F2d47A8eAD6b86c834976B8c31736/read-contract)

### User Balances

User balances are accounted with Yak Receipt Tokens (YRT). The number of shares corresponds to ownership of each pool's underlying assets.

`User balance of BAG = YRT shares * (total BAG / total shares)`

| View Function                        | **Description**                                                         |
| ------------------------------------ | ----------------------------------------------------------------------- |
| `balanceOf(address)`                 | Amount of shares a user owns (number does not go up)                    |
| `getDepositTokensForShares(uint256)` | Conversion rate for a given amount of shares (number goes up over time) |

### User Actions

Each strategy allows users to deposit and withdraw. The simplest implementation may use only two functions:

| Write Function      | Description                              |
| ------------------- | ---------------------------------------- |
| `deposit(uint256)`  | Deposit deposit tokens                   |
| `withdraw(uint256)` | Redeem shares to withdraw deposit tokens |

{% hint style="info" %}
There is no need for integrations to manage `reinvest()` functionality, as the YY community “just handles” it.
{% endhint %}

## Example Integrations

### Asset Management

* [Baguette Finance](https://app.baguette.exchange/#/mill)
* [Avme Wallet](https://twitter.com/AVME\_IO/status/1404453576978673671?s=20)

### Asset Trackers

* [Markr](https://markr.io/)
* [Zapper](https://zapper.fi/)
* [DeBank](https://debank.com/)
* [0xTracker](https://0xtracker.app/)

### Contributors Email Inbox

Used for official listings and admin: yakcontributors@proton.me

For dev-related inquiries, visit the Yak Devs Telegram group: [https://t.me/yakdevs](https://t.me/yakdevs)



