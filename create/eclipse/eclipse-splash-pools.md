---
title: How to create a Splash Pool on Eclipse
description: Create Splash Pools on Eclipse for simpler, more cost-effective liquidity.
icon: coins
---

Splash Pools offer a simpler, more cost-effective way to create liquidity pools on Eclipse.

### What are Splash Pools?

*Splash Pools* are a new innovation from Orca, designed to enable users and token creators to deploy liquidity in a unique type of pool built on top of Orca's existing CLMM infrastructure.

These pools exclusively support full-range positions, eliminating the need to initialize additional *tickArray accounts*. This makes them ideal for projects that want to establish pools that operate seamlessly without requiring ongoing management.

With Splash Pools, creating pools on Orca is faster, simpler, and more cost-effective than ever. Since Splash Pools use the same program as Orca's existing pools, they are automatically compatible with all current integrations.

### How do Splash Pools differ from true CPMM pools?

In *Splash Pools*, liquidity providers (LPs) receive a pool position NFT that represents their specific position, rather than receiving fungible LP tokens. Additionally, yields earned by LPs must be manually harvested, in contrast to CPMM pools where yields are automatically compounded into the position. This operational model offers LPs greater flexibility in managing their yields but requires more hands-on involvement compared to CPMMs.

### How to create a Splash Pool

The Pool Creation tool is intended for expert and professional users only. If you are neither of these, please carefully research this subject before using the tool. Alternatively create a ticket by accessing the [🤖│support-ticket](https://discord.gg/orca-so) channel on Discord.

This guide is for Orca Splash Pools: if you want to create a regular CLMM pool, please refer to [How to create an initial pool for an asset.](/create/eclipse/eclipse-clmm-pools)

NOTE: If you have not added your token to the Orca Token List, please refer to the guide [how to add a token to the Orca Token List](/create/eclipse/eclipse-orca-token-list).
If additional support is required, please reach out to Orca through an open communication channel or via [#❓│dev-questions](https://discord.com/channels/798712664590254081/838660851178274866) on Discord.

### How to Create a pool on Orca, permissionlessly

UI tooltips are provided in the pool creation modal. These contain useful information, so be sure to read them as you go.

* Before you can create a pool, your wallet must hold a quantity of each token in your planned pair, as well as sufficient ETH to pay any network fees.
* Navigate to https://www.orca.so/create-pool[.](https://www.orca.so/create-pool)
* Connect your wallet.
* Select `Create Splash Pool`.
* Click on `Select Token` to chose your token.
* Enter the symbol, name, or mint address for your token.
* (Optional) By default your token will be paired with SOL, if you wish to pair with another token instead click on the `SOL` label.
      Then select your chosen token from the list of find it by entering the symbol, name, or mint address.
* Enter your initial price, by typing it in the *Initial Price Field* (yellow box in image), or by selecting the Estimated Market Price (red box in image).

   NOTE: The *Estimated Market Price* is calculated based on market rates from Jupiter. Please verify the price before using it.
   It is **critical** that the pool creator ensure that this price meets their expectation.


   NOTE: The *Initial Price* is the price at which trading will commence. It is not possible to edit the price later; it can only be adjusted through trading actions.
   Failure to set the correct price can result in **loss of liquidity** or **additional costs**.
* Enter the number of tokens you wish to supply in one of the token fields. The amount of the paired asset to be deposited will be calculated automatically.
* When you are happy, click `Preview Pool`.
* Carefully review the parameters for your pool. Ensure you read the highlighted message. If you are satisfied, mark the checkbox.
* When ready, activate the `Create Pool` button.
    * Review the details in your wallet, then authorize.
* The pool creation progress will be displayed.
        You will need to authorize two transactions.
    * Congratulations! You have completed your pool creation. Carefully read the displayed message, note the grayed out buttons, these will change once your pool is fully active.
    * Once the pool is fully active in the Orca UI, the Trade and Provide Liquidity buttons will become active, all users will be able to see, trade against, and deposit to the pool now.
    
If your token is not on Orca's Token List it will carry a warning triangle. To remove this sign, please contact Orca via channels of communication your already have open, or create a ticket using the `Support` function in the wallet menu or by accessing the [🤖│support-ticket](https://discord.gg/orca-so) channel on Discord.

If you want to add rewards to your pool, please see [How to add rewards to a pool](/create/eclipse/eclipse-adding-rewards).