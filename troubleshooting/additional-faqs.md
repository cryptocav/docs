---
title: Additional FAQs
description: More answers to common questions.
icon: circle-question
---

### I received an NFT in my wallet that says it's from Orca, is it legitimate?

Orca pool positions are represented by an NFT, but any other NFTs purporting to be from Orca are almost certainly part of a scam. Orca will not send you an NFT that promises you free tokens or access to an airdrop. Orca will not ask you to connect your wallet to another website.

### I can't harvest my yield from my pool, why?

This can happen for two reasons:

* Your wallet does not have a token account for the token you are trying to harvest. **Solution:** if this is the case, trading to obtain a small balance of the token, should allow you to harvest.
* The rewards for the pool are depleted. **Solution:** raise the issue with a Community Manager on Orca's [#🤖│support-ticket](https://discord.com/channels/798712664590254081/1126616010481471589) Discord channel, they will ensure the party who adds the rewards for your pool are informed.

### I'm trying to close my position, but I get the error *"unable to close position because it's not empty"*, why?

This is usually happens when one of the reward tokens for the pool are depleted. **Solution:** raise the issue with a Community Manager via Orca's [#🤖│support-ticket](https://discord.com/channels/798712664590254081/1126616010481471589) Discord channel, they will ensure the party who adds the rewards for your pool are informed.

### When I try to trade, the trade button says *"Unavailable in your country or region",* what does that mean?

Orca has detected that you are connecting from a country or region blocked from trading on Orca. Please see [Locations blocked from using the Orca UI](/reference/useful-information/locations-blocked-from-using-the-orca-ui) for more details.

### An Orca Community Manager contacted me by DM, can I trust them?

Orca's Community Managers will never initiate private conversations. If they messaged you first they are an imposter, please report in Orca's [#🕵🏽│scam-reports](https://discord.com/channels/798712664590254081/844977837172850699) Discord channel.

### I want to trade a token, but can't find it on Orca, why?

Orca extracts its token list from CoinGecko - if the token is not listed on CoinGecko you can request to have it added to Orca (see [this guide](https://docs.orca.so/orca-for-liquidity-providers/community-listing/how-to-guides/how-to-add-a-token-to-the-orca-token-list)). If the token is listed on Orca, but you still can't trade it may be that no liquidity exists, you can check by searching for the token in the [liquidity browser](https://www.orca.so/liquidity/browse).

### I want to create a pool for my token, but it isn't listed, what can I do?

If you cannot find a token, it is likely because it is not on CoinGecko. You can either list your token there, or follow [this guide](https://docs.orca.so/orca-for-liquidity-providers/community-listing/how-to-guides/how-to-add-a-token-to-the-orca-token-list).

### What does the error *"oops something went wrong"* mean?

This error is often the result of an inadequate SOL balance. It is recommended to maintain a balance of at least 0.05 SOL in your wallet.

### Why does it say "trading pair not supported" mean?

If adequate liquidity doesn't exist for a pair in the current tick, trading is not possible.

### What does *"Try using a newer wallet that supports Versioned Transactions"*, mean?

Versioned Transactions are the latest transaction format which allows for additional functionality in the Solana runtime, you can read more [here](https://docs.solana.com/developing/versioned-transactions).

### Why doesn't the price in an Orca pool match the price shown on sites like CoinGecko?

Prices aren't set by Orca, or an oracle, each pool is its own market and the price is determined by trading activity. Prices will usually converge on wider market value through the action of trading, traders (and bots) specialising in arbitrage trading seek out imbalances between different markets and trade for profit.