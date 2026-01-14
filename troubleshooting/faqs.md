---
title: FAQs
description: Frequently asked questions about Orca.
icon: circle-question
---

#### What is Orca?

Orca is a decentralized exchange (DEX) that strives to be the epicenter of spot trading on Solana.

Built by DeFi OGs with a user-first approach, Orca is now its smoothest, fastest and most reliable v2 iteration now. Combining constant-product like features on top of a concentrated liquidity AMM (CLMM) paired with an easy-to navigate intuitive UI, and unparalleled user support: Orca is accessible for traders and liquidity providers of all experience levels.

#### What is the difference between a CLMM and a traditional exchange?

There are two primary ways to trade cryptocurrencies: traditional order book exchanges (CLOBs) and [automated market maker](https://www.gemini.com/cryptopedia/amm-what-are-automated-market-makers) (AMM/CLMM) protocols. In a CLOB, buyers and sellers are matched based on price and the amount of tokens to trade. In contrast, AMMs allow users to trade against a pool of tokens rather than directly with other users.

For blockchain applications, Orca believes that CLMM-based trading protocols offer a superior approach due to their simplicity and composability. With the right tools and education, a CLMM can achieve everything a CLOB can—and more.

#### Why Solana?

Of the solutions competing to scale the blockchain ecosystem, Solana's performance stands out: 50,000 transactions per second, 400ms block times, and low transaction fees. What’s more, Orca has been continually impressed by the values, vision, and engineering progress of the Solana team. For these reasons, Orca believes that Solana is the best choice to support the next generation of DeFi apps.

#### How do I trade on Orca?

You can find a full guide for trading, [here](/trading/how-to-swap-solana).

#### What is an Adaptive Fee Pool?

An Adaptive Fee Pool dynamically adjusts trading fees based on market volatility. LPs still choose a base fee tier, but fees increase during volatile conditions—potentially earning more when trading activity generates increased price volatility → [Learn more about Adaptive Fee Pools](/reference/educational-documents/adaptive-fee-pools).

#### What is a Fixed Fee Pool?

A Fixed Fee Pool charges the same swap fee for every trade, regardless of market conditions. LPs select a specific fee tier (e.g., 0.05%), and that rate remains constant.

#### Why choose Orca for seasoned DeFi natives?

Orca continues to iterate in its quest to provide users with ever-improving reliability and efficiency. During periods of high volatility, on-chain trades often fail—precisely when success is most critical.

Beneath the surface, Orca incorporates several technical improvements:

* A front-end built with Next.js, which is slated to be open-sourced.
* A custom Smart Router using up to six liquidity pools to provide optimal pricing.

* Faster confirmation times and a simple retry mechanism.
* More accurate stats and price APIs.

* Dynamic priority fees.

Additionally, if a competitor (via Jupiter) offers a better price, you can choose that quote instead, without even leaving Orca.

#### What does "spend at most" and "receive at least" mean in the trade details dropdown?

The displayed figure represents the absolute maximum you will spend or the absolute minimum you’ll receive from your trade if slippage occurs to the maximum permitted extent. If slippage causes this figure to be exceeded, the trade will fail.

#### Where can I find more information on the fees displayed in the trade details dropdown?

A small portion of your trade goes to liquidity providers for the pools your trade routes through and a further portion to the Orca treasury and Orca Climate Fund (details [here](https://docs.orca.so/reference/trading-fees)). A further portion is network fees. The exact amount depends on the trade route.

#### What is a sub-route?

Orca's Smart Router can route your trade through up to six channels to find the best price. A sub-route is an indirect path for a trade, such as ORCA > SOL > USDC, rather than trading directly between ORCA and USDC. These indirect trades are sometimes referred to as multihop trades. To ensure the best price, Orca’s Smart Router can also split trades across multiple routes simultaneously. You can view how your trade is composed by expanding the trade details dropdown.

#### Does Orca have a governance token?

The ORCA governance token was launched on 9th August 2021. See the [Token Treasury](/staking/token-treasury) page for more details. For details of Orca's governance process please see the [Governance User Guide](https://docs.orca.so/orca-for-holders/governance/tutorials/governance-v0-user-guide).

#### Which wallets can I use with Orca?

To connect to Orca you will need a compatible wallet, a list of currently supported wallets can be found [here](https://docs.orca.so/reference/wallets). Orca plans to integrate other wallets that support Solana program execution, as they are released.

Orca cannot and does not endorse nor guarantee the security of compatible wallets. Podmates should exercise caution and [do their own research](https://docs.orca.so/orca-for-traders/how-to-guides/do-your-own-research-dyor) before interacting with or depositing to any wallet.

#### Can I use Orca on my phone?

You can use Orca on the phone with mobile device compatible wallets, you can find a list [here](https://docs.orca.so/reference/wallets).

#### Has Orca been audited?

Orca's Whirlpools concentrated liquidity product has been double audited and amendments are also audited → [View Orca's Audits](https://github.com/orca-so/whirlpools/tree/main/.audits).

#### What does "Not Enough SOL" mean?

SOL is required to pay network fees. It is recommended to maintain a balance of at least 0.05 SOL. Actual fees are typically far lower, but for simplicity, a small minimum balance of SOL is required to transact. → For more details, see: [Pool network fees](https://docs.orca.so/reference/pool-network-fees).

#### Which curves do Orca's pools use?

Orca's uses concentrated liquidity pools, similar to ([but not identical to](https://docs.orca.so/orca-for-liquidity-providers/master#how-do-orcas-pools-differ-from-uniswap-v3)) Uniswap v3. Each liquidity provider chooses a range within which to provide liquidity: trades are executed using the combined liquidity of all individual [in-range](https://docs.orca.so/reference/definitions#in-range-and-out-of-range) curves.

#### What fees do I pay when I trade?

* Taker fee: When trading, a percentage of the trade value is paid as a fee. These fees vary depending on the routing of your trade. The table [here](https://docs.orca.so/reference/trading-fees) shows the fee paid when trading on Orca, and how it is split between earnings for liquidity providers, Orca Treasury, and Climate Fund.
* Network fee: when trading a nominal amount of SOL is also paid in the form of Solana network fees. The exact amount varies depending on the parameters of the trade; when trading a token for the first time, more SOL is required to add that token to your wallet. In the past, typically trades cost between 0.0001 — 0.001 SOL. More details about network fees can be found [here](https://docs.orca.so/reference/pool-network-fees).

Orca does not charge any additional fees.

#### What is price impact?

The trade price on Orca depends on the size of the order, as price impact is influenced by trade size and available liquidity. As the number of tokens you buy from the pool increases, the token's price rises. This increase in price is called [price impact](https://www.researchgate.net/publication/46462472_Price_Impact). If your trade results in a price impact of 1% or more, the UI will display a *Price Impact Warning*. You can still proceed with the trade after acknowledging the warning.

#### Why did my trade fail?

If your trade fails, it is most likely due to market volatility causing the price to move beyond your slippage tolerance. When a trade fails, Orca will provide an error reason, and the UI will offer the opportunity to retry with the same parameters.

Due to current smart contract limitations, trades that route through multiple pools have a higher likelihood of failing. However, the transaction may succeed if sent again. Orca recognizes that this can be frustrating, so the new version incorporates improvements in trade logic when using multiple pools. Additionally, Orca dynamically adjusts slippage and priority fees to increase the likelihood of success, even during periods of Solana network congestion. If you prefer to adjust these settings manually, please refer to the guide on adjusting slippage tolerance.

#### How does Orca decide which tokens to list?

Orca adds tokens to the Orca Token List based on information provided by the project and demonstrable community demand (e.g., volume or interest). As a decentralized protocol that facilitates trades, Orca aims to support any asset tradable on Solana. Permissionless listing allows advanced users to create initial pools for assets (see [Orca for Asset Listers](https://docs.orca.so/orca-for-asset-listers)). While creating an initial pool is intended for advanced users, anyone can create a pool for a token already listed on Orca using the simpler [pool creation process](https://docs.orca.so/orca-for-liquidity-providers/classic-community-listing/creating-a-pool-tutorial).

#### Are tokens on Orca wrapped?

An increasing number of tokens on Orca are wrapped. There are several source protocols for wrapped tokens, please ensure to *Do Your Own Research.*

#### I have ERC-20 tokens in MetaMask. How can I trade them on Orca?

To trade ERC-20s on Orca, you’ll need to convert them to SPL tokens by transferring them through a bridge, it is important to *do your own research* before wrapping tokens.

#### How does concentrated liquidity impact the trade experience on Orca?

As a trader, there is nothing that need be done to take advantage of Orca's concentrated liquidity pools; all the magic happens behind the scenes.

#### Can I trade programmatically on Orca?

Of course! You can interact with pools using [Typescript SDK](https://github.com/orca-so/whirlpools). Please visit the [Orca Developer Portal](https://orca-so.gitbook.io/orca-developer-portal/orca/welcome) and [#📚│dev-resources](https://discord.com/channels/798712664590254081/1049775881008193716). Developer Advocates are on standby in the [#❓│dev-questions](https://discord.com/channels/798712664590254081/838660851178274866) channel in the Orca Discord, you can ask technical questions there!

#### What are the risks of using Orca?

There are a number of risks to using Orca:

* Smart contract vulnerabilities: The Solana Mainnet is still in beta, and there is always the possibility of an exploit in the smart contract. To mitigate this Orca's concentrated liquidity product is [double audited](https://docs.orca.so/orca-for-liquidity-providers/master#has-orca-been-audited).

* Divergence loss: also known as *impermanent loss*, occurs when token prices deviate from their initial deposit values, causing the value of liquidity to decrease compared to simply holding the tokens in a wallet. Due to market volatility, the value of deposited liquidity may be lower at the time of withdrawal than at the time of deposit, leading to potential losses for liquidity providers. For a detailed explanation, [blog post](https://pintail.medium.com/uniswap-a-good-deal-for-liquidity-providers-104c0b6816f2) from the Uniswap team is an excellent resource. The risk of divergence loss can be higher in concentrated liquidity pools.

   Divergence loss, as a metric, is a comparison of the value of a liquidity position versus simply holding the assets. Loss in value due to changes in the underlying asset's price is not considered divergence loss.
* Wallet providers: Orca is compatible with a wide range of wallets (see compatible [wallets](https://docs.orca.so/reference/wallets)). A wallet exploit could affect users.

   Orca **CANNOT** and does **NOT** endorse nor guarantee the security of compatible wallets. Podmates should exercise caution and do their own research before interacting with or depositing to any wallet.

#### Why was I charged higher network fees than usual?

When setting your chosen range, if it includes a lower and/or upper price limit that falls within price ranges where no positions have been created previously, you may incur additional network fees of 0.07 SOL or 0.14 SOL. These fees are non-refundable, so carefully review the quoted fees before authorizing the transaction. To avoid these costs, consider adjusting your range.

These fees are part of Solana's network fees, used as rent for an account called a tickArray, which is essential for Orca's pool operations. Orca cannot control these fees, and they may change if Solana updates its network fee structure. For more details on other fees, see: [Pool Network Fees](https://docs.orca.so/reference/pool-network-fees).

#### Why would I provide liquidity on Orca?

Whether or not you provide liquidity is entirely up to you. Users typically provide liquidity to Orca’s pools to earn trading fees. For example, if you provide liquidity to a SOL/USDC pool, you will receive a pool position NFT in return. This NFT acts as a receipt for your deposited tokens and is needed to withdraw them.

Each time a trade routes through your selected SOL/USDC pool, a fee is paid by the trader (the taker), a portion of which is shared with liquidity providers (the makers). See [Trading fees](https://docs.orca.so/reference/trading-fees) for details. These fees can be [harvested](https://docs.orca.so/orca-for-liquidity-providers/orca-v2-how-to-guides/how-to-harvest-yield) at any time.

#### How do I earn fees on Orca?

When you provide liquidity in a pool you earn a [maker fee](https://docs.orca.so/reference/trading-fees) from each trade executed against your liquidity, some pools also attract rewards. All earned yields are [harvestable](https://docs.orca.so/orca-for-liquidity-providers/orca-v2-how-to-guides/how-to-harvest-yield) at any time.

#### Can I harvest yield from just one position?

Yes, on Orca v2 it is possible to harvest a single position through Orca's UI, you can find instructions [here](/liquidity/harvesting-yield).

#### As a liquidity provider do I get ORCA tokens as a reward?

Orca occasionally distributes ORCA token rewards to encourage deeper liquidity for specific trading pairs. Eligible pools are clearly marked in the explorer. Pools that are not eligible for ORCA rewards will still generate trading fees from the provided asset pair.

#### How are the displayed yields calculated?

Yields displayed are based on the formula 24h Yield / TVL.

#### How is the current price in a pool determined?

The current price in an existing pool is determined solely by market action through trading. Orca cannot alter or interfere with this price, even if the pool is empty. The initial price in a new pool is set by the pool creator. To avoid losses, users should ensure the current price matches their expectations before depositing liquidity or trading, and pool creators should take care when setting the initial price.

**REVIEW CAREFULLY:** it is critical you check your range and the current price of the pool match your intentions, depositing liquidity at a price not consummate with wider market values may result in loss.

#### Can I withdraw my liquidity at any time?

Yes, the Orca protocol allows you to withdraw liquidity at any time.

#### Can I yield farm / stake on Orca?

Some pools attract rewards in the form of token emissions, pools currently receiving emissions can be found here.

Trading fees and emission yields accrue continuously and can be harvested any time with no lock-up. Orca does not offer single-sided staking.

#### What are the risks and advantages of concentrated liquidity pools?

In Orca's concentrated liquidity pools, liquidity providers compete for trading fees and token emissions, which are distributed based on the parameters of their positions. The effects of leverage mean that tighter positions receive higher yields than wider ones. However, tighter ranges are also more vulnerable to Divergence Loss (also known as Impermanent Loss or IL) and are more likely to fall out of range. Out-of-range positions do not earn.

#### Why doesn't Orca display APRs for pools?

Projecting an APR based on past activity is not a reliable way to predict yields over a year. Orca displays the pool's 24-hour Yield/TVL, but it's important to remember that past performance is not a guarantee of future returns.

You can adjust settings in the UI to display an annualized yield projection: *Annualized Yield / TVL (24h)*. However, it's important to note that projecting an annualized yield using 24 hours of activity is illustrative only and not should not relied up on.

#### What token represents my deposit?

In traditional constant product pools, liquidity provider (LP) tokens represent ownership of liquidity. These pools have a fixed range and no multiplier, making all LP tokens identical and fungible.

In Orca's concentrated liquidity pools, however, liquidity providers set the parameters of their positions, making each LP token unique and non-fungible.

Positions in Orca's pools are represented by NFTs, which serve as a receipt for your liquidity. If a pool position NFT is burned or lost, the associated liquidity and any yield cannot be withdrawn and are irrevocably lost. For more information, see [What is a pool position NFT](/reference/faqs#what-is-a-pool-position-nft-can-i-sell-it).

#### What is a pool position NFT? Can I sell it?

The pool position NFT is an LP token that represents a position in a pool. If it is burned or lost, the associated liquidity cannot be withdrawn. It is technically possible to trade a pool position NFT on secondary markets; however, if sold, the associated liquidity is also transferred to the buyer and will no longer be held by the original owner.

#### How do price ranges work?

In traditional constant product pools, liquidity is provided across the entire price range (from 0 to ∞). In Orca's concentrated liquidity pools, however, users select the minimum and maximum prices for their liquidity. It's important to note that these limits are not arbitrary; users must choose from a set of evenly distributed, discrete ticks.

#### What happens if the price goes above or below my limits?

Trading continuously influences the fluctuation of a pool's price and token balances.

As users trade token B for token A, the pool's price shifts toward the position's maximum limit. Due to the laws of supply and demand, the value of token A increases relative to token B. Once the price reaches the maximum limit, all of token A will have been sold, leaving the position entirely composed of token B. Conversely, when the price approaches the position's minimum limit, the reverse occurs.

If the current price reaches or exceeds the minimum or maximum limits, the position becomes dormant, ceasing to provide liquidity and, therefore, stops earning incentives or trading fees. However, if the price moves back within the position's range, liquidity provision, incentives, and trading fees will resume.

#### How can I provide liquidity if my position is out-of-range?

If your position is out-of-range, you can either wait for it to return to the price range (if expected) or provide liquidity to a new range.

Should you wish to set a new range, you will need to withdraw your liquidity. Since the tokens withdrawn will not match the required deposit ratio of an in-range position it will be necessary to trade, you can do this using the Autoswap toggle.

#### Does concentrated liquidity mitigate Divergence Loss?

No. The exposure to divergence loss increases relative to th of the selected range.

However, concentrated liquidity, pools allow users to deposit less liquidity and get the same or higher yields, due to the multiplier effect of [leverage](https://docs.orca.so/reference/definitions#leverage).

#### Why isn’t the deposit ratio 50:50 for my range?

The deposit ratio is dependent on the selected price range and its relationship to the current price: the closer the current price is, to either of the min or max limits than it is to the other, the less balanced the deposit ratio will be. A full range position will have a 50:50 deposit ratio.

#### How is the leverage shown in the UI calculated?

![](/images/image_28.jpg)

In this formula Pu is the max price, and Pl is the min price for the elected price range.

#### How do Orca's CLMM pools differ from Uniswap V3?

Beside the obvious advantages of Solana's low transaction fees and fast transactions, Orca's pools have:

* a simpler, more guided UX for concentrated liquidity provision;
* a [double audited](https://docs.orca.so/orca-for-liquidity-providers/master#has-orca-been-audited), custom built, and open sourced smart contract designed for the Solana virtual machine;

* built-in yield farming—a first for any concentrated liquidity AM.

#### How much of the emissions rewards will I earn?

When emission-based rewards are applied, a fixed number of tokens are distributed each second according to the weekly emission rate. These rewards are shared proportionally among liquidity providers based on their share of the pool’s in-range liquidity.

For example, if you hold 1% of the liquidity in the current tick, you will receive 1% of the rewards distributed every second.

#### What is the fee structure for using Orca's pools, and are there different fee rates for different pairs?

When creating a pool users can choose a fee rate, which will determine the taker fee paid by traders. How this fee is divided can be seen here.

#### How do I track PnL (profit and loss) after providing liquidity in pools?

First, decide whether your PnL (Profit and Loss) will be tracked in terms of the deposited tokens or relative to a currency such as USD. Make a note of the token values at the time of your initial deposit (if you did not do this, these values can be retrieved from a blockchain explorer). You will also need to track harvested yield and any additional deposits.

Provided you have this data, the formula to calculate your PnL is straightforward:

**PnL = Final Value of Position + Accumulated Fees and Rewards - Value of Deposits**

**Disclaimer:** The content of this communication is not financial advice and should not be relied upon as such. This communication has not been provided in consideration of any recipient’s financial needs. Orca has not conducted any financial assessment based on the personal circumstances of any recipients. Before using the protocol, carefully review all relevant documentation and consider the risks, including the total loss of funds.

#### I burned my Pool Position NFT, can Orca help me retrieve my funds?

No. If a Pool Position NFT has been burned there is no way for Orca (or anyone else) to access the liquidity that was associated with it.
The NFT is the proof to the blockchain that your wallet owns the liquidity, if that proof is destroyed you can no longer interact with the liquidity it represented.
Because Orca's pools are non-custodial it is not possible for Orca to alter the ownership retrospectively, nor assign the ownership to a new NFT.

#### Will the old Community Listing feature be deprecated?

Yes, the older Community Listing feature is not included in Orca v2, which has a completely new pool creation flow.

#### Does Orca charge fees to create pools?

No, only Solana network and Metaplex fees are payable.

#### What are Token Extensions?

Token Extensions are advanced functionalities for tokens to comply with legal requirements. Majority of the tokens created do not need Token Extension functionalities turned on. For more information, check out our [Token Extensions document](/reference/useful-information/token-extensions).

#### I created a new pool but can't find it in the UI, where is it?

It can take up to 15 minutes for a new pool to appear in the UI. Forcing a reload in your browser may reduce this time.

#### How can I change the token price in my pool after I create it?

You can't simply change a price in a pool, only market action can change a pool price. If you need help calculating the size of trade needed to move the current price to the target price please reach out to Orca. If you do not have an open channel of communication with Orca then please create a ticket by accessing the [🤖│support-ticket](https://discord.gg/orca-so) channel on Discord.

#### Should I create my pool, before or after launch?

This is up to you, but be aware that once a pool is created your token will be visible in the UI and anyone with any of your token will be able to add liquidity to the pool and/or trade against it.

#### How can I delete a pool I created?

It is not possible to delete a pool, it is therefore critical to take care during the creation process.

#### How can I remove the warning triangle that shows on my token?

To remove this sign, please contact Orca to discuss its removal, you can speak to Orca via channels of communication your already have open, or create a support ticket directly in the UI or by accessing the [🤖│support-ticket](https://discord.gg/orca-so) channel on Discord.

#### How can I get price data to show for my token?

Price data on Orca is usually derived from a pool on Orca.

Price data in wallets and other dApps is typically extracted from CoinGecko API data, it is therefore sensible to list your token on CoinGecko at the first opportunity (see [How to list a new asset with CoinGecko)](https://docs.orca.so/orca-for-asset-listers/how-to-guides/how-to-list-a-new-asset-with-coingecko)

#### I have spotted an issue, what should I do?

Orca is committed to continual improvement of new Orca and would love to hear your feedback or reports, head over to the [#🐛│bug-reports](https://discord.com/channels/798712664590254081/805037868174409748) channel and let us know.

#### My question isn’t covered, what can I do?

Orca will continue to refine these FAQs based on questions asked. Please head to [#🤖│support-ticket](https://discord.com/channels/798712664590254081/1126616010481471589) to ask Orca's AI, Mava, or one of our CMs your question: they will endeavor to help. Orca is keen to improve these documents continually, your feedback, suggestions and questions are appreciated.

#### What's next for Orca?

Orca is working on multiple improvements for the existing product and will continue to iterate. The journey of becoming an epicenter of spot trading on Solana never ends! There are additional projects in the works that will apply Orca’s core principles of human-centered design to new areas of finance. Because no matter whether you’re a trader, liquidity provider, new token creator, or builder — Orca wants to make it easy for you 🐳