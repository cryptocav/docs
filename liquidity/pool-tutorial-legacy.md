---
title: Creating a Pool Tutorial
description: Tutorial for creating a new liquidity pool.
icon: droplet
---

#### Create a pool

* Select `Liquidity` at the top of the main screen.
* With the Explorer tab active click on `+Create a pool`.
* Read the explanation in the *Create a pool* modal, and then select `Get started`.
* Enter *Token A* using its label, symbol or mint address, then repeat for *Token B*.
* (Optional) if you have not already done so select `Connect wallet`.
* Select `Continue to next step`.
* Carefully set initial deposit parameters.

   Note: these parameters are critical to how your pool will operate.
   Pool fee rates are analogous to a spread in a traditional orderbook: a 0.30% fee rate equates to a 60 bps spread for traders. Different fee tiers are useful for market makers during varying levels of market volatility.
   Please do your research and swim carefully when creating your pool.
* When you are ready select `Preview`.
* Review details of your pool carefully.

   Warning: high transaction fees: creating a pool uses a lot of space on the blockchain. Solana network fees will be higher than for standard transactions.
* Select `Create pool` and deposit, review and approve in your wallet: this transaction creates your pool.
* A second transaction is needed to deposit to the pool, review and approve in your wallet.
* That's it! Your pool is live!

    Note: you can find links in the modal to your pool, but new pools may take up to 10 minutes to appear in the explorer.
* (Optional) select `Add token to the Orca Token List` if you wish to add a token to Orca's token list - this will open a form on which you can submit a request. Please see [How to add a token to the Orca Token List](/token-creators/orca-token-list) and/or [How to add rewards to a pool](https://app.gitbook.com/o/-MUINxovuAV6FEUooNDz/s/-MPvyETgLWLe-8rEIO01/~/changes/TF0SYvYQ6VUMgMf7hlf6/orca-for-liquidity-providers/community-listing/how-to-guides/how-to-add-rewards-to-a-whirlpool).