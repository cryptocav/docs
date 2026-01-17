---
title: How to use Range Orders on Eclipse
description: Use range orders for advanced trading on Eclipse.
icon: arrow-right-arrow-left
---


Orca’s CLMM allows users to create customizable liquidity positions, such as single-sided asset positions, enabling them to trade in a way that is more familiar to users of Central Limit Order Books (CLOBs). These advanced strategies, often referred to as *range orders*, were not possible with traditional CPMM models.

A CLOB trader typically deploys limit orders to trade assets only at a specific price. Such orders are filled (subject to available liquidity) when the market reaches the set price.

By providing single-sided liquidity, Orca’s CLMM can broadly mimic a CLOB limit order.

These range orders offer both advantages and disadvantages compared to traditional CLOB limit orders. However, when used effectively, they allow a user to automatically buy or sell an asset at a predefined price.

The key advantages of a CLMM over a CLOB in this context include:

* **Fee earning**: While creating limit orders in a CLOB often incurs costs, CLMM users earn fees as their order is executed.
* **Tax advantages**: In many tax jurisdictions, a taxable event is not triggered until assets are withdrawn from the CLMM. This allows users to delay taxable events while assessing current market conditions.

### Limitations of range orders on a CLMM

The nature of CLMM mechanics means that not all order types that can be executed on a CLOB can be mimicked on a CLMM. As the current price of a pool rises, the asset increasing in value (relative to the paired asset) is incrementally sold for the asset decreasing in value. This mechanism means that only certain types of range orders are possible, specifically *Buy Limit Orders* and *Take Profit Orders*, which rely on this direction of conversion.

While a range order may appear no different from any other single-sided liquidity position, it is defined by the user’s intention rather than the mechanics of the pool. For a range order to be considered executed, the user must withdraw their assets. Otherwise, the range order will continue to function like any other position, with one asset being exchanged for the other as the price fluctuates within the position’s price range.

Creating a Buy Limit Order

Creating a Take Profit Order/Sell Limit Order

#### How to create a Buy Limit Order

Orca’s CLMM can be used by traders to execute a *Buy Limit Order*. This is made possible by CLMM mechanics—when one asset rises in value relative to its paired asset, it is sold in exchange for the other asset. By carefully deploying a single-sided liquidity position, traders can leverage the CLMM to effectively execute a *Buy Limit Order*.
**Examples:** You believe that SOL is likely to fall to a price of 150 USDC from its current price of 160 USDC before rebounding, and you want to buy SOL at the lower price to take advantage of the anticipated recovery. This can be achieved by creating a single-sided position across a downside price range in a SOL/USDC pool. For this example, we will create a tight custom range of 150.002226–150.017226 USDC per SOL in the 0.01% fee tier SOL/USDC pool. The deposit will consist entirely of USDC.
We now wait for the price to fall to or below the range minimum and then close our position. By that point, all the USDC will have been exchanged for SOL, and we will also have earned some trading fees.
It is also possible to create a type of *buy limit order* that cannot be achieved on a CLOB, designed to take advantage of an anticipated protracted downtrend with an expected bottom. In this case, a wider range can be set, aiming to earn trade fees throughout the duration of the downtrend. For example, we could create a range from 150.002226 to 160.011694 USDC per SOL. As the price moves down through this range, small amounts of USDC will be traded for SOL at every price point between the maximum and minimum range until all the USDC is exhausted.

If we withdraw after the price reaches or falls below our minimum range, the position will consist entirely of SOL, and we will have earned additional fees. With this method, the price paid for SOL will be averaged across the selected range, meaning it will be higher than the chosen minimum.

**Position Creation Process**

