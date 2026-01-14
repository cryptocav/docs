---
title: How to Create a Full-Range Position on Solana
description: Create your first full-range liquidity position.
icon: droplet
sidebarTitle: How to Create a Full-Range Position o...
---

### Creating a Full-Range Position

The simplest way to provide liquidity on Orca is to create a full-range position. A full-range position is one that spreads your liquidity across the entire price range, from 0 to infinity (∞). This type of position closely approximates liquidity deposited in a traditional CPMM. It sacrifices capital efficiency and the potential for enhanced yields, but gains ease of management and reduced exposure to divergence loss.

You can click on any image in this guide to view it in fullscreen.

#### Navigate to the [Pools](https://www.orca.so/pools) page

Always check the URL carefully in your browser or wallet before connecting.

#### Connect your Wallet

Make sure both the UI and your wallet are set to the Solana network.

#### Find your pool

Find the pool you wish to add liquidity to, you can either locate it in the pool list or use the search field.
**TIP:** You can search using the token name, ticker, or token mint address, but make sure to check carefully that you have selected the right token.

![](/images/image_64.jpg)

#### Open Liquidity Terminal

Once you have found your pool, Click on it and the pool's *Liquidity Terminal* will open.

![](/images/image_65.jpg)

#### Ensure `Full` is selected in the *Create Position* sidebar

![](/images/image_66.jpg)

#### Enter deposit amounts

Enter the amount to deposit in one of the highlighted fields.

The other values will automatically adjust to match the deposit ratio for a full-range position.

Alternatively, you can click `Max` in the corresponding deposit field to deposit the maximum quantity of tokens.

If you want to use *Autoswap*, which matches the position's deposit ratio by trading one token for the other within the pair, please:
→ See the Autoswap guide for more details.

![](/images/image_67.jpg)

#### (Optional) Adjust your liquidity slippage

If required you can adjust your liquidity slippage by clicking on the `Liq. slippage` button.
→ See [**Understanding Slippage**](/reference/educational-documents/understanding-slippage) for more details.

#### Complete your deposit

Once you are satisfied with your deposit values, click `Deposit`.

![](/images/image_68.jpg)

#### Review your transaction

Review the details in your wallet—including any network fees—and approve the transaction.

**REVIEW CAREFULLY.** It is critical that you check your range and ensure the current price of the pool matches your intentions. Depositing liquidity at a price not consistent with wider market values may result in irreversible loss.

#### Deposit Complete!🎉

You can click on `View Details` to view the deposit transaction on Solscan. Your wallet will now contain a *pool position NFT*. In your wallet, it will be displayed as a simple image with the warning "**DO NOT BURN**".

**DO NOT** sell or burn this NFT. You can send it to another wallet to transfer your position, but (whale forbid) please **DO NOT** burn or sell it, or you'll lose your liquidity!

Orca **CANNOT** help you recover any funds lost as a result of burning a pool position NFT.

#### Next Steps

You're now providing full-range liquidity on Orca! Check your position anytime on the [Portfolio page](https://www.orca.so/portfolio) and see our [Managing Your Portfolio](/liquidity/managing-portfolio) guide for help with managing your new position.

---

### We'd Love to Hear from You!

**Need support or want to share feedback?**

* Open a support ticket directly from the Orca UI by clicking `Support`
* Reach out via [Discord](https://discord.gg/deRXbXWXk8) or Telegram

**Have suggestions, requests or feedback?**

* Share them by clicking `Feedback` in the Orca UI
* Use the [`#✍│feedback`](https://discord.gg/TdRtv4GCKF) channel on Discord