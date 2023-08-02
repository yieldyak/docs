---
description: How to withdraw from Yield Yak Pools directly
---

# Manual Withdrawal

In the event that you are unable to interact with http://yieldyak.com UI for whatever reason, you may need to conduct a withdrawal from the contract. Below, you will find a helpful guide on how to interact with Yield Yak farms and contracts directly from the explorer.

## Step 1. Locate the particular farm you wish to remove your LP from

**Method 1**: Locate the particular farm on yieldyak.com/farms that you wish to withdraw from and click on 'More' to go in to the farm detail page.&#x20;

Once there, scroll down and click the 'View on Explorer button' which will open the contract on [https://snowtrace.io/ ](https://snowtrace.io/)

![Click the 'View on Explorer' button on the farm detail page.](<../../.gitbook/assets/View on Explorer.png>)

**Method 2**: Open your wallet on C-Chain Explorer: [https://snowtrace.io/](https://snowtrace.io/) and click on the 'Tokens' drop down menu. Scroll down until you find the YRT tokens for the farm you wish to withdraw from and click it.&#x20;

## Step 2: Read Contract and balance

Once the page for that contract or token tracker loads, click on the 'Contract' tab and then 'Read Contract' button:

![Reading the contract on Snowtrace](<../../.gitbook/assets/Read Contract (1).png>)

Scroll down until you get to the 'balanceOf' field. Enter your wallet address and hit 'Query'. This will output your balance. Copy the number you see after '(unit256) : '.

![Copy the number after uint256:](<../../.gitbook/assets/Screenshot 2022-04-20 at 10.58.52 PM.png>)

## Step 3: Write contract and withdraw

Scroll up to the top of the page and click the 'Write Contract button':

![](<../../.gitbook/assets/Write contract.png>)

Then click the 'Connect to Web3' link which will prompt you to connect your wallet.

![Select MetaMask of WalletConnect to connect your wallet](<../../.gitbook/assets/Connect Wallet.png>)

Click 'OK' if you sbelow warning.

![Warning: Feature is in beta](<../../.gitbook/assets/Snowtrace Beta warning.png>)

You will see your wallet address and the Green circle confirming your wallet is connected.

![](<../../.gitbook/assets/Wallet connected successfully (1).png>)

Scroll down until you see 'withdraw' and paste the number from the previous page in to this field and click 'write'.

![](<../../.gitbook/assets/Withdraw from Contract.png>)

You will have to approve this transaction in Metamask (or whichever wallet you are using).&#x20;

You now have your LP tokens in your wallet.