* Navigate to the Liquidity page (https://www.orca.so/pools)
* Ensure the UI and your wallet are set to the Eclipse network.

   * If you haven't done so already, connect your wallet.

   * Locate the pool in which you wish to create your Buy Limit Order by finding it in the pool list or using the search field

   ![](/images/image_99.jpg)

   TIP: You can search using the token name, ticker, or token mint address, but check carefully that you have selected the right token.
* Click on the pool you wish to add liquidity to. The liquidity sidebar will open.

   ![1](/images/image_100.jpg)
* Ensure `Custom` range is selected in the liquidity side bar.
   ![](/images/image_101.jpg)
* After selecting Custom Range a one sided range can be created in three ways

   * By dragging the sliders
   * By free typing the prices in the lower and upper fields
   * By using the + and - buttons in the lower and upper fields
* Enter the amount you wish to deposit in an appropriate field, or you can click on `Max` to deposit that quantity of tokens from your wallet (red boxes), you may need to scroll down. *In this example we are attempting to buy $1 of SOL at a price 10% lower than the current pool price, you can see this highlighted in the green box.*
   ![](/images/image_102.jpg)
* (Optional) Adjust your liquidity slippage by clicking on the liquidity button - see [Understanding Slippage](/trade/slippage) for more details. Once you are satisfied with your deposit values, click Deposit.
* Review the details in your wallet, including payable network fees and approve.

    **REVIEW CAREFULLY** it is critical you check your range and the current price of the pool match your intentions, depositing liquidity to a pool with a price not consummate with wider market values may result in loss.

If the price dips and passes through your range, your position will be made entirely of SOL tokens. You must withdraw your liquidity at this point to ensure it does not become active again and your position revert to USDC.

#### How to create a Take Profit Order/Sell Limit Order

Orca’s CLMM can be used by traders to execute a Take Profit Order or a Sell Limit Order. This is possible due to CLMM mechanics—when an asset is rising in value, relative to the paired asset, it is sold for the other asset, this means that by carefully deploying a single sided position the CLMM can be used to execute a Take Profit Order/Sell Limit Order. The method of execution of these two order types is identical even if the intention of the order may vary.
**Examples:** You believe that SOL is likely to rise to a price of 170 USDC from its current price of 160 USDC, and you want to sell your SOL for USDC at this higher price. This can be achieved by creating a one sided position across a price range on the up side of a SOL/USDC pool. For the purposes of this example we will create a tight custom range of 170.007724-170.024725 USDC per SOL in the SOL/USDC 0.01% fee tier pool. Our deposit will be composed entirely of SOL.
We now wait for the price to rise to or above the range Max and close our position. All the SOL will have been sold for USDC, we will also earn some trade fees.
It is also possible to create a type of Take Profit Order or a Sell Limit Order which cannot be achieved on a CLOB, which aims to take advantage of an anticipated protracted up trend, with an anticipated top. With this a wider range can be created, with the aim of taking advantage of trade fees during the period defined by the up trend. Here we could create a range from 160.011694-170.024725 USDC per SOL. As the price moves up through our range a little SOL will be sold for USDC at every price point between our Min and Max range until all the SOL is exhausted. If we withdraw after the price reaches or passes our Max range our position will be composed entirely of SOL and we will earn additional fees. With this method the price received for the SOL will be averaged out across the selected range, so will be lower than the selected Max.

#### Position Creation Process

* Navigate to the Liquidity page (https://www.orca.so/pools)
* Ensure the UI and your wallet are set to the Eclipse network.
* If you haven't done so already, connect your wallet.

   * Locate the pool in which you wish to create your Buy Limit Order by finding it in the pool list or using the search field


   TIP: You can search using the token name, ticker, or token mint address, but check carefully that you have selected the right token.
* Click on the pool you wish to add liquidity to. The liquidity side bar will open.

   * Ensure Custom range is selected in the liquidity side bar
   * After selecting Custom Range the a one sided range can be created in three ways

   * By dragging the sliders
   * By free typing the prices in the lower and upper fields
   * By using the + and - buttons in the lower and upper fields
* Enter the amount you wish to deposit in an appropriate field, or you can click on `Max` to deposit that quantity of tokens from your wallet (red boxes), you may need to scroll down. *In this example we are attempting to sell $1 of SOL at a price 10% higher than the current pool price, you can see this highlighted in the green box.*
   ![](/images/image_103.jpg)
* (optional) adjust your liquidity slippage by clicking on the liquidity button - see [Understanding Slippage](/trade/slippage) for more details. Once you are satisfied with your deposit values, click Deposit.
* Review the details in your wallet, including payable network fees and approve.

    **REVIEW CAREFULLY** it is critical you check your range and the current price of the pool match your intentions, depositing liquidity at a price not consummate with wider market values may result in loss.

If the price rises and passes through your range, your position will be made entirely of USDC tokens. You must withdraw your liquidity at this point to ensure it does not become active again and your position revert to SOL.