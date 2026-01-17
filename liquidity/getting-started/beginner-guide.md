---
title: Beginner's Guide to Liquidity
description: Get started with liquidity provision on Orca - perfect for beginners.
icon: graduation-cap
---

Welcome to liquidity provision on Orca. This guide will walk you through everything you need to know to start earning fees by providing liquidity, even if you've never done it before.

## What is Liquidity Provision?

When you provide liquidity, you're depositing tokens into a pool that traders use to swap between assets. In return, you earn a portion of the trading fees.

**Simple example:**
- You deposit SOL and USDC into a pool
- Traders swap SOL for USDC (and vice versa) using your liquidity
- You earn a share of fees from every trade
- When you withdraw, you get your tokens back plus earned fees

## Why Provide Liquidity?

| Benefit | Description |
|---------|-------------|
| **Earn passive income** | Collect trading fees without active trading |
| **Put idle assets to work** | Earn yield on tokens you're holding anyway |
| **Support the ecosystem** | Help traders get better prices |
| **Flexible commitment** | Withdraw anytime (no lock-up periods) |

## Understanding Concentrated Liquidity

Orca uses **Concentrated Liquidity Market Makers (CLMMs)**, which let you focus your capital within a specific price range.

### Traditional vs. Concentrated Liquidity

**Traditional (CPMM):** Your liquidity is spread across all possible prices (0 to infinity)
- Simple to use
- Lower capital efficiency
- Lower fee earnings

**Concentrated (CLMM):** Your liquidity is focused in a price range you choose
- Higher capital efficiency
- Higher potential fee earnings
- Requires more decisions (choosing your range)

### What This Means for You

With concentrated liquidity:
- You earn fees **only when the price is within your range**
- Narrower ranges = higher fees but more management
- Wider ranges = lower fees but less management

Don't worry—we'll help you choose the right approach for your situation.

## Before You Start

### Prerequisites

1. **A Solana wallet** - We recommend [Phantom](https://phantom.app) or [Backpack](https://backpack.app)
2. **SOL for transaction fees** - Keep at least 0.1 SOL for fees
3. **Tokens to deposit** - You'll need both tokens in the pair (e.g., SOL and USDC)

### Important Concepts to Understand

**Impermanent Loss (IL)**
When token prices change, your position's value may differ from simply holding the tokens. This isn't always a "loss"—you're trading potential price gains for fee income.

**Trading fees**
Pools have different fee tiers (0.01%, 0.05%, 0.3%, 1%). Higher fees = more earnings per trade but potentially less trading volume.

## Choosing Your First Pool

### Recommended for Beginners

Start with these types of pools:

| Pool Type | Example | Why It's Good for Beginners |
|-----------|---------|----------------------------|
| **Stablecoin pairs** | USDC/USDT | Minimal impermanent loss, predictable |
| **Major token pairs** | SOL/USDC | High volume, consistent fees |
| **Full-range positions** | Any pair | Simpler, no range management needed |

### Pools to Avoid as a Beginner

- **Low-liquidity pools** - Harder to enter/exit, less predictable
- **New or meme tokens** - High volatility, higher risk
- **Exotic pairs** - More complex to understand

## Your First Liquidity Position

### Option 1: Full-Range Position (Simplest)

A full-range position spreads your liquidity across all prices—similar to traditional LP.

**Best for:**
- Complete beginners
- "Set and forget" approach
- Learning the basics

**Trade-off:** Lower fee earnings but minimal management

[Full-Range Position Guide →](/liquidity/getting-started/full-range)

### Option 2: Custom Range Position (More Efficient)

Choose a specific price range for your liquidity.

**Best for:**
- Users comfortable with some management
- Higher potential returns
- Specific market views

**Trade-off:** Higher fee earnings but requires monitoring

[Custom Range Position Guide →](/liquidity/getting-started/custom-range)

### Which Should You Choose?

```
Are you completely new to DeFi liquidity?
├── Yes → Start with Full-Range
└── No → Do you want to maximize returns?
    ├── Yes → Custom Range
    └── No → Full-Range is fine
```

## Step-by-Step: Opening Your First Position

### Step 1: Navigate to the Pool

1. Go to [orca.so](https://www.orca.so)
2. Connect your wallet
3. Click on **Pools** in the navigation
4. Search for your desired pair (e.g., "SOL/USDC")
5. Click on the pool to open it

### Step 2: Click "New Position"

1. On the pool page, click **New Position**
2. You'll see the position creation interface

### Step 3: Choose Your Range

**For Full-Range:**
- Click the **Full Range** button
- Your range will cover all prices

**For Custom Range:**
- Set your minimum price (lower bound)
- Set your maximum price (upper bound)
- Keep the current price within your range

### Step 4: Enter Your Deposit Amount

1. Enter the amount of one token
2. The other token amount will auto-calculate (for in-range positions)
3. Check you have sufficient balance

### Step 5: Review and Confirm

1. Review the position summary:
   - Tokens being deposited
   - Price range
   - Estimated fee tier
2. Click **Add Liquidity**
3. Approve the transaction in your wallet

### Step 6: You're Done!

Your position is now active and earning fees.

## After Opening Your Position

### Monitor Your Position

Check on your position regularly:
- Go to **Portfolio** to see all your positions
- Track fees earned
- Watch if price stays in your range

### Harvesting Fees

Fees accumulate in your position. To collect them:
1. Go to your position in Portfolio
2. Click **Harvest**
3. Approve the transaction

[Detailed Harvesting Guide →](/liquidity/manage/harvest)

### When to Adjust

Consider adjusting your position when:
- Price moves outside your range (you stop earning)
- You want to take profits
- Market conditions change significantly

## Common Beginner Questions

**What if the price moves outside my range?**

You stop earning fees, but your funds are safe. You can:
- Wait for price to return
- Close the position
- Open a new position at the current price

**Can I lose money?**

You won't lose your deposited tokens, but:
- Impermanent loss can reduce your position's value vs. holding
- Token prices can drop
- Fees earned may not always offset IL

**How much should I deposit?**

Start small while learning. There's no minimum, but consider:
- Transaction fees (keep enough SOL)
- Your comfort level
- Diversification (don't put everything in one position)

**How often should I check my position?**

Depends on your range:
- Full-range: Weekly or less often
- Tight custom range: Daily
- Wide custom range: Every few days

## Understanding Your Returns

### What You Earn

1. **Trading fees** - Your share of fees from trades
2. **Token rewards** - Some pools offer additional token incentives

### What Affects Your Earnings

| Factor | Impact |
|--------|--------|
| **Trading volume** | More trades = more fees |
| **Your range width** | Narrower = higher fee share when in range |
| **Time in range** | More time in range = more fees |
| **Pool fee tier** | Higher fee tier = more per trade |

## Risks to Understand

### Impermanent Loss

When prices change, your position rebalances. This can mean:
- Ending up with more of the token that dropped in price
- Less total value than if you'd just held the tokens

[Deep Dive: Impermanent Loss →](/liquidity/concepts/impermanent-loss)

### Smart Contract Risk

Your funds are held in smart contracts. While Orca is audited, no protocol is 100% risk-free.

### Price Risk

The tokens themselves can lose value regardless of LP performance.

## Next Steps

Now that you understand the basics:

1. **Open your first position** - [Full-Range Guide](/liquidity/getting-started/full-range) or [Custom Range Guide](/liquidity/getting-started/custom-range)
2. **Learn about fees** - [Understanding Trading Fees](/liquidity/concepts/trading-fees)
3. **Understand IL better** - [Impermanent Loss Explained](/liquidity/concepts/impermanent-loss)
4. **Manage your positions** - [Portfolio Management](/liquidity/manage/portfolio)

## Glossary

| Term | Definition |
|------|------------|
| **LP** | Liquidity Provider - someone who deposits into pools |
| **CLMM** | Concentrated Liquidity Market Maker |
| **Range** | The price bounds where your liquidity is active |
| **Fee tier** | The percentage fee charged on trades |
| **IL** | Impermanent Loss |
| **TVL** | Total Value Locked - total liquidity in a pool |
| **APR** | Annual Percentage Rate - estimated yearly return |
