---
title: How to create a Custom Range Position on Eclipse
description: Create custom-range positions on Eclipse.
icon: droplet
sidebarTitle: How to create a Custom Range Position...
---

While providing liquidity to a concentrated liquidity pool offers multiple benefits, it is an advanced feature best suited for experienced liquidity providers. A custom range position allows LPs to focus their liquidity within specific price ranges, thereby increasing capital efficiency and potential yields.

However, managing a full-range position requires more active oversight and carries a higher risk of divergence loss, which occurs when the value of the assets diverges from each other within the liquidity pool.

This added complexity makes it crucial for LPs to thoroughly understand the risks and actively manage their positions to optimize outcomes.

* Navigate to the Liquidity page (<https://www.orca.so/pools?chainId=eclipse>).
* Ensure the UI and your wallet are set to the Solana network.

   ![](/images/image_39.jpg)
* If you haven't done so already, connect your wallet.

   ![](/images/image_40.jpg)
* Find the pool you wish to add liquidity to by locating it in the pool list or by searching using the search field.

   ![](/images/image_41.jpg)

   **TIP:** You can search using the token name, ticker, or token mint address, but make sure to check carefully that you have selected the right token.
* Click on the pool you wish to add liquidity to. The *liquidity sidebar* will open.

   ![](/images/image_42.jpg)
* Ensure `Custom` range is selected in the liquidity sidebar.

   ![](/images/image_43.jpg)
* After selecting Custom range the desired range can be changed in five ways:

   * By dragging the sliders.
   * By selecting a preset ±% range.
   * By free-typing a ±% range.
   * By free-typing the prices in the lower and upper fields.
   * By using the + and - buttons in the lower and upper fields.

   ![](/images/image_44.jpg)
* Enter the amount you wish to deposit in one of the highlighted fields (you may need to scroll down). The other values will automatically adjust to match the required deposit ratio for your chosen range.

   ![](/images/image_45.jpg)

   (Optional) Activate the `Autoswap` toggle to automatically trade between the paired tokens to match your desired deposit.
   Alternatively, you can click on `Max` to deposit that quantity of tokens from your wallet.
* (Optional) Adjust your liquidity slippage by clicking on the `Liq. slippage` button. See [Understanding Slippage](/reference/educational-documents/understanding-slippage) for more details.
* Once you are satisfied with your deposit values, click `Deposit`.

    ![](/images/image_46.jpg)
* Review the details in your wallet, including payable network fees and approve.

  **REVIEW CAREFULLY.** It is critical that you check your range and ensure the current price of the pool matches your intentions. Depositing liquidity at a price not consistent with wider market values may result in irreversible loss.
* Deposit Complete!🎉

    ![](/images/image_47.jpg)

    You can click on `View Details` to view the deposit transaction on the Eclipse Explorer. Your wallet will now contain a *pool position NFT*. In your wallet, it will be displayed as a simple image with the warning "**DO NOT BURN**".

    ![](/images/image_48.jpg)

**DO NOT** sell or burn this NFT. You can send it to another wallet to transfer your position, but (whale forbid) please **DO NOT** burn or sell it, or you'll lose your liquidity!
Orca **CANNOT** help you recover any funds lost as a result of burning a pool position NFT.

If you need any support or have any feedback or suggestions, feel free to open a support ticket from the Orca UI by either clicking `Support` in the wallet menu, or on [Orca's Discord](https://discord.gg/orca-so), or [Orca's Telegram](https://t.me/orca_so).

If you have any suggestions for how to guides, tutorials, or educational material you would like to see, please let Orca know on the Discord server in [#✍│feedback](https://discord.com/channels/798712664590254081/813323917649379389).