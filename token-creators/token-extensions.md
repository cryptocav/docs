---
title: Token Extensions
description: Learn about supported token extensions.
icon: coins
---

### Token Extensions Overview

Token Extensions are advanced functionality designed specifically to meet the need of businesses with compliance obligations. They are added feature sets designed with regulatory obligation in mind, and may break Whirlpool’s functionality if integrated incorrectly.

Orca currently supports a set of Token Extension, with some requiring Token Badge permission. The extensions support status is listed on the table below.

Token Badge is only granted via an explicit, case by case review by the Orca Team. Due to some extension’s ability to compromise Orca’s programs, Token Badges are not issued lightly.

If your project has a reasonable requirement for using Token Extensions, you may reach out to Orca. Please fill out the contact form linked at the bottom of the page.

For a deeper dive into TokenExtensions, please check out [Solana Foundation’s White Paper](https://cdn.builder.io/o/assets%2Fce0c7323a97a4d91bd0baa7490ec9139%2F83c26b9268f64400b8eb67442579a31a?alt=media&token=525415b0-d3ea-48d7-83d6-0fb0d9e522c6).

### Extension Functionalities and Support Status

| Extensions | Functionality | Support Status |
|---|---|---|
| TransferFee | Allow transfer fees to be charged on each transfer and sent to a defined account. | Supported |
| MemoTransfer | Requiring all incoming transfers to include a memo instruction immediately before the transfer function. | Supported |
| MetadataPointer | Allow token creator to designate an address for the canonical metadata. | Supported |
| TokenMetadata | Allow storage of token info such as name, symbol, and key parameters. | Supported |
| InterestBearing | Allows tokens to be set with an interest rate, which continuously compounds. | Supported |
| ConfidentialTransfer (non-confidential transfer only) | Allow confidential transfers between participating users without revealing the amount of the transfer. | Supported, Non-confidential transfer only |
| PermanentDelegate | Allow for the transfer of any amount of tokens from any account to another or even burn them. | TokenBadge required |
| TransferHook | Allows calling specific programs with each token transfer | TokenBadge Required |
| MintCloseAuthority | Allows owners to close mint accounts and reclaim the on the mint account. | TokenBadge Required |
| DefaultAccountState | Allows mints to predefine the state of a token account upon creation. An account can be either frozen or initialized. | TokenBadge Required |
| FreezeAuthority (not extension, but restricted) | Allows token creator to freeze or thaw individual token accounts associated with their token | TokenBadge Required |
| NonTransferable | Enables "soul-bound" tokens that cannot be transferred to other accounts | Not Supported |
| GroupPointer | Allow token creator to designate a group of accounts for its metadata. | Not Supported |
| Member | Describes configurations for a group member, such as group address and a member's number. | Not Supported |
| MemberPointer | Allows the token creator to designate a member account (see above) that describes the mint. | Not Supported |
| Native mint for Token-2022 (not extension, but restricted) | - | Not Supported |
| All other extensions not listed in the above | - | Not Supported |

### Q & A

For more technical deep dive into Token Extensions, feel free to check out our [developer documentation on TokenExtension](https://dev.orca.so/Architecture%20Overview/TokenExtensions%20Support), and our [smart contract implementation](https://github.com/orca-so/whirlpools/pull/134). Please feel free to ask questions in our [Public Discord channel](https://discord.com/channels/798712664590254081/838660851178274866).

If you have a need to gain TokenBadge permission, you can [contact us](https://discord.gg/wm8mMEb3hc).

Thanks! 🐳