---
title: Managing Your Portfolio
description: Monitor and manage your liquidity positions on Orca.
icon: chart-pie
---

The Portfolio page is your command center for managing liquidity positions on Orca. Here you can view all your positions, track performance, harvest fees, and make adjustments.

## Accessing Your Portfolio

1. Go to [orca.so/portfolio](https://www.orca.so/portfolio)
2. Connect your wallet
3. Your positions load automatically

## Portfolio Overview

### What You'll See

The Portfolio page displays:

| Section | Information |
|---------|-------------|
| **Total Value** | Combined value of all positions |
| **Positions List** | All your active liquidity positions |
| **Unclaimed Fees** | Fees ready to harvest |
| **Position Details** | Individual position information |

### Position Cards

Each position shows:

- **Token pair** - Which tokens you're providing liquidity for
- **Current value** - USD value of your position
- **Price range** - Your selected min/max prices
- **In range status** - Whether you're currently earning fees
- **Unclaimed fees** - Accumulated fees to harvest
- **Fee APR** - Current estimated annual return

## Understanding Position Status

### In Range (Earning)

Your position is **in range** when the current price is within your selected bounds:

- ✅ You're earning trading fees
- The position indicator shows green
- Continue monitoring normally

### Out of Range (Not Earning)

Your position is **out of range** when price moves outside your bounds:

- ⚠️ You're not earning fees
- The position indicator shows yellow/red
- Consider rebalancing or waiting for price to return

## Position Management Actions

### Viewing Details

Click on any position to expand and see:

- Detailed token balances
- Price range visualization
- Fee breakdown
- Performance history
- Available actions

### Harvesting Fees

To collect accumulated fees:

1. Click on the position
2. Click **Harvest** (or **Collect Fees**)
3. Approve the transaction
4. Fees transfer to your wallet

[Detailed Harvest Guide →](/liquidity/manage/harvest)

### Adding Liquidity

To increase your position:

1. Click on the position
2. Click **Add Liquidity**
3. Enter the amount to add
4. Approve the transaction

[Adding Liquidity Guide →](/liquidity/manage/add)

### Withdrawing Liquidity

To reduce or close your position:

1. Click on the position
2. Click **Withdraw** or **Close Position**
3. Enter the amount (or select full withdrawal)
4. Approve the transaction

[Withdrawal Guide →](/liquidity/manage/withdraw)

## Position Sidebar

For quick access to common actions, use the Position Sidebar:

- Quick harvest
- Rapid adjustments
- Position switching

[Position Sidebar Guide →](/liquidity/manage/sidebar)

## Understanding Position NFTs

### What Are Position NFTs?

Your liquidity positions are represented by NFTs:

- Each position = one unique NFT in your wallet
- The NFT proves ownership of the position
- Whoever holds the NFT controls the position

### Important Warnings

⚠️ **Do NOT burn or transfer position NFTs carelessly**

- Sending the NFT transfers the entire position
- Burning the NFT = permanent loss of position and funds
- Keep NFTs in your primary wallet unless intentionally transferring

### Transferring Positions

If you want to move a position to another wallet:

1. Simply transfer the position NFT
2. The new wallet can now manage the position
3. The original wallet loses access

This is useful for:
- Moving to a hardware wallet
- Transferring to a multisig
- Selling positions (advanced)

## Tracking Performance

### Metrics to Watch

| Metric | What It Tells You |
|--------|------------------|
| **Position Value** | Current worth of deposited tokens |
| **Fees Earned** | Total fees collected over time |
| **Fee APR** | Annualized return from fees |
| **Time in Range** | How long you've been earning |
| **Impermanent Loss** | Value change vs. holding |

### Calculating Real Returns

Your actual return = Fees Earned - Impermanent Loss

Even if IL is positive (you gained), fees add to returns.
If IL is negative (you lost value), fees may offset it.

## Best Practices

### Regular Monitoring

- **Check weekly** for full-range positions
- **Check daily** for tight custom ranges
- **Set alerts** for automated notifications

[Setting Up Alerts →](/liquidity/manage/alerts)

### Harvest Timing

Consider harvesting:
- When fees reach a meaningful amount
- Before making any position changes
- For tax tracking purposes

### When to Adjust

Consider adjusting positions when:
- Out of range for extended periods
- Market conditions change significantly
- Better opportunities emerge
- You want to realize gains/losses

## Troubleshooting

### Position Not Showing

1. **Check wallet connection** - Reconnect if needed
2. **Refresh the page** - Wait for data to load
3. **Verify correct wallet** - Ensure you're using the right address
4. **Check NFT ownership** - Position NFT must be in connected wallet

### Incorrect Values Displayed

1. **Refresh the page** - Prices update in real-time
2. **Check network status** - Solana RPC issues can cause delays
3. **Clear cache** - Browser cache may show stale data

### Can't Interact with Position

1. **Verify NFT ownership** - Must be in connected wallet
2. **Check SOL balance** - Need SOL for transaction fees
3. **Try again** - Network congestion can cause failures

## Security Tips

### Protecting Your Positions

1. **Never share position NFTs** unless intentionally transferring
2. **Use hardware wallets** for large positions
3. **Verify transactions** before approving
4. **Beware of scams** asking you to transfer NFTs

### Safe Practices

- Bookmark orca.so directly
- Don't click links from DMs
- Verify you're on the real Orca site
- Review all transactions carefully

## Related Resources

- [Position Sidebar Guide](/liquidity/manage/sidebar) - Quick actions
- [Harvesting Yield](/liquidity/manage/harvest) - Collecting fees
- [Adding Liquidity](/liquidity/manage/add) - Increasing positions
- [Withdrawing](/liquidity/manage/withdraw) - Reducing positions
- [Closing Positions](/liquidity/manage/close) - Full withdrawal
- [Creating Alerts](/liquidity/manage/alerts) - Automated monitoring
