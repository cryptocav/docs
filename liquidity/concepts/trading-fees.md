---
title: Trading fees
description: Understand how trading fees work and are distributed.
icon: droplet
---

### Trading Fees on Orca

Whenever a trade is executed on Orca, a percentage of the input token is collected as a trading fee. The exact fee depends on the **fee tier** of the pool (or pools) used for the trade.

Orca supports two types of fee structures:

* **Fixed Fee Pools** — where the fee is constant
* **Adaptive Fee Pools** — where the fee increases relative to volatility

### Fee Distribution

The total trading fee is deducted from the input token.

🧾 *Input token:* The token supplied by the trader at the start of the trade — for example, in a SOL → USDC trade, SOL is the input token, and the trading fee is deducted from the SOL amount.

This fee is then distributed among the liquidity provider (maker), the protocol, and the Climate Fund.

This distribution is consistent across both the Solana and Eclipse networks, and applies to all fee tiers:

* 87% to the Liquidity Provider
* 12% to the Protocol Treasury, subdivided as follows:

  + 50% to the initial development team, supporting ongoing operations and development
  + 30% to the Orca DAO Fee Treasury
  + 20% used programmatically to buy ORCA for the xORCA pool

* 1% to the Climate Fund

### Fee rate and Tiers

When a new pool is created, the fee rate is selected by the pool creator. In the context of a CLMM (concentrated liquidity market maker), the fee rate functions similarly to a spread in a traditional order book.

Each fee tier is associated with a specific tick spacing and defines the percentage of the trade value paid as a fee.

The table below outlines:

* The Tick Spacing and Fee Tier
* The Fee paid by the trader (taker)

* How the fee is shared between the Liquidity Provider (Maker), Orca DAO Treasury, and Climate Fund

> **Note:**
> For fixed fee pools, the fee paid by the trader is always equal to the selected fee tier.
> For adaptive fee pools, the base rate matches the selected fee tier, but the actual fee may increase dynamically based on volatility.
> Regardless of whether the fee increases, the fee split remains the same: 87% to LPs, 12% to protocol, 1% to the Climate Fund.

### Solana Fee Tiers

| Tick Spacing | Fee Tier¹ | Maker Fee | Protocol Treasury | Climate Fund |
|---|---|---|---|---|
| 256 | 2% | 1.74% | 0.24% | 0.02% |
| 128 or 32896 | 1% | 0.87% | 0.12% | 0.01% |
| 96 | 0.65% | 0.5655% | 0.0078% | 0.0065% |
| 64 | 0.3% | 0.261% | 0.036% | 0.003% |
| 16 | 0.16% | 0.1392% | 0.0192% | 0.0016% |
| 8 | 0.08% | 0.0696% | 0.0096% | 0.0008% |
| 4 | 0.04% | 0.0348% | 0.0048% | 0.0004% |
| 2 | 0.02% | 0.0174% | 0.0024% | 0.0002% |
| 1 | 0.01% | 0.0087% | 0.0012% | 0.0001% |

¹ The taker fee matches the fee tier percentage

### Eclipse Fee Tiers

| Tick Spacing | Fee Tier¹ | Maker Fee | DAO Treasury | Climate Fund |
|---|---|---|---|---|
| 256 | 2% | 1.74% | 0.24% | 0.02% |
| 128 or 32896 | 1% | 0.87% | 0.12% | 0.01% |
| 64 | 0.65% | 0.5655% | 0.0078% | 0.0065% |
| 32 | 0.3% | 0.261% | 0.036% | 0.003% |
| 16 | 0.15% | 0.1305% | 0.018% | 0.0015% |
| 8 | 0.1% | 0.087% | 0.012% | 0.001% |
| 4 | 0.05% | 0.0435% | 0.006% | 0.0005% |
| 2 | 0.02% | 0.0174% | 0.0024% | 0.0002% |
| 1 | 0.01% | 0.0087% | 0.0012% | 0.0001% |

¹ The taker fee matches the fee tier percentage

A *double-hop trade* such as SOL -> USDT -> ETH would pay a fee to trade SOL -> USDT and a further fee to trade USDT -> ETH.