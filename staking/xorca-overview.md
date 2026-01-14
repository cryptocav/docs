---
title: xORCA Staking & Governance
description: Stake ORCA tokens and earn protocol rewards with xORCA.
icon: landmark
---

**xORCA aligns the interests of ORCA tokenholders with the protocol's success by sharing rewards funded by protocol trading fees via a liquid staking mechanism.** It strengthens the case for long-term holding, backed by protocol fees from the leading DEX on Solana with proven product-market fit.

### Basics of xORCA

![](/images/image_122.jpg)

**Staking Site**: <https://www.orca.so/stake>

**How it works**

* Stake your ORCA → receive xORCA, a tradable SPL token that grows in value over time (similar to a Liquid Staking Token)
* SPL Token Address : `xorcaYqbXUNz3474ubUMJAdu2xgPsew3rUCe5ughT3N`  (view on [Solscan](https://solscan.io/token/xorcaYqbXUNz3474ubUMJAdu2xgPsew3rUCe5ughT3N))

* xORCA Staking Program ID: `StaKE6XNKVVhG8Qu9hDJBqCW3eRe7MDGLz17nJZetLT` (view on [Solscan](https://solscan.io/token/xorcaYqbXUNz3474ubUMJAdu2xgPsew3rUCe5ughT3N))

**The Mechanics**

* 20% of Whirlpool [protocol fees](/reference/useful-information/trading-fees) are used to buy ORCA on the open market
* Purchased ORCA is deposited into the *xORCA staking vault,* increasing the ORCA/xORCA exchange rate
* This means each xORCA gradually becomes redeemable for more ORCA — without you doing anything

**Unstaking Process**

* To unstake: users redeem xORCA → wait for expiration of 7-day cooldown → Withdraw ORCA

**Governance**

* Governance and upgrade authority are controlled by a 3-of-5 multisig (requiring 3 signatures out of 5 signers)

### How xORCA Works

xORCA is a liquid staking token for staked ORCA.

* Your ORCA is deposited into a vault
* You receive xORCA tokens that represent a pro-rata claim on the vault. xORCA is a liquid token that can be used across Solana just like any other SPL token

* Buybacks add more ORCA into the vault but do not mint new xORCA, the exchange rate between xORCA and ORCA rises

> 1 xORCA redeems for more ORCA over time.

### Vault Mechanics

**Exchange rate (ER)**: Determines how much ORCA each xORCA can be redeemed for

![](/images/image_123.jpg)

**Buybacks**: When ΔORCA is deposited without new xORCA minted:

![](/images/image_124.jpg)

* **Outcome**: All existing xORCA become more valuable in terms of ORCA.
* **Why it matters**: Buybacks increase the value of each token

**Staking deposits**: When depositing ORCA, new xORCA are minted increasing both vault balance and supply proportionally

* **Outcome**: Exchange Rate (ER) remains unchanged
* **Why it matters**: Staking is neutral — it allows new users to enter without diluting existing holders

### Staking Lifecycle

#### Deposit

* Stake: User deposits ORCA
* Mint: program mints xORCA
* Receipt: xORCA transferred to users wallet

#### Redemption

* Redemption: user redeems xORCA → program burns xORCA and creates Claim Ticket
* Cooldown: 7-day cooldown elapses
* Withdraw: redeem Claim Ticket for ORCA

#### Redemption rate snapshot

A snapshot of the exchange rate is taken at the moment xORCA is burned and a *Claim Ticket* issued

![](/images/image_125.jpg)

#### Supply

* Initial xORCA supply: 0
* xORCA is a standard SPL token, fully transferable, composable, and DeFi ready - just like a Liquid Staking Token (LST)

#### Buybacks

* **Source**: 20% of protocol fees. With a 12% protocol fee share, this equals 2.4% of total trading fees
* **Execution**: Program purchases ORCA on the open market, deposits into vault

#### Key Acount Address

* **ORCA Vault (Orca ATA):** [[link](https://solscan.io/account/Ce5j11WAsSzM3nkzrw4Kw6v6ic3nbyqpv5eywjYKeKc5)] - The ATA in our wallet that actually holds all the ORCA
* **xORCA State Account:** [[link](https://solscan.io/account/CSqKhyW1cpdyjheAx5HXx4ibcnYrzpL5JywEMAkZixBK)] - The "wallet" that the xORCA program owns to store ORCA tokens
* **Pre-launch ORCA buyback wallet**: [J4Y2ryHy32uiBNksCQ65Ati2euAUQWgd5UHU31oRtncS](https://solscan.io/account/J4Y2ryHy32uiBNksCQ65Ati2euAUQWgd5UHU31oRtncS)—this balance will be added to the xORCA vault in the future, details will be confirmed soon

### Source of Staking Rewards

#### Fee Flow

Traders pay fees when they trade on Orca. Here's how those fees flow to xORCA holders:

* 12% of those fees go to the protocol
* 20% of that protocol share is used to buy ORCA—this equals 2.4% of total trade fees
* The purchased ORCA goes into the vault → raising the value of xORCA

Note : Vault inflows depend on the execution price of ORCA

#### Exchange-Rate Growth

The value of each xORCA depends on the ratio between:

* ORCA in the vault
* xORCA in circulation

Mathematically this can be expressed with this formula:

![](/images/image_126.jpg)

* ER = Exchange Rate
* Valut ORCA = # of ORCA in valut

* xORCA Supply = Total amount of xORCA in circulation

When buybacks add ORCA to the vault, the exchange rate increases even though no new xORCA is created.

**Formula for a buyback:**

![](/images/image_127.jpg)

* B = ORCA added from buybacks
* S = xORCA supply

**What This Means For Stakers**

* Every buyback makes each xORCA redeemable for more ORCA
* New stakers don’t dilute existing holders, because xORCA is only minted when ORCA is deposited

* Over time, the exchange rate grows steadily, so your xORCA balance becomes more valuable without you doing anything

**Example (24 Hours, Illustrative)**

* Volume: $1,000,000,000
* Total fees: $800,000

* Buybacks: $19,200
* At $2.00/ORCA → 9,600 ORCA purchased

* If supply = 10,000,000 xORCA and ER\_old = 1.0000 → ER\_new = 1.00096

Note: Yields vary with trading volume and prices. Past performance is not indicative of future returns.

### Governance & Administration

* Multisig (3-of-5): Manages upgrade authority, parameter changes, and pause controls.

**Authorities**

* Upgrade authority: Multisig
* xORCA mint authority: program PDA

* Vault authority: program PDA

**Emergency controls**

The multisig has the ability to:

* Pause stake/unstake (withdrawals always available)
* Change buyback source wallet

* Optional guardian role (time-limited, via timelock)