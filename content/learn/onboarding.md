---
description: ''
sidebar: 'learn'
prev: '/learn/deploymentmainnet/'
next: '/learn/liquidity/'
---

# Exchange v2 Onboarding

[![](https://img.youtube.com/vi/blizra8V63A/0.jpg)](https://www.youtube.com/watch?v=blizra8V63A "Onboarding to Exchange v2")

## Using L2 Exchange

Ethereum layer 2 scaling is needed now more than ever. Luckily, Loopring zkRollup is here to help you save gas, save time, and basically not get stuck on congested layer 1 — all while maintaining complete Ethereum self-custody security. Below is a walkthrough guide about Loopring Exchange, the layer 2 DEX built atop the Loopring zkRollup.

## What is Loopring Exchange?

Loopring Exchange is a non-custodial Ethereum exchange built on Loopring layer 2. It is an orderbook-based and AMM-based exchange that replicates the high-performance, low-cost trading experience of centralized exchanges. Users can trade speedily & cheaply (without worrying about Ethereum congestion or gas fees) while maintaining self-custody control of their assets. The exchange is built atop the open source Loopring protocol.

Loopring Exchange is more than a DEX, and also acts as a payment app. Users can send ETH and ERC20 token transfers to any Ethereum address instantly, cheaply, and securely on L2.

## What is a zkRollup?

zkRollup is a type of layer 2 scaling solution on Ethereum, allowing much higher throughput and much lower costs, without sacrificing security. It does this by moving all of the heavy lifting (computations) off-chain, keeping the rules enforced and security in intact by using validity proofs: cryptographic proofs attesting to what happened off-chain. Because Ethereum verifies these proofs, and stores enough data to tell exactly which off-chain account owns what, zkRollups inherit the same non-custodial security as Ethereum, but can run much faster. For more in-depth technical info, read our Design Doc.

## Guide

You can currently access Loopring L2 by going to Loopring Exchange on a web browser, or through the Loopring smart wallet mobile app (currently available for Android only).

We’ll focus on the Loopring Exchange web platform in this guide, but note that all the L2 tactics you learn here can be applied to your Loopring wallet as well. If you’re more technical, you can also interact with L2 via our relayer API.
How to get onboard Loopring L2

1. Head to Loopring Exchange. Click ‘Connect Wallet’ and link up your MetaMask, MEW, or a WalletConnect-compatible wallet.

2. With your wallet connected, you will see it says “Deposit to Activate Layer-2”. Click that. Choose an asset to deposit, and the amount. Confirm the transaction in your wallet to execute the deposit. After 18 Ethereum confirmations, you’ve made it to the zkRollup!

    Note: Since depositing is an Ethereum layer-1 transaction, meaning it moves from L1 to L2, this costs gas. It is approximately just the gas cost of a normal token transfer. Pay this gas cost once, and then you are on L2 with those assets, living gas-free for as long as you’d like.

As mentioned, you must deposit your assets into a smart contract to get onto L2. This contract receives your assets and ‘maps’ them to your slot in the Merkle tree, which you — and only you — control. You can withdraw your assets from the contract whenever you like, even if Loopring disappeared or turned evil (only Ethereum needs to exist for your assets to be safe).

Pro tip: Some people are apprehensive about paying a gas fee just to get on L2. But truth is, it is cheaper to deposit to L2 once than it is to do one Uniswap trade. Depositing ETH and most ERC20 tokens onto Loopring is ~60k gas whereas a swap on Uniswap costs around ~120k gas per swap. And you only need to migrate once! The rest of your token swaps are gas-free!

3. There should be an ‘Unlock’ button. Go ahead and click that. This asks your wallet for a signature to unlock your L2 account. It is a signature, not a transaction, so no gas fee!

This ‘Unlock’ button will appear every time you access your L2 account from here on. It’s the equivalent of logging on, but just needing your Ethereum address to sign a transaction with one click.

Once you’re logged in, you can check out your Loopring L2 balances, deposit other assets, or withdraw back to L1 by click on the “Account” tab.

## How to make instant transfers on Loopring

The ‘Account’ tab is also where you can send assets on L2 to any other Ethereum address — whether they have previously used Loopring L2 or not. It is ideal for payments, especially frequent ones to many people!

All you need is someone’s Ethereum address or ENS name, choose the asset and amount, and you can send them an instant, gas-free transfer on L2. You can even add a memo. Click ‘Transfer’, sign the request, and it is sent.

    Note: Transfers are currently free on Loopring unless the transfer is to a ‘new’ account that has never interacted on L2. Only in this case is there a small flat fee of a few cents to cover the account activation cost. Eventually, there will be a very small flat fee of a few cents for all transfers.

## How to swap tokens gas-free

Loopring L2 supports both types of Ethereum DEX ‘market structures’: orderbooks and Automated Market Makers (AMMs). First let’s look at swapping on the AMM.

On Loopring Exchange, click on the ‘Swap’ tab at top. Choose your pool (each pool has two assets you can swap between) and which way you are swapping. Choose your amount to swap.

The AMM pool will automatically show you the exchange rate.

You will also see the minimum amount you are guaranteed to receive from the swap. You can adjust the slippage tolerance by clicking the gear near top right. Just beware of the price impact in some illiquid pools!

Currently, Loopring fees are 0.25% for the swap. 0.15% of that goes to liquidity providers (LPs), the remaining 0.1% goes to the relayer and protocol fee. Fees are taken from the token you are buying. Remember: there are no gas fees!

Once you’re ready, click ‘Swap’ and your transaction will be executed instantly. No delay, no gas fee. Your L2 balance will be updated. You can see your swap history and the fees you paid in the ‘Orders’ tab.

## How to add liquidity to an L2 AMM pool

Liquidity providers (LPs) currently earn 0.15% fee from all trades in the pools they provide liquidity to, proportional to their share of that pool. To become an LP, like Uniswap and other AMMs, you simply deposit an equal value of both assets in the pool. Depositing to a pool incurs no fees, and per usual, it’s gas-free too!

To become an LP on Loopring, head over to the ‘Pool’ tab on top, and choose which pool you want to provide liquidity to from the drop-down menu. Click ‘Add’.

To add liquidity to a pool, you need an equal value of both assets, which gets deposited to the pool at the prevailing exchange rate of that pool. That is, if you want to become an LP in the LRC-ETH pool, you would need $100 worth of LRC and $100 worth of ETH. In future, you will be able to deposit with a single asset — we’re working on that!

Choose the amount you want to add from one asset or the other. The UI will automatically prompt you to deposit the other asset quantity given the exchange rate at that time to ensure an equal value. Then click ‘Add’.

Your deposit will execute immediately.

Your position in the pool will be represented by LP tokens which you hold on L2. You can see your LP tokens for a given pool and the percentage that it represents on the ‘Pool’ page. You can also see your LP tokens in your ‘Balance’ under ‘Account’, since it is effectively an asset like any other. The name of an LP token for the LRC-ETH pool for example would be LP-LRC-ETH.

To see the history of your AMM pool add/remove liquidity operations, click ‘Account’, and then ‘AMM Transactions’.

    Note: being an LP is not risk free. You face the potential risk of ‘impermanent loss’ just like with most other AMMs.

Finding the highest earning pools on Loopring

Under the ‘AMM Info’ tab, click ‘AMM pools’. Here you’ll see the liquidity in each pool, the volume, fees earned, and if there are any LRC liquidity mining or other incentive programs.

All of this ultimately leads to an APY (annualized percentage yield) column, so you can see the expected return you’d earn from being an LP in that pool.

To learn more about liquidity mining on Loopring L2, read this. There are liquidity incentives provided in LRC and other tokens for certain AMM pools. These incentive campaigns change in 14-day cycles, so keep an eye on the AMM pools page and our Discord for updated APYs and cycles.

If you’re interested in liquidity mining, all you have to do is be an LP in the relevant pools. There’s nothing more to do. Just hodl!

The liquidity mining rewards are automatically sent to accounts on L2 at the end of the 14-day cycle.

    Note: There are also rewards for traders! Users with high swap volume in a given pool are rewarded. Click ‘AMM Swap Tournament’ to learn which pools are being incentivized and with how much in rewards. This also changes in 14-day cycles.

## How to remove liquidity from an AMM pool

On the ‘Pool’ tab, you will see ‘My Pools’ which shows you the pools currently have assets in. You can go ahead and click ‘Remove’.

You will be prompted to decide how much of your assets you want to withdraw from that pool. Decide the amount, which effectively means redeeming your LP tokens for that portion of the underlying two tokens.

You will see the amount of each token you will be getting back in return. Please note that there is a very small fee when removing liquidity from a pool!

    Note: This amount you are removing includes any fees you have earned throughout your time providing liquidity. LP fees (0.15%) automatically accrue to the pool every time someone swaps with that pool. This enlarges the pool for all LPs, so when you remove your liquidity, you are taking your share of the fees with you.

There is a fee to remove liquidity from the AMM pool. This is because the operation, even though done on L2, has a smaller corresponding L1 gas cost. So the cost varies with gas prices on L1. At time of writing, it is 0.0073 ETH.

## How to trade on the orderbooks

Loopring is more than just an AMM. It is also an orderbook DEX. So if you rather ‘trade’ a pair on the books rather than the pool, head over to the ‘Trade’ tab.

There you will see the familiar orderbook layout, displaying bids and asks, a price chart, price history, etc. Note: sometimes the orderbooks has different asset pairs than the AMM pool. Especially stablecoin to stablecoin pairs.

The orderbooks support limit orders, meaning you can state the price you want to buy or sell at, and leave it resting on the books. Someone can then come along and fill your order. This way, you are guaranteed to get the price you want.

Makers receive rebates on their orders that get filled on the books. The rebate is 0.02% (2 bps). So any resting limit order you have that gets taken by another user, you earn 0.02% of that amount — i.e., a negative fee!

Right now there are no market orders (buys or sells at the prevailing best ask or bid). If you want to do a market order, though, it is quite easy to replicate. Just click on one of the orders you would like to take, and it will auto-fill those details into the order placement area. Make sure you select whether you want to Buy or Sell that asset. Click Buy or Sell, and that’s it.

    Note, in addition to maker rebates, there is also often liquidity mining for orderbook pairs! This incentivizes users (especially market makers or algorithmic traders) to place tight resting limit orders on the books, and receive rewards for providing that liquidity (being a maker) for others to take. Learn more about how orderbook liquidity mining works here. If you want to plug into the orderbooks to trade or MM programatically, here is the API. You may also want to plug into an existing market making software that is connected to Loopring Exchange, such as Hummingbot!

## How to Withdraw From L2 to L1

On the ‘Account’ tab, you can withdraw assets from your Loopring L2 account back to Ethereum L1. Remember, a big virtue of zkRollups is that you can withdraw at anytime — your funds can never be stolen, frozen, or seized by Loopring.

Select the asset you want to withdraw and the amount. You can withdraw to a different address than your own; not just moving from your L2 to your L1, but from your L2 to a different L1. Either a different address of yours, or a friend, etc.

But by default, your own address is entered. Click ‘Withdraw’ and you will be prompted to sign a message, and that’s it.

Due to the aggregation of a zkRollup, and since it’s an L2 to L1 interaction, withdrawals can take some time until the ‘train wants to leave the station from L2 to L1’.

It can be 5 to 30 minutes to withdraw, or a few hours depending on a couple variables. With more activity on L2, it will actually be much shorter, since trains will leave the station more frequently as seats fill much quicker and more consistently.

There is a fee to process a withdrawal, since the Loopring relayer has costs in processing these withdrawals (compute power for the ZK proofs, and the overhead gas cost to publish a rollup block to Ethereum). This fee fluctuates with L1 gas fees, and is usually less than half the cost of token transfer on L1.

If you’re in a rush to move from L2 to L1, we just enabled ‘fast withdrawals’. This was a much-requested feature allowing you to withdraw to L1 in the very next Ethereum block, you just pay a higher fee for the expedience.
Congratulations! You are at the cutting edge of Ethereum.

Layer 2 is the present and future of Ethereum scaling. and will actually be magnified by the rollout of Eth 2.0, not replaced by it. L2s will support a massive amount of economic activity, while L1 will be where rollups settle their big batches of txs representing all the user activity off-chain. L1 will be the settlement layer (or for whale movements), L2 will be the environments where most users actually ‘live’ and use applications.

If you completed this tactic, then you are ahead of the pack in seeing what the future of finance looks like.

If you’re an Android user, you can check out the mobile smart wallet and have the power of Loopring L2 in your pocket. iOS will be out any day.

Thanks, have fun on L2!
