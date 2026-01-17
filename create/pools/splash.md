---
title: Creating a Splash Pool
description: Create a Splash Pool for simple, cost-effective token launches.
icon: droplet
---

Splash Pools are Orca's streamlined pool creation option, designed for simplicity and cost-effectiveness. If you're launching a new token or want a straightforward liquidity pool, Splash Pools are the recommended choice.

## What Are Splash Pools?

Splash Pools are full-range liquidity pools built on Orca's CLMM infrastructure. They combine the simplicity of traditional AMMs with the benefits of Orca's efficient architecture.

### Splash Pools vs. CLMM Pools

| Feature | Splash Pool | CLMM Pool |
|---------|------------|-----------|
| **Position type** | Full-range only | Custom ranges available |
| **Setup cost** | Lower | Higher |
| **Complexity** | Simple | More advanced |
| **Management** | Minimal | More involved |
| **Tick array setup** | Automatic | Manual (for unlisted tokens) |
| **Best for** | New tokens, simple launches | Established tokens, LP optimization |

### When to Choose Splash Pools

✅ **Use Splash Pools when:**
- Launching a new token
- You want simplicity over optimization
- You prefer minimal ongoing management
- You're new to providing liquidity

❌ **Consider CLMM Pools when:**
- You want custom price ranges
- You need maximum capital efficiency
- Your token is already established
- You're an experienced LP

## How Splash Pools Work

### Full-Range Liquidity

Splash Pools use full-range positions:

- Liquidity spans all possible prices (0 to ∞)
- Always in range—never stops earning
- Similar to traditional AMM behavior
- Lower capital efficiency, but simpler

### Position NFTs

Like all Orca positions, Splash Pool positions are represented by NFTs:

- You receive an NFT representing your position
- The NFT proves ownership
- Fees must be manually harvested (not auto-compounded)

### Fee Earnings

LPs earn trading fees proportional to their share of the pool:

- Fees accumulate in your position
- Harvest anytime through the UI
- No auto-compounding (unlike some traditional AMMs)

## Creating a Splash Pool

### Prerequisites

Before you start:

1. **Both tokens** - Have both tokens in your wallet
2. **SOL for fees** - Keep at least 0.1 SOL
3. **Initial price** - Know your token's starting price
4. **Token metadata** - Name, symbol, and logo ready

### Step-by-Step Guide

#### Step 1: Navigate to Pool Creation

