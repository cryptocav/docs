---
title: Creating a CLMM Pool
description: Create a concentrated liquidity pool with full customization options.
icon: chart-mixed
---

CLMM (Concentrated Liquidity Market Maker) pools give you complete control over your pool's configuration. This guide walks you through creating a CLMM pool on Orca.

## Should You Create a CLMM Pool?

Before proceeding, consider which pool type fits your needs:

| Feature | Splash Pool | CLMM Pool |
|---------|------------|-----------|
| **Setup complexity** | Simple | More complex |
| **Cost** | Lower | Higher |
| **Position types** | Full-range only | Custom ranges |
| **Management** | Minimal | More involved |
| **Best for** | New tokens, simple launches | Established tokens, advanced users |

**Recommendation:** If you're launching a new token and want simplicity, start with a [Splash Pool](/create/pools/splash). CLMM pools are better suited for established tokens or when you need custom range positions.

## Prerequisites

Before creating a pool:

1. **Have both tokens** - Your wallet needs both tokens in the pair
2. **Have SOL for fees** - Keep 0.1+ SOL for transaction fees
3. **Know your initial price** - Decide the starting price for your token
4. **Choose a fee tier** - Select based on expected volatility

### Understanding Fee Tiers

| Fee Tier | Best For | Examples |
|----------|----------|----------|
| **0.01%** | Stablecoin pairs | USDC/USDT |
| **0.05%** | Stable, high-volume pairs | Major stablecoins |
| **0.30%** | Standard pairs | SOL/USDC |
| **1.00%** | Volatile/exotic pairs | Memecoins, new tokens |

Higher fees compensate LPs for volatility risk but may reduce trading volume.

## Creating a CLMM Pool

### Step 1: Navigate to Pool Creation

1. Go to [orca.so/create-pool](https://www.orca.so/create-pool)
2. Connect your wallet
3. Select **Create Concentrated Pool**

### Step 2: Select Your Tokens

1. Click **Select Token** to choose your token
2. Search by name, symbol, or paste the mint address
3. By default, your token pairs with SOL
4. (Optional) Click the SOL label to pair with a different token

### Step 3: Set the Initial Price

This is the starting trading price for your pool.

**Option A: Use Estimated Market Price**
- Orca shows an estimated price from Jupiter
- Click to use this price
- Verify it matches your expectations

**Option B: Enter Custom Price**
- Type your desired price in the Initial Price field
- Useful for new tokens without market data

**Important:** The initial price determines where trading begins. Setting the wrong price can result in immediate arbitrage against your pool.

### Step 4: Choose Your Position Type

#### Full-Range Position

Creates liquidity across all possible prices:

1. Click **Full Range**
2. Your range covers $0 to infinity
3. Similar to traditional AMM behavior

**Pros:** Simpler, always in range
**Cons:** Lower capital efficiency

#### Custom Range Position

Focus liquidity in a specific price range:

1. Select **Custom Range**
2. Set your **Min Price** (lower bound)
3. Set your **Max Price** (upper bound)
4. Use +/- buttons for fine adjustments

**Pros:** Higher capital efficiency when in range
**Cons:** Requires monitoring and management

### Step 5: Enter Deposit Amount

1. Enter the amount for one token
2. The other amount auto-calculates based on:
   - Your price range
   - Current price
   - Pool ratio

**Note:** For custom ranges not including the current price, you may deposit only one token.

### Step 6: Select Fee Tier

1. Click **Change** if you want a different fee tier
2. Select from available tiers
3. Consider your token's volatility

### Step 7: Review and Create

1. Click **Preview Pool**
2. Review all parameters carefully:
   - Token pair
   - Initial price
   - Price range (if custom)
   - Deposit amounts
   - Fee tier
3. Read the confirmation message
4. Check the acknowledgment box
5. Click **Create Pool**

### Step 8: Approve Transactions

1. You'll need to approve **two transactions**
2. First transaction initializes the pool
3. Second transaction deposits liquidity
4. Wait for confirmation

### Step 9: Pool Activation

After creation:
- The pool appears in the UI
- **Trade** and **Provide Liquidity** buttons are initially grayed out
- Once fully indexed, buttons become active
- Other users can then trade and provide liquidity

## After Creating Your Pool

### Verify Your Pool

1. Search for your token on [orca.so](https://www.orca.so)
2. Confirm the pool appears
3. Test with a small swap

### Token List

If your token shows a warning triangle:
- It's not yet on the Orca Token List
- Trading still works, but display is limited
- [Request token list addition](/create/listings/token-list)

### Add Rewards (Optional)

Incentivize more LPs with token rewards:
- [How to Add Rewards](/create/rewards/overview)

### Monitor Your Pool

Use these tools:
- [Orca Portfolio](https://www.orca.so/portfolio) - Track your positions
- [Account Microscope](https://everlastingsong.github.io/account-microscope/) - View pool state and tick arrays

## Advanced: Tick Arrays

CLMM pools use tick arrays to track liquidity at different price points. For unlisted tokens:

- Some tick arrays may need initialization
- Creating positions at different prices initializes arrays
- Splash Pools handle this automatically

If you encounter issues, reach out on [Discord](https://discord.gg/orca-so).

## Troubleshooting

### "Insufficient Balance"

- Ensure you have enough of both tokens
- Keep extra SOL for transaction fees

### "Transaction Failed"

- Try increasing slippage tolerance
- Ensure sufficient SOL for fees
- Try again—network congestion can cause failures

### Pool Not Showing in UI

- Wait a few minutes for indexing
- Refresh the page
- Clear browser cache if needed

### Price Immediately Changes After Creation

This usually means:
- Initial price was different from market price
- Arbitrageurs corrected the price
- Double-check your price setting next time

## Best Practices

### Setting Initial Price

1. **Check market price** - If your token trades elsewhere, match that price
2. **New tokens** - Set based on your tokenomics and launch plan
3. **Verify before confirming** - Price cannot be edited after creation

### Choosing Fee Tier

- Higher volatility → Higher fee tier
- Higher competition → Lower fee tier might attract more volume
- When in doubt, 0.30% is a reasonable default

### Managing Your Pool

- Monitor liquidity levels
- Watch for price movements out of range
- Consider adding rewards to attract more LPs

## Related Resources

- [Splash Pools](/create/pools/splash) - Simpler pool creation
- [Token Extensions](/create/pools/extensions) - SPL Token Extension support
- [Adding Rewards](/create/rewards/overview) - Incentivize liquidity
- [Token List](/create/listings/token-list) - Improve discoverability
- [Beginner LP Guide](/liquidity/getting-started/beginner-guide) - Understand liquidity provision
