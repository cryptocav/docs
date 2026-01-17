---
title: Orca on Eclipse Launch FAQ
description: Common questions about Orca on Eclipse answered.
icon: rocket
---

#### Is Eclipse a Solana L2?

Not quite, Eclipse is a modular L2, which settles on the Ethereum Mainnet. The Solana Virtual Machine is used for execution.

#### Will my Solana based assets be available when I connect to Orca on Eclipse?

No, Solana and Eclipse are completely separate environments. While your address will be the same, your assets will be held on separate chains, so cannot be accessed from both chains at the same time.

#### How do I get my assets from Solana to Eclipse?

You can bridge assets using the [Hyperlane Nexus Bridge](https://www.usenexus.org/) supported tokens are currently limited but will increase as the chain matures. Other bridges will likely launch on Eclipse, but it is important you do your own research before using any app.

#### Is SOL used for transaction fees on Eclipse?

No, Eclipse uses ETH for gas, you will need to bridge some ETH from Ethereum Mainnet in order to transact on Eclipse, you can use this [guide](/get-started/eclipse/eclipse-bridging-eth) to learn how to use the [Eclipse Canonical Bridge](https://bridge.eclipse.xyz/).

#### How do I switch to Eclipse on Orca?

The Orca UI incorporates a simple switching mechanism, the Network Selection Menu, a simple guide can be found [here](/get-started/eclipse/eclipse-connecting)

#### As an LP will I earn bigger yields on Eclipse?

Yields are generated from trading fees, how much an LP earns will depend on trading volume, chosen strategies, and the activities of other LPs. It cannot be said that LPs will earn more or less on Eclipse, but the opportunities for Orca users will be increased.

#### Can I bridge assets back to Solana from Eclipse?

Yes, the Hyperlane Nexus Bridge allows users to bridge assets from Eclipse to Solana. Supported tokens are currently limited but will increase as the chain matures. Other bridges will likely launch on Eclipse, but it is important you do your own research before using any app.

#### Can I create new Orca pools when using Eclipse?

Yes, you can create new pools when using Orca on Eclipse in the same way as on Solana.

#### Can I use my normal Solana wallet on Eclipse?

The number of wallets that support Eclipse is currently limited. If you're already using a Solana wallet other than Backpack, you can easily import your existing address into Backpack by using your seed phrase. Simply follow the relevant guide provided [here](https://support.backpack.exchange/all-articles?cat=Wallet+Import%2FRecover) to complete the process.

#### Why does ETH have the same mint address on Eclipse as SOL does on Solana?

The mint address represents the native coin within the SVM (Solana Virtual Machine) environment. On Solana, the native coin is SOL, while on Eclipse, it is ETH. Both native coins share the same mint address, So11111111111111111111111111111111111111111, on their respective chains.

When these native coins are wrapped—such as for use in liquidity pools or trades, rather than for paying transaction fees—their mint address changes to So11111111111111111111111111111111111111112 on their respective chain.

#### Does SOL exist on Eclipse?

Yes, SOL can be bridged to Eclipse using the [Hyperlane Nexus Bridge](https://www.usenexus.org/). SOL bridged through Hyperlane Nexus has the mint address [BeRUj3h7BqkbdfFU7FBNYbodgf8GCHodzKvF9aVjNNfL](https://explorer.eclipse.xyz/address/BeRUj3h7BqkbdfFU7FBNYbodgf8GCHodzKvF9aVjNNfL)

#### Will there be opportunities for LPs to earn rewards on Orca on Eclipse

Absolutely, Orca will still incentivize pools from time to time, by onboarding yourself onto Eclipse you can be ready to take advantage of incentives when they are announced.