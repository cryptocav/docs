---
title: How to create an initial pool for an asset on Eclipse
description: Create concentrated liquidity (CLMM) pools on Eclipse for token creators and advanced users.
icon: coins
sidebarTitle: How to create an initial pool for an ...
---

This guide walks through creating a concentrated liquidity (CLMM) pool on Eclipse for token creators and advanced users.

A simpler model, *Orca's Splash Pools*, are also available for users wanting a quicker, simpler and cheaper pool requiring little management see the [How to create a Splash Pool guide](/create/eclipse/eclipse-splash-pools).
The *Concentrated Pool Creation Tool* is intended for expert and professional users only. If you are neither of these please very carefully research this subject before using the tool, please create a ticket by accessing the [🤖│support-ticket](https://discord.gg/orca-so) channel on Discord, if you need assistance or have any questions.

NOTE: If you have not added your token to the Orca Token List (see [how to add a token to the Orca Token List](/create/eclipse/eclipse-orca-token-list)), tickArray accounts may need separately initialising for your token to facilitate trade. This can be achieved by creating additional positions. [Orca Splash Pools](/create/eclipse/eclipse-splash-pools) do not require tickArray management, and may be a better option for some users.

You can view the state of your pool, including its tickArrays on Account Microscope (https://everlastingsong.github.io/account-microscope/).
If additional support is required, please reach out to Orca through an open communication channel or via [#❓│dev-questions](https://discord.com/channels/798712664590254081/838660851178274866) on Discord.

### How to Create a pool on Orca, permissionlessly

#### Full Range

UI Tool tips are provided in the pool creation modal, these contain useful information so be sure to read them as you go.

* Before you can create a pool your wallet must hold a quantity of each token in your planned pair, as well as sufficient ETH to pay any network fees.
* Navigate to https://www.orca.so/create-pool.
* Connect your wallet.
* Select `Create Concentrated Pool`.
   ![](/images/image_135.jpg)
* Click on `Select Token` to chose your token.
   ![](/images/image_136.jpg)
* Enter the symbol, name, or mint address for your token.
   ![](/images/image_137.jpg)
* (Optional) By default your token will be paired with SOL, if you wish to pair with another token instead click on the `SOL` label.
   ![](/images/image_138.jpg)
   Then select your chosen token from the list of find it by entering the symbol, name, or mint address.
* NOTE: The *Estimated Market Price* is calculated based on market rates from Jupiter. Please verify the price before using it.
   It is **critical** that the pool creator ensure that this price meets their expectation.

   ![](/images/image_139.jpg)

   NOTE: the initial price is the price at which trading will commence. It is not possible to edit the price later, which can be moved through trading action alone.
   Failure to set the correct price can result in **loss of liquidity** or **additional costs** moving the price through trading action.
* Enter the number of tokens you wish to supply in one of token fields. The number of the paired asset to be deposited will be calculated automatically.
   ![](/images/image_140.jpg)
* If you wish to create a pool with a different fee tier that the displayed one, click `Change`.
    ![](/images/image_141.jpg)
* Pick a *fee tier* from the available tiers.
    ![](/images/image_142.jpg)
* When you are satisfied with your parameters click `Preview Pool`.
    ![](/images/image_143.jpg)
* Carefully review your parameters, and read the highlighted message. If you are happy check the checkbox.
    ![](/images/image_144.jpg)
* Click `Create Pool`.
    ![](/images/image_145.jpg)
* The pool creation progress will be displayed.
    ![](/images/image_146.jpg)
    You will need to authorize two transactions.
    * Congratulations! You have completed the pool creation. Carefully read the displayed message, note the grayed out buttons, these will change once your pool is fully active.
    ![](/images/image_147.jpg)
* Once the pool is fully active in the Orca UI, the Trade and Provide Liquidity buttons will become active, all users will be able to see, trade against, and deposit to the pool now.
    ![](/images/image_148.jpg)

#### Custom Range

UI Tool tips are provided in the pool creation modal, these contain useful information so be sure to read them as you go.

* Before you can create a pool your wallet must hold a quantity of each token in your planned pair, as well as sufficient ETH to pay any network fees.
* Navigate to https://www.orca.so/create-pool.
* Connect your wallet.
* Select `Create Concentrated Pool`.
* Click on `Select Token` to chose your token.
* Enter the symbol, name, or mint address for your token.
* (Optional) By default your token will be paired with SOL, if you wish to pair with another token instead click on the `SOL` label.
   Then select your chosen token from the list of find it by entering the symbol, name, or mint address.
* Enter your initial price, by typing it in the *Initial Price Field* (red box in image), or by selecting the Estimated Market Price (yellow box in image).

   NOTE: The Estimated Market price is calculated based on market rates from Jupiter. Please verify the price before using it.
   It is **critical** that the pool creator ensure that this price meets their expectation.


   NOTE: the initial price is the price at which trading will commence. It is not possible to edit the price later, which can be moved through trading action alone.
   Failure to set the correct price can result in **loss of liquidity** or **additional costs** moving the price through trading action.
* Select `Custom Range`.
   ![](/images/image_149.jpg)
* Enter your *Min Price* and *Max Price* for your range, by typing in the fields or using the `+` and `-` buttons.
    ![](/images/image_150.jpg)
* Enter the number of tokens you wish to supply in one of the token fields. The number of the paired assets to be deposited will be calculated automatically.
    ![](/images/image_151.jpg)
* If you wish to create a pool with a different fee tier than the displayed one, click `Change`.
    ![](/images/image_152.jpg)
* Pick a *fee tier* from the available tiers.
    ![](/images/image_153.jpg)
* When you are satisfied with your parameters click `Preview Pool`.
    ![](/images/image_154.jpg)
* Carefully review your parameters, and read the highlighted message. If you are happy check the checkbox.
    ![](/images/image_155.jpg)
* Click `Create Pool`.
    ![](/images/image_156.jpg)
* The pool creation progress will be displayed.
        You will need to authorize two transactions.
    * Congratulations! You have completed the pool creation. Carefully read the displayed message, note the grayed out buttons, these will change once your pool is fully active.
    * Once the pool is fully active in the Orca UI, the Trade and Provide Liquidity buttons will become active, all users will be able to see, trade against, and deposit to the pool now.
    
If your token is not on Orca's Token List it will carry a warning triangle. To remove this sign, please contact Orca via channels of communication your already have open, or create a ticket using the `Support` function in the wallet menu or by accessing the [🤖│support-ticket](https://discord.gg/orca-so) channel on Discord.

If you want to add rewards to your pool, please see [How to add rewards to a pool](/create/eclipse/eclipse-adding-rewards).