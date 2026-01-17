---
title: xORCA Staking
description: Stake ORCA tokens to earn rewards and participate in governance.
icon: coins
---

xORCA is Orca's staking system that lets you earn rewards from protocol trading fees while participating in governance. When you stake ORCA, you receive xORCA—a token that grows in value over time.

## Quick Start

**Want to start earning? Here's the TL;DR:**

1. Go to [orca.so/stake](https://www.orca.so/stake)
2. Connect your wallet
3. Enter the amount of ORCA to stake
4. Confirm the transaction
5. Receive xORCA tokens that earn rewards automatically

*That's it! Your xORCA will increase in value over time as trading fees flow in.*

## Why Stake ORCA?

| Benefit | Description |
|---------|-------------|
| **Earn passive rewards** | 20% of protocol fees buy ORCA and increase xORCA value |
| **No active management** | Your rewards accumulate automatically |
| **Stay liquid** | xORCA is tradeable—you can sell or use it in DeFi |
| **Support governance** | xORCA holders influence protocol decisions |

## How xORCA Works

### The Simple Version

Think of xORCA like a savings account that earns interest:

1. **Deposit ORCA** → You receive xORCA tokens
2. **Trading happens** → Protocol earns fees
3. **Buybacks occur** → Fees buy ORCA, adding to the vault
4. **xORCA appreciates** → Your xORCA becomes worth more ORCA

**Key insight:** The amount of xORCA you hold stays the same, but each xORCA becomes redeemable for more ORCA over time.

### Example

Let's say you stake 1,000 ORCA when 1 xORCA = 1 ORCA:
- You receive 1,000 xORCA
- After a year of buybacks, 1 xORCA might = 1.05 ORCA
- Your 1,000 xORCA is now worth 1,050 ORCA

You didn't do anything—the value grew automatically.

## How to Stake

### Step 1: Navigate to Staking

Go to [orca.so/stake](https://www.orca.so/stake) and connect your wallet.

### Step 2: Enter Amount

1. Enter the amount of ORCA you want to stake
2. Review the current exchange rate
3. See how much xORCA you'll receive

### Step 3: Confirm

1. Click **Stake**
2. Approve the transaction in your wallet
3. Your xORCA appears in your wallet

### Step 4: You're Done!

Your xORCA will automatically increase in value as protocol fees accumulate.

## How to Unstake

Unstaking requires a **7-day cooldown period**:

### Step 1: Initiate Redemption

1. Go to [orca.so/stake](https://www.orca.so/stake)
2. Click **Unstake**
3. Enter the amount of xORCA to redeem
4. Confirm the transaction

### Step 2: Wait for Cooldown

- A 7-day timer begins
- Your redemption rate is locked at this moment
- You receive a "Claim Ticket" (an NFT representing your claim)

### Step 3: Withdraw

After 7 days:
1. Return to the staking page
2. Click **Withdraw**
3. Receive your ORCA

**Why the cooldown?** It ensures protocol stability and prevents gaming of the system around large buyback events.

## Where Do Rewards Come From?

### Fee Flow

```
Traders pay fees → 12% goes to protocol → 20% of that buys ORCA → ORCA added to vault
```

**In numbers:**
- Trading fee: 0.3% (example)
- Protocol share: 12% of 0.3% = 0.036%
- xORCA buybacks: 20% of 0.036% = 0.0072% of trade volume

### What This Means

When trading volume is high, more ORCA is bought and added to the vault, making your xORCA more valuable faster.

**Example day with $1B volume:**
- Total fees: ~$800,000
- Protocol share: ~$96,000
- Buybacks: ~$19,200 worth of ORCA

*Note: Actual returns vary with trading volume and ORCA price.*

## Important Considerations

### Benefits

- **Automatic compounding** - No need to claim and restake
- **Liquid token** - Use xORCA in DeFi or transfer it
- **Protocol-aligned** - You benefit when Orca succeeds
- **Simple** - Stake once, earn forever

### Considerations

- **7-day cooldown** - Plan ahead if you need liquidity
- **Variable returns** - Depends on trading volume
- **Price exposure** - xORCA value depends on ORCA price
- **Smart contract risk** - Funds are held in contracts (audited)

## xORCA vs. Holding ORCA

| Aspect | Holding ORCA | Staking for xORCA |
|--------|-------------|-------------------|
| **Rewards** | None | Yes, from fees |
| **Liquidity** | Instant | 7-day unstaking |
| **Governance** | Yes | Yes (enhanced) |
| **Complexity** | None | Minimal |
| **Best for** | Short-term holding | Long-term believers |

## Using xORCA

### In DeFi

xORCA is a standard SPL token. You can:
- Trade it on DEXs
- Use as collateral (where supported)
- Transfer to any wallet

### For Governance

xORCA provides voting power in Orca governance. Stakers can:
- Vote on proposals
- Delegate voting power
- Participate in discussions

## Technical Details

For those who want to understand the mechanics:

### Exchange Rate

The exchange rate determines how much ORCA each xORCA is worth:

```
Exchange Rate = ORCA in Vault / xORCA Supply
```

When buybacks add ORCA to the vault without minting new xORCA, the exchange rate increases.

### Key Addresses

| Account | Purpose |
|---------|---------|
| **xORCA Token** | `xorcaYqbXUNz3474ubUMJAdu2xgPsew3rUCe5ughT3N` |
| **Staking Program** | `StaKE6XNKVVhG8Qu9hDJBqCW3eRe7MDGLz17nJZetLT` |
| **ORCA Vault** | [View on Solscan](https://solscan.io/account/Ce5j11WAsSzM3nkzrw4Kw6v6ic3nbyqpv5eywjYKeKc5) |

### Governance & Security

- **Multisig control** - 3-of-5 signatures required for changes
- **Audited contracts** - Security reviewed
- **Emergency controls** - Pause capability for safety (withdrawals always available)

## Frequently Asked Questions

**How much will I earn?**

Returns depend on Orca trading volume. Higher volume = more buybacks = faster xORCA appreciation. Historical returns vary.

**Can I stake any amount?**

Yes, there's no minimum. However, consider transaction costs when staking very small amounts.

**What if ORCA price drops?**

Your xORCA will still increase in ORCA terms, but the USD value depends on ORCA's price. xORCA protects against missing out on staking rewards, not price drops.

**Is my xORCA safe?**

xORCA is held in your own wallet. The staking contracts are audited, but all DeFi carries smart contract risk.

**Can I transfer my xORCA?**

Yes, xORCA is a standard token. You can send it to any Solana wallet.

**What happens during the cooldown?**

Your redemption rate is locked when you initiate unstaking. You won't earn additional rewards during the 7-day wait.

## Next Steps

- [Stake ORCA](https://www.orca.so/stake) - Start earning now
- [Governance Overview](/governance/overview) - Learn about voting
- [How to Participate](/governance/participate) - Get involved
- [Governance FAQ](/governance/faq) - More questions answered
