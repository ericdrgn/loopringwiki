---
description: ''
sidebar: 'faq'
prev: '/faq/security/'
next: '/faq/exchangev1/'
---

# AMM

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

## Finding the highest earning pools on Loopring

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
