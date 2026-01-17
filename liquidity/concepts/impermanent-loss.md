---
title: Impermanent Loss
description: Understand impermanent loss and how it affects LPs.
icon: droplet
---

**What This Guide Covers**

Impermanent loss (IL) is one of the most misunderstood concepts in DeFi.
Despite the name, IL is not always impermanent—and not always a true loss relative to your original capital.

This guide explores:

* Why the term "impermanent loss" can be misleading
* How IL behaves in Concentrated Liquidity Market Makers (CLMMs)

* When IL becomes permanent—and when it does not
* How strategic management of positions can affect outcomes

* Why Orca believes the term *Divergence Loss*(DL) better describes this phenomenon

Understanding these dynamics is essential for liquidity providers who want to make informed decisions and optimize returns over time.

### Understanding Impermanent Loss in CLMMs

Most liquidity providers (LPs) have heard of *impermanent loss* (IL), but many struggle to fully understand what it is—or perhaps more importantly, what it isn’t. (Spoiler: it’s not always impermanent, and not necessarily a loss.)

Given the term’s ambiguity, it's hardly surprising that IL is often misunderstood.

In essence, impermanent loss might be *neither* truly impermanent nor an *actual* loss. Whether IL becomes permanent—and whether it results in a real loss—depends entirely on how and when the liquidity provider interacts with their position.

So, what exactly is impermanent loss? Let's walk through it carefully.

### What Impermanent Loss Means

**Impermanent:** Temporary; capable of being reversed.
**Loss:** A reduction in value.

In an Automated Market Maker (AMM), IL occurs when the relative prices of the assets you’ve provided liquidity for change compared to when you deposited them. If you withdraw liquidity at a different price ratio, the value of your position may be lower than if you had simply held the tokens.

However, IL is:

* Not always impermanent.
* Not always a true loss in absolute terms.

* Not necessarily worse than other strategies.

In a Concentrated Liquidity Market Maker (CLMM) like Orca, these effects can be sharper—but they can also be managed carefully.

### Why the Name Is Confusing

The term "impermanent loss" itself can cause misunderstanding:

* **Impermanence** suggests the loss will resolve itself. In reality, if you withdraw liquidity at the wrong time, the loss becomes permanent.
* **Loss** implies that LPs are left worse off. Yet many LPs stay profitable overall, even after accounting for IL.

Understanding these nuances is critical for making informed liquidity decisions.

### Example Scenarios

For simplicity, we assume:

* 1 USDC = $1
* **Initial SOL price:** $200
* **Selected range:** $160–$250
* **Liquidity provided:**

  + 2.5 SOL (worth $500)
  + 500 USDC

1

#### Scenario 1: When Impermanent Loss Is Temporary

* Price falls to: 170 USDC/SOL
* If you withdraw now:

  + Receive ~4.50 SOL (worth ~$766) + 130 USDC
  + Total value: ~$896

* If you had simply held:

  + 2.5 SOL (worth ~$425) + 500 USDC = $925

At this moment, withdrawing would realize an IL of $28.86

However, if you wait and the price returns to $200, your position would again be worth $1000—no loss realized.

This outcome is explained by path independence:
In a CLMM, if you withdraw liquidity at the same price you deposited, you'll retrieve the same value, regardless of the path prices took.

> **Key takeaway:**
> Impermanent loss can become permanent but only if you withdraw liquidity at a price point other than the one at which you deposited

2

#### Scenario 2: When Impermanent Loss Isn't Truly a Loss

* **Price rises to:** 250 USDC/SOL
* **If you withdraw now:**

  + Receive ~1059 USDC
  + Total value: ~$1059

* **If you had simply held:**

  + 2.5 SOL (worth ~$625) + 500 USDC = $1125

Compared to holding, you have "lost" $65.83.

However, you are still ahead of your original $1000 deposit.

This illustrates that IL is often a *relative* loss—it compares your LP strategy to simply holding, rather than showing an absolute decrease in value.

And importantly, this does **not yet** include any trading fees earned while your liquidity was active, which can more than compensate for the IL.

### Key Takeaway

* **IL is only realized if you withdraw.**
  If you wait and prices recover, the loss can disappear. It is worth noting that price may never return to the exact deposit value.
* **IL is a relative measure, not an absolute loss.**
  You can still be in profit compared to your initial deposit.
* **Fee earnings are critical.**
  You outperform simple holding when your earned fees exceed any realized IL.
* **Position management matters.**
  If you expect price recovery, holding your position may be better.
  If you expect continued divergence, repositioning could make sense.

---

### Terminology: Why Orca Prefers "Divergence Loss"

While the industry-standard term is *impermanent loss*, Orca often refers to the phenomenon as *divergence loss* (DL).

We believe *divergence loss* is a clearer and more accurate description, because:
* The impermanence of IL depends entirely on LP behavior—not market behavior alone.

* Divergence directly reflects what happens: asset prices move apart (diverge) from their original ratio.
* Loss should always be understood relative to an alternative action, not automatically assumed to be absolute.

Throughout Orca documentation, you may encounter both terms used side-by-side, especially in contexts where external standards are also referenced.

Our goal is to help liquidity providers fully understand the risks, strategies, and outcomes associated with liquidity provision—without relying on misleading terminology.

### Conclusion

Impermanent loss is an important concept for every liquidity provider to understand—but it’s only part of the bigger picture.
Managing liquidity positions requires balancing:

* Fee generation
* Risk of price divergence

* Opportunity costs compared to alternative strategies like holding, staking, or lending

With careful strategy and active management, LPs can often turn impermanent loss from a threat into an opportunity.