1. Go to [orca.so/create-pool](https://www.orca.so/create-pool)
2. Connect your wallet
3. Click **Create Splash Pool**

#### Step 2: Select Your Token

1. Click **Select Token**
2. Enter your token's name, symbol, or mint address
3. Your token appears in the selector

**Default pairing:** Your token pairs with SOL by default.

**Custom pairing:** Click the SOL label to select a different quote token.

#### Step 3: Set Initial Price

Enter the starting price for your token:

**Option A: Use Estimated Price**
- Orca shows an estimated market price from Jupiter
- Click to auto-fill (if available)
- Verify it matches your expectations

**Option B: Enter Custom Price**
- Type your desired price manually
- Required for new tokens without market data

⚠️ **Critical:** The initial price determines where trading starts. Setting the wrong price results in immediate arbitrage against your pool. Double-check before confirming.

#### Step 4: Enter Deposit Amount

1. Enter the amount for one token
2. The other amount auto-calculates
3. Verify you have sufficient balance

**Tip:** For new tokens, consider how much liquidity you want to provide. More liquidity = better trading experience = more adoption.

#### Step 5: Preview and Confirm

1. Click **Preview Pool**
2. Review all parameters:
   - Token pair
   - Initial price
   - Deposit amounts
3. Read the warning message carefully
4. Check the acknowledgment box
5. Click **Create Pool**

#### Step 6: Approve Transactions

1. Approve the first transaction (pool initialization)
2. Approve the second transaction (liquidity deposit)
3. Wait for confirmations

#### Step 7: Pool Activation

After creation:

- Pool appears in the Orca UI
- **Trade** and **Provide Liquidity** buttons start grayed out
- Once indexed, buttons become active
- Your token is now tradeable on Orca

## After Creating Your Pool

### Verify Your Pool

1. Search for your token on [orca.so](https://www.orca.so)
2. Confirm the pool appears in search
3. Test with a small swap

### Token List Warning

If your token shows a warning triangle (⚠️):

- Token is not on the Orca Token List
- Trading still works
- Consider [requesting listing](/create/listings/token-list) for better UX

### Add Rewards (Optional)

Incentivize more liquidity providers:

- Attract additional LPs with token rewards
- Deeper liquidity = better trading experience
- [Learn about adding rewards](/create/rewards/overview)

## Managing Your Splash Pool Position

### Monitoring

- Check your position at [orca.so/portfolio](https://www.orca.so/portfolio)
- Track accumulated fees
- Monitor trading volume

### Harvesting Fees

To collect earned fees:

1. Go to Portfolio
2. Find your Splash Pool position
3. Click **Harvest**
4. Approve the transaction

### Adding More Liquidity

To increase your position:

1. Go to the pool page
2. Click **Add Liquidity**
3. Enter additional amounts
4. Approve the transaction

### Withdrawing

To reduce or close your position:

1. Go to Portfolio
2. Find your position
3. Click **Withdraw**
4. Enter amount (or full withdrawal)
5. Approve the transaction

## Best Practices

### Setting Initial Price

1. **Market price exists?** → Match it closely
2. **New token?** → Set based on your tokenomics
3. **Always verify** → Price cannot be changed after creation

### Initial Liquidity Amount

Consider:

| Liquidity Level | Trade Quality | Typical For |
|----------------|---------------|-------------|
| **< $1,000** | High slippage | Testing only |
| **$1,000 - $10,000** | Moderate slippage | Small launches |
| **$10,000 - $100,000** | Good trading | Standard launches |
| **> $100,000** | Excellent trading | Major launches |

### Growing Your Pool

1. **Get listed** - [Submit to Orca Token List](/create/listings/token-list)
2. **Add rewards** - [Incentivize LPs](/create/rewards/overview)
3. **External listings** - [CoinGecko](/create/listings/coingecko), [Jupiter](/create/listings/jupiter)
4. **Promote** - Share on social media

## Troubleshooting

### Pool Not Showing

- Wait a few minutes for indexing
- Refresh the page
- Clear browser cache
- Verify transaction succeeded on Solscan

### Transaction Failed

- Check SOL balance for fees
- Try again (network issues)
- Verify token amounts

### Wrong Initial Price

If you set the wrong price:

- Arbitrageurs will correct it (costing you money)
- You cannot edit the price directly
- Consider creating a new pool with correct price
- Remove liquidity from the incorrectly priced pool

## Frequently Asked Questions

**What fees do Splash Pools charge?**

Splash Pools use a standard fee tier. The exact fee depends on pool configuration.

**Can I convert a Splash Pool to a CLMM pool?**

No, but you can create a separate CLMM pool for the same pair and migrate liquidity.

**Why use Splash over CLMM for new tokens?**

Simpler setup, lower cost, automatic tick array handling, and appropriate for unknown price ranges.

**Can others add liquidity to my Splash Pool?**

Yes, anyone can add liquidity to any pool on Orca.

**Do I earn fees from others' swaps?**

Yes, your fee share is proportional to your liquidity share.

## Related Resources

- [CLMM Pools](/create/pools/clmm) - Advanced pool creation
- [Token Extensions](/create/pools/extensions) - SPL Token Extension support
- [Adding Rewards](/create/rewards/overview) - Incentivize LPs
- [Token List](/create/listings/token-list) - Improve discoverability
- [Beginner LP Guide](/liquidity/getting-started/beginner-guide) - Understand liquidity provision
