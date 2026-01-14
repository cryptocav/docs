---
title: Understanding Slippage
description: Understand slippage, price impact, and how to protect your trades.
icon: arrow-right-arrow-left
---

### Slippage, price impact, and poor value trades

It is important when using Orca (or any dApp) to understand: what slippage is and what it is not; the associated risks and implications of its use; and when to consider adjusting your settings.

It is also important to understand the differences between slippage, price impact, and poor value trades.

#### What is slippage?

When trading slippage is the difference between the quoted price when you authorized a transaction and the final price your trade executes at. Movement of token values, in the liquidity pools against which you are trading, that occur between you authorizing a trade and the trade reaching on-chain finality can result in variation in the number of tokens received (or spent).
When depositing to, or withdrawing from a pool, the ratio of tokens deposited/received fluctuates with the pool price, slippage in this context, therefore has an impact on the ratio of tokens deposited or received.

#### Slippage tolerance settings

Users are able to set how much slippage they are willing to accept and still see their transaction executed. Setting your slippage tolerance defines the maximum percentile change you are willing to accept between the originally quoted outcome and the final amounts when the transaction settles.
In times of high volatility and/or congestion increasing your slippage tolerance may improve the chance of your trade executing successfully. However, setting slippage too high can result in your transaction being front run or subjected to a sandwich attack.

### Risks of setting a high slippage tolerance

Setting slippage tolerance settings too high comes with some risks

* Front running and sandwich attacks
* Poor value trades

**What is Front Running?**

Blockchain front running occurs when another user, with access to information on unconfirmed transactions, uses that knowledge to place a transaction ahead of yours on the blockchain. This results in your transaction executing at a disadvantageous price relative to the expected outcome, allowing the attacker to extract value from you.

A sandwich attack is a specific form of front running where the original transaction is inserted between two or more transactions, further enhancing the value extraction for the attacker.

Front running extracts value by causing the original transaction to experience more slippage than it would have without the insertion of the attacker's transactions. Since a transaction cannot experience more slippage than the set maximum slippage tolerance, setting a lower slippage tolerance reduces vulnerability to front running.

#### Slippage tolerance settings causing Poor Value Trades

Besides exposing yourself to the risk of front running, if slippage is set too high there is the risk that your transaction will execute at a poor value for you. This can happen simply because of sudden price movement happens to occur between you authorizing your transaction and settlement. This can be avoided by ensuring that slippage tolerance settings are not set too high.

#### Slippage vs Price Impact

These terms are often confused or used interchangeably, but they truly refer to different concepts. While slippage is the movement of transaction values that occurs between the time a transaction is quoted and when it is settled—caused by factors other than your transaction itself—price impact is the change in price specifically caused by your transaction. High price impact can occur when your trade is large compared to the available liquidity.
Orca’s UI displays price impact information when quoting a trade. It is important to carefully consider whether you are willing to accept a trade with a high price impact, as it can result in a poor value trade.

#### Trade Slippage vs Liquidity Pool Slippage

Orca recognizes that slippage when trading and when transacting against a pool, as an LP, are quite different, as such Orca allows users to set separate slippage tolerance settings for liquidity pool transactions and trades.

As liquidity pool transactions (adding/removing liquidity or closing a position) are more prone to transaction failure due to slippage, and are not exposed to the risk of front-running, a higher success rate can be safely achieved by increasing pool slippage tolerance.

#### When to set a higher slippage tolerance

Setting a higher slippage tolerance may be necessary at times to ensure your transaction settles, below are some examples, this is not an exhaustive list and caution must be taken when setting a higher slippage tolerance:

* High Volatility: When transacting in a highly volatile market, prices can change rapidly. Increasing slippage tolerance ensures that your transaction goes through despite these fluctuations. If you do not need to transact quickly, make modest increases, until the transaction succeeds, or simply wait for volatility to ease.
* Low Liquidity: In markets with low liquidity, price swings are more common due to the limited number of buyers and sellers. Higher slippage tolerance may help ensure your trade is executed.
* Urgent Transactions: If you need a transaction to be executed quickly and can't afford for it to fail, setting a higher slippage tolerance can prevent delays caused by minor price changes.

Remember, while setting a higher slippage tolerance can facilitate the execution of your trade, it also exposes you to an increased risk of a poor value trade. Use this option judiciously based on your specific trading needs and market conditions and only increase slippage tolerance after careful consideration and research. Orca cannot accept responsibility for poor value or loss caused by inappropriate slippage tolerance settings.

#### Other causes of poor value trades

While Orca’s trade router will search for the best price and trade across multiple pools to deliver it, each pool on Orca remains its own distinct and separate market, independent of every other pool on Orca and beyond in the wider market. The only action that keeps prices in a pool aligned with wider market values is trading activity. Prices are not controlled by Orca, nor are they adjusted to match a 'correct price'. The price you see for a token on a price aggregator site, such as CoinGecko, is an average of the token prices across all available markets tracked by that aggregator; it is not a true or correct price.

As such, when you receive a trade quote, it is critical to ensure that you are satisfied with the trade and that it meets your expectations regarding value. Failing to verify that the quoted price meets your expectations may result in a poor value trade. This risk is amplified by thin liquidity, new, dormant, or infrequently used pools, or periods of high volatility—particularly with new tokens. Orca cannot accept responsibility for any poor value trades a user experiences.