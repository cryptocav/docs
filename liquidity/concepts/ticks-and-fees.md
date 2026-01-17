---
title: Understanding Ticks, Tick Spacing, and Fee Tiers on Orca
description: Deep dive into ticks, tick spacing, and fee tier selection.
icon: droplet
sidebarTitle: Understanding Ticks, Tick Spacing, an...
---

Ticks, tick spacing, and fee tiers are the backbone of Orca's concentrated liquidity (CLMM) pools. They provide flexibility and efficiency for liquidity providers (LPs) and deliver optimized trading. In this article we will explore each concept and take a closer look at how these elements interrelate, and hopefully, though increased understanding, enhance your experience of using Orca.

### What are ticks?

Ticks are discrete price intervals within a pool. By segmenting price ranges into ticks, LPs are able to allocate capital precisely where it’s most effective (maybe where they think most trading will occur). For example, you might choose to concentrate liquidity within a specific range for a pair like USDC/SOL, optimizing your capital for expected market conditions.

### What is Tick Spacing?

*Tick spacing* describes the size (or granularity) of ticks and therefore price intervals, used for a given pool.
Narrow spacing allows for higher precision when depositing liquidity. This increased precision is typically best suited to stable or price correlated pairs with predictable price movements. Wider spacing, on the other hand, suits volatile pairs, providing flexibility for asset pairs expected to see greater price volatility.

*Tick spacing* and *fee tiers* on Orca are correlated ensuring LPs for more volatile pairs are more likely to earn higher yields to offset increase risk exposure.

### What are Fee Tiers?

Fee tiers describe the transaction fee paid by traders when trading against the liquidity in a pool. These fees are used to generate yield reward LPs. There are a broad selection of fee tiers available on Orca from 0.01% to 2%. It is typical to find most liquidity for stable and price correlated pairs allocated to lower fee tiers due to lower price risk, while volatile pairs adopt higher rates to compensate for greater price risk exposure. LPs can effectively compete with one another by adjusting their liquidity across different fee tiers, seeking optimal returns. Typically periods of increased market volatility leads to an increase of movement of liquidity through these tiers (laddering) as LPs attempt to react dynamically to price fluctuations and meed demands of the prevailing, or expected, trading activity.
On Orca, every fee tier operates as a separate pool, in competition with other fee tiers on the platform and also with external liquidity sources. This competition drives opportunities for arbitrage traders, and LPs to exploit fee and price differences between pools for profit. Periods of heightened market volatility amplify this competition, causing liquidity to flow rapidly between tiers.

> **Now introducing Adaptive Fee Pools**
>
> With the introduction of Orca’s Adaptive Fee pools, LPs can now deposit into this new class of pool where fee tiers function as a base rate rather than a fixed rate. In contrast to traditional Fixed Fee pools—where the trader always pays a fixed fee based on the selected fee tier——Adaptive Fee pools allow the actual fee to increase in response to price volatility.
> This means LPs can still select their desired base fee tier (from 0.01% to 2%), but benefit from higher fees (and therefore potentially greater yield) during periods of elevated market volatility.
> e.
> Adaptive Fee pools represent a more flexible way for LPs to compete and respond to shifting market dynamics while maintaining the clarity and control of Orca's fee tier structure.

### How do Ticks, Tick Spacing, and Fee Tiers interrelate?

On Orca tick spacing and fee

* **Efficiency:** Narrow tick spacing optimizes capital efficiency in low-volatility, stable and price correlated pools.
* **Risk and Coverage:** Wider tick spacing is ideal for volatile pairs, offsetting risks of increased price risks and divergence loss exposure.
* **Trader Costs:** Concentrated liquidity reduces slippage and price impact for traders.
* **Liquidity Provider Strategy:** LPs can leverage these concepts to strategically allocate liquidity, balancing potential earnings against risks.
* **Yields:** Yields derived from trading fees are distributed to LPs based on their share of the liquidity in the tick the trade was executed against.
* **Rewards Distribution:** Rewards for liquidity providers are distributed based on their share of the liquidity in the current tick. The more liquidity you provide to an active tick, the greater your share of the rewards.

For more information about tick spacing and associated fee tiers for Solana and Eclipse, visit our [documentation on trading fees](https://docs.orca.so/useful-information/trading-fees).

### Conclusion

Ticks, tick spacing, and fee tiers are integral to our pool's functionality and understanding these concepts should empower you to improve your liquidity strategies. Dive into our pools armed with your new understanding, and hopefully unlock the full potential of Orca's concentrated liquidity.