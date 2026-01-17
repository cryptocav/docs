---
title: Glossary
description: Glossary of DeFi and Orca-specific terms.
icon: book
---

Key terms and concepts used throughout Orca's documentation.

#### Asset Allocation

How you deploy your overall capital, how you spread it out across different asset classes, such as shares, commodities and assets: diversification here can also be used to reduce risk. Selecting an Asset Allocation strategy that suits your goals, risk tolerance and the lenght of time you want to hold an asset or collection of assets, should follow a structured plan with objectives.

#### Deposit Ratio

The ratio of the two assets deposited is determined by the price you set at this step.

#### Diversification

A well known adage is "Never put all your eggs in one basket".

Diversification refers to the practice of allocating capital across a broad range of financial asset classes, products, instruments, strategies, and protocols. Within DeFi, besides simply owning a range of assets, diversification can also refer to deploying those assets variously though - for example - staking, lending, or providing liquidity. In the case of Concentrated Liquidity, it is also possible to diversify within a single pool by selecting multiple separate price ranges.

The goal of diversification is to reduce the overall risk that may arise form holding a narrow range of assets, asset classes, or deploying single strategies. A diverse portfolio composition is more likely to experience smoother variance in overall value and earnings during times of heightened market volatility.

Diversification can be achieved within a single asset class (such as holding a range of assets) and across asset classes (such as owning commodities, shares, securities, saving, and assets).

#### Divergence Loss

Divergence loss is one type of risk that liquidity providers take in exchange for fees they earn in liquidity pools. If divergence loss exceeds the yield earned upon withdrawal, the user has suffered negative returns compared to holding their tokens outside the pool. In CLAMM pools, both the yield from trading fees and rewards and divergence loss are amplified.

#### Estimated Yield

Projected yields are estimated using data drawn from the previous 24 hours of trading for the price range selected. Note that concentrating liquidity increases both yield and divergence loss, and previous returns are not a guarantee of future returns.

#### Fee Rate

The percentage of each trade for this pool that goes to liquidity providers. This value may change to optimize fees over time.

#### In-Range and Out-of-Range

In a concentrated liquidity pool a user defines the boundaries of the price-range within which they wish to provide liquidity. When the current price of the asset is within the selected price-range, a liquidity provider's position is "In-Range" and the user will earn trading fees, and any associated incentives.

However, if the current price for the pair moves outside the users selected price-range, their position would now be "Out-of-Range" and two things will happen: firstly, the users position will become dormant - no incentives, or trading fees, will be earned; secondly, the user's position will consist entirely of one asset. As long as the user's position remains "Out-of-Range", these conditions will remain the case. If the current price for the pair moves back into the price-range of the user's position, then fees and rewards will recommence and the balance of the position will once more begin to fluctuate with the relative values of the paired tokens.

#### Leverage

How concentrated your liquidity will be compared to a constant product AMM pool. If this number is 8x, you would earn 8x the fees and incentives for each trade. Likewise, your capital will be exposed to a comparably higher risk of divergence loss.

#### NFT Mint Address

The existence of price ranges makes each pool position unique. Therefore, each position is represented by an NFT instead of fungible pool tokens.

#### Price Range

Liquidity deposited will only be used for trades (and earn fees and incentives) when the current price of the assets in this pool is within this range.

#### Risk Tolerance

Describes the variability in expected returns (or losses) that a user is prepared to accept, across the planned time frame the user expects to hold the asset, when set against the assessed likelihood of possible outcomes. It is important that, as part of planning, users assess their personal willingness to accept the range of changes in value and incentives reasonably anticipated for their chosen assets and strategies. Risk tolerance is a personal matter, we request that users do their own research and evaluate their own risk tolerance before using pools.

#### Tick Spacing

Each pool is divided evenly into buckets of liquidity with predefined boundaries known as "ticks". A tick spacing of 8 means that each tick is 0.08% larger than the previous tick, and 128 means that each tick is 1.28% larger than the previous tick. Stable pools use smaller tick spacing to allow for more granular price ranges.