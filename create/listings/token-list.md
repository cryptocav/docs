---
title: Orca Token List
description: How to add your token to the Orca Token List for better discoverability.
icon: list-check
---

Adding your token to the Orca Token List improves discoverability and user experience. Tokens on the list display with proper names, symbols, and logos throughout the Orca interface.

## Why Add Your Token?

| Benefit | Description |
|---------|-------------|
| **Better UX** | Your token shows with name and logo instead of just an address |
| **Discoverability** | Users can find your token by searching its name or symbol |
| **Trust signals** | Listed tokens appear more established to users |
| **Trading volume** | Easier discovery often leads to more trading activity |

## Requirements

Before submitting your token for listing, ensure you meet these requirements:

### Mandatory Requirements

- **Active liquidity pool** - Your token must have an existing pool on Orca
- **Sufficient liquidity** - Pool should have meaningful TVL (recommended: $10,000+)
- **Valid token metadata** - Name, symbol, and logo properly configured on-chain
- **Working logo URL** - Logo must be accessible via HTTPS

### Token Metadata Standards

Your token should have:

| Field | Requirements |
|-------|-------------|
| **Name** | Clear, non-misleading name (max 32 characters) |
| **Symbol** | Unique ticker symbol (max 10 characters) |
| **Logo** | Square image, minimum 128x128px, PNG or SVG format |
| **Decimals** | Properly configured decimal places |

### What Won't Be Listed

Orca reserves the right to decline tokens that:

- Impersonate other projects or tokens
- Have misleading names or symbols
- Are associated with scams or rug pulls
- Violate intellectual property rights
- Have no legitimate use case

## How to Submit

### Option 1: During Pool Creation

When creating a new pool through Orca:

1. Complete the pool creation process
2. You'll be prompted to submit token metadata
3. Fill in the required information
4. Submit for review

### Option 2: For Existing Pools

If your token already has a pool but isn't listed:

**Step 1: Prepare Your Information**

Gather the following:
- Token mint address
- Token name and symbol
- Logo URL (must be HTTPS)
- Pool address on Orca
- Project website
- Social links (Twitter, Discord, etc.)

**Step 2: Submit a Request**

Submit your listing request through one of these channels:

1. **Support Ticket** - Use the Support function in the Orca app wallet menu
2. **Discord** - Open a ticket in the [Orca Discord](https://discord.gg/orca-so) support channel
3. **Direct Contact** - If you have existing communication channels with the Orca team

**Step 3: Provide Required Details**

In your submission, include:

```
Token Name: [Your Token Name]
Token Symbol: [SYMBOL]
Mint Address: [Solana address]
Pool Address: [Orca pool address]
Logo URL: [https://...]
Website: [https://...]
Twitter: [@handle]
Discord: [invite link]
Brief Description: [1-2 sentences about your project]
```

### Step 4: Wait for Review

The Orca team will review your submission:

- **Review timeline:** Typically 3-7 business days
- **You may be contacted** for additional information
- **Approval notification** will be sent once listed

## After Listing

Once your token is listed:

### Verify the Listing

1. Go to [orca.so](https://www.orca.so)
2. Search for your token by name or symbol
3. Verify logo and name display correctly

### Update Token Information

If you need to update your token's information after listing:

1. Submit a new request through the same channels
2. Specify what needs to be updated
3. Provide the updated information (e.g., new logo URL)

## Listing on External Platforms

For broader ecosystem visibility, also consider listing on:

### CoinGecko

CoinGecko provides price tracking and market data:

- [CoinGecko Listing Guide](/create/listings/coingecko)
- Adds price charts and market cap data
- Improves credibility

### Jupiter Strict List

Jupiter is the primary Solana DEX aggregator:

- [Jupiter Listing Guide](/create/listings/jupiter)
- Increases trading accessibility
- Aggregates liquidity across DEXs

## Frequently Asked Questions

**How long does listing take?**

Typically 3-7 business days, but may vary based on review queue and completeness of your submission.

**Is there a fee for listing?**

There is no fee for standard token list submissions.

**My token was rejected. What can I do?**

Review the rejection reason, address any issues, and resubmit. Common issues include:
- Insufficient liquidity
- Missing or broken logo URL
- Incomplete information

**Can I list multiple tokens?**

Yes, submit separate requests for each token.

**Do I need to be listed to create a pool?**

No. Anyone can create pools for any valid SPL token. Listing improves discoverability but isn't required for pool creation.

**My logo isn't showing correctly. What should I do?**

Verify:
- Logo URL is accessible via HTTPS
- Image is square (1:1 aspect ratio)
- File format is PNG or SVG
- Image is at least 128x128 pixels

## Best Practices

### Before Submitting

1. **Test your pool** - Ensure swaps work correctly
2. **Verify metadata** - Double-check all token information
3. **Test logo URL** - Open it in a browser to confirm it loads
4. **Build liquidity** - More liquidity increases approval chances

### For Better Visibility

1. **Announce your listing** - Share on social media when listed
2. **Encourage trading** - Active pools maintain visibility
3. **Maintain liquidity** - Keep sufficient liquidity in your pools
4. **Engage community** - Active projects get more attention

## Related Resources

- [Creating a Splash Pool](/create/pools/splash) - Launch pools for new tokens
- [Creating a CLMM Pool](/create/pools/clmm) - Advanced pool creation
- [Adding Rewards](/create/rewards/overview) - Incentivize liquidity providers
- [CoinGecko Listing](/create/listings/coingecko) - External listing guide
- [Jupiter Listing](/create/listings/jupiter) - DEX aggregator listing
