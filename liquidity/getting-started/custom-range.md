---
title: How to create a Custom-Range Position on Solana
description: Create concentrated liquidity positions with custom price ranges.
icon: droplet
sidebarTitle: How to create a Custom-Range Position...
---

While providing liquidity to a concentrated liquidity pool offers multiple benefits, it is an advanced feature best suited for experienced liquidity providers. A custom range position allows LPs to focus their liquidity within specific price ranges, thereby increasing capital efficiency and potential yields.

However, managing a custom-range position requires more active oversight and carries a higher risk of divergence loss, which occurs when the value of the assets diverges from each other within the liquidity pool.

This added complexity makes it crucial for LPs to thoroughly understand the risks and actively manage their positions to optimize outcomes.

You can click on any image in this guide to view it in fullscreen.

#### Navigate to the [Pools](https://www.orca.so/pools) page

Always check the URL carefully in your browser or wallet before connecting.

#### Connect your wallet

Make sure both the UI and your wallet are set to the Solana network.

#### Find your pool

Find the pool you wish to add liquidity to, you can either locate it in the pool list or use the search field.
**TIP:** You can search using the token name, ticker, or token mint address, but make sure to check carefully that you have selected the right token.


#### Open Liquidity Terminal

Once you have found your pool, Click on it and the pool's *Liquidity Terminal* will open.


#### Ensure `Custom` range is selected in the *Create Position* sidebar.

![](/images/image_157.jpg)

#### Adjust your range

Once `Custom` is selected, you can set your desired range using any of the following methods:

* By dragging the sliders in the *Create Position* sidebar.
* By dragging the range boundaries on the price chart.
* By selecting a preset ±% range.
* By free-typing a ±% range.
* By free-typing the prices in the lower and upper fields.
* By using the + and - buttons in the lower and upper fields.

![](/images/image_158.jpg)

#### Enter deposit amounts

Enter the amount you wish to deposit in one of the highlighted fields (you may need to scroll down). The other values will automatically adjust to match the required deposit ratio for your chosen range.
Alternatively, you can click `Max` in the corresponding deposit field to deposit the maximum quantity of tokens.

![](/images/image_159.jpg)

If you want to use *Autoswap*, which matches the position's deposit ratio by trading one token for the other within pair, please:
→ See the Autoswap guide for more details.

#### (Optional) Adjust your liquidity slippage

If required you can adjust your liquidity slippage by clicking on the `Liq. slippage` button.
→ See [**Understanding Slippage**](/trade/slippage) for more details.

#### Complete your deposit

Once you are satisfied with your deposit values, click `Deposit`.

![](/images/image_160.jpg)

#### Review your transaction

Review the details in your wallet—including any network fees—and approve the transaction.

**REVIEW CAREFULLY.** It is critical that you check your range and ensure the current price of the pool matches your intentions. Depositing liquidity at a price not consistent with wider market values may result in irreversible loss.

#### Deposit Complete! 🎉
You can click on `View Details` to view the deposit transaction on Solscan. Your wallet will now contain a *pool position NFT*. In your wallet, it will be displayed as a simple image with the warning "**DO NOT BURN**"


**DO NOT** sell or burn this NFT. You can send it to another wallet to transfer your position, but (whale forbid) please **DO NOT** burn or sell it, or you'll lose your liquidity!
Orca **CANNOT** help you recover any funds lost as a result of burning a pool position NFT.

#### Next Steps

You're now providing custom-range liquidity on Orca! Check your position anytime on the [Portfolio page](https://www.orca.so/portfolio) and see our [Managing Your Portfolio](/liquidity/manage/portfolio) guide for help with managing your new position.

---

### We'd Love to Hear from You!

**Need support or want to share feedback?**

* Open a support ticket directly from the Orca UI by clicking `Support`
* Reach out via [Discord](https://discord.gg/deRXbXWXk8) or Telegram

**Have suggestions, requests or feedback?**

* Share them by clicking `Feedback` in the Orca UI
* Use the [`#✍│feedback`](https://discord.gg/TdRtv4GCKF) channel on Discord