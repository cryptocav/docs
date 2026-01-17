---
title: How to Create a Full-Range Position on Eclipse
description: Create a simple full-range liquidity position on Eclipse with reduced divergence loss risk.
icon: droplet
sidebarTitle: How to Create a Full-Range Position o...
---

The simplest way to provide liquidity on Orca is to create a full-range position. A full-range position is one that spreads your liquidity across the entire price range from 0 to ∞. In this sense, a full-range position is a close approximation to liquidity deposited in a traditional CPMM, sacrificing capital efficiency and enhanced yields but gaining ease of management and reduced exposure to divergence loss.

### Creating a Full-Range Position

* Navigate to the Liquidity page (https://www.orca.so/pools?chainId=eclipse).
* Ensure the UI and your wallet are set to the Eclipse network.

   * If you haven't done so already, connect your wallet.

   * Find the pool you wish to add liquidity to by locating it in the pool list or by searching using the search field.


   **TIP:** You can search using the token name, ticker, or token mint address, but make sure to check carefully that you have selected the right token.
* Click on the pool you wish to add liquidity to. The *liquidity sidebar* will open.

* Ensure `Full` is selected in the liquidity sidebar.

   ![](/images/image_132.jpg)
* Enter the amount to deposit in one of the highlighted fields. The other values will automatically adjust to match the deposit ratio for a full-range position.

   ![](/images/image_133.jpg)

   Alternatively, you can click on `Max` in a corresponding *Deposit Amount* box to deposit that quantity of tokens from your wallet.
* (Optional) Adjust your liquidity slippage by clicking on the `Liq. slippage` button. See [Understanding Slippage](/trade/slippage) for more details.
* Once you are satisfied with your deposit values, click `Deposit`.

   ![](/images/image_134.jpg)
* Review the details in your wallet, including payable network fees and approve.

  **REVIEW CAREFULLY.** It is critical that you check your range and ensure the current price of the pool matches your intentions. Depositing liquidity at a price not consistent with wider market values may result in irreversible loss.
* Deposit Complete!🎉


    You can click on `View Details` to view the deposit transaction on the Eclipse Explorer. Your wallet will now contain a *pool position NFT*. In your wallet, it will be displayed as a simple image with the warning "**DO NOT BURN**".

    
**DO NOT** sell or burn this NFT. You can send it to another wallet to transfer your position, but (whale forbid) please **DO NOT** burn or sell it, or you'll lose your liquidity!
Orca **CANNOT** help you recover any funds lost as a result of burning a pool position NFT.

If you need any support or have any feedback or suggestions, feel free to open a support ticket from the Orca UI by either clicking `Support` in the wallet menu, or on [Orca's Discord](https://discord.gg/orca-so), or [Orca's Telegram](https://t.me/orca_so).

If you have any suggestions for how-to guides, tutorials, or educational material you would like to see, please let Orca know on the Discord server in [#✍│feedback](https://discord.com/channels/798712664590254081/813323917649379389).