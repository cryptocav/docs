---
title: Adding Pool Rewards
description: Incentivize liquidity providers with token rewards on your pool.
icon: gift
---

Reward programs incentivize liquidity providers (LPs) to deposit into your pool. By distributing tokens to LPs, you can attract more liquidity, improve trading depth, and grow your token's ecosystem.

## How Rewards Work

When you add rewards to a pool:

1. You provide tokens to be distributed over a set period
2. LPs who provide liquidity earn a share of rewards
3. Rewards are distributed proportionally based on liquidity provided
4. LPs claim rewards alongside their trading fees

## Benefits of Adding Rewards

| Benefit | Description |
|---------|-------------|
| **Attract liquidity** | More LPs means deeper liquidity |
| **Reduce slippage** | More liquidity = better prices for traders |
| **Build community** | Reward early supporters and believers |
| **Bootstrap growth** | Kickstart trading activity for new tokens |

## Prerequisites

Before adding rewards, you need:

1. **An existing pool** - Rewards are added to existing pools
2. **Reward tokens** - The tokens you'll distribute
3. **Token on Orca Token List** - Required for reward setup
4. **Contact with Orca** - Rewards require coordination

## Process Overview

Adding rewards involves coordination with Orca. Here's the general flow:

```
1. Prepare → 2. Contact Orca → 3. Confirm details → 4. Transfer tokens → 5. Rewards go live
```

## Step-by-Step Guide

### Step 1: Prepare Your Information

Gather the following details:

| Information | Description |
|-------------|-------------|
| **Pool address** | The Orca pool you want to incentivize |
| **Reward token** | The token you'll distribute |
| **Total amount** | How many tokens to distribute |
| **Duration** | How long the reward program runs |
| **Start date** | When rewards should begin |

### Step 2: Ensure Token List Status

Your token must be on the Orca Token List:

- **Already listed?** → Proceed to Step 3
- **Not listed?** → [Request listing first](/create/listings/token-list)

Note: Include your contact details in the listing request so Orca can follow up about rewards.

### Step 3: Contact Orca

Reach out through one of these channels:

1. **In-App Support** - Use the Support button in the wallet menu
2. **Discord** - Open a ticket in [#support-ticket](https://discord.gg/orca-so)
3. **Existing channels** - If you have direct contact with Orca team

**Include in your message:**

```
Subject: Reward Program Request

Pool: [pool address or token pair]
Reward Token: [token name and address]
Amount: [total tokens to distribute]
Duration: [e.g., 30 days, 90 days]
Preferred Start: [date]
Contact: [your preferred contact method]
```

### Step 4: Await Confirmation

The Orca team will:

1. **Review feasibility** - Confirm the rewards can be accommodated
2. **Provide transfer details** - Send the address for reward tokens
3. **Confirm timing** - Agree on start date and duration

**Expected timeline:** 3-7 business days for initial response

### Step 5: Transfer Reward Tokens

Once confirmed:

1. Transfer tokens to the address Orca provides
2. Send the transaction signature to Orca
3. Confirm the transfer was received

### Step 6: Rewards Go Live

After Orca activates rewards:

1. The pool displays reward APR in the UI
2. LPs start earning rewards immediately
3. Rewards distribute continuously over the set duration

## Reward Parameters

### Duration Options

Common reward durations:

| Duration | Best For |
|----------|----------|
| **14 days** | Short promotional campaigns |
| **30 days** | Standard reward programs |
| **90 days** | Long-term liquidity building |
| **Custom** | Discuss with Orca team |

### Distribution Method

Rewards distribute:

- **Continuously** - Not in discrete chunks
- **Proportionally** - Based on LP position size and time
- **Within range** - Only in-range liquidity earns rewards

### Claiming Rewards

LPs claim rewards:

- Through the Orca UI alongside fees
- At any time (no lock-up)
- Using the Harvest function

## Scenarios

### New Pool, New Token

1. Create your pool ([Splash](/create/pools/splash) or [CLMM](/create/pools/clmm))
2. [Get your token listed](/create/listings/token-list)
3. Contact Orca about rewards (include listing request)
4. Transfer tokens and launch rewards

### Existing Pool, Listed Token

1. Contact Orca with pool details
2. Confirm program parameters
3. Transfer tokens
4. Rewards activate

### Extending an Existing Program

1. Contact Orca before current program ends
2. Provide additional tokens
3. Program extends seamlessly

## Best Practices

### Setting Reward Amounts

Consider:

- **Target APR** - What yield attracts LPs?
- **Pool TVL goals** - How much liquidity do you need?
- **Budget** - What can you sustainably distribute?
- **Competition** - What are similar pools offering?

### Timing Your Program

- **Launch timing** - Coordinate with marketing/announcements
- **Duration** - Longer programs build more sustainable liquidity
- **Renewals** - Plan ahead to avoid gaps

### Maximizing Impact

1. **Announce your program** - Share on social media
2. **Provide context** - Explain why you're incentivizing
3. **Engage LPs** - Build community around your pool
4. **Monitor performance** - Track TVL and trading volume

## Costs

- **Reward tokens** - You provide the tokens to distribute
- **Setup** - No fee for standard reward programs
- **Platform fees** - Standard Orca protocol fees apply to trades

## Frequently Asked Questions

**Can I add multiple reward tokens?**

Yes, pools can have multiple reward tokens. Contact Orca to set up additional rewards.

**Can I cancel a reward program early?**

Generally, no. Commit to amounts you're comfortable distributing. Discuss edge cases with Orca.

**How are rewards displayed to LPs?**

LPs see estimated APR based on current reward rate and pool TVL.

**What if no one provides liquidity?**

Rewards still distribute. Higher rewards per LP incentivizes deposits.

**Can I reward a pool I didn't create?**

Yes, you can add rewards to any existing Orca pool.

## Related Resources

- [Creating a Splash Pool](/create/pools/splash) - Simple pool creation
- [Creating a CLMM Pool](/create/pools/clmm) - Advanced pool creation
- [Token List](/create/listings/token-list) - Required for rewards
- [Harvesting Yield](/liquidity/manage/harvest) - How LPs claim rewards
