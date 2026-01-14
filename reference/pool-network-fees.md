---
title: Pool network fees
description: Understanding network fees for pool operations.
icon: book
---

Orca's innovative of adoption of tokenExtension NFTs for holding pool position information has delivered a virtually cost free LP experience for our users. You can read more about this in our [Medium blog post](https://medium.com/@orca-so/lower-costs-fully-refundable-fees-for-lp-positions-dc09f8f0ebe1).
Orca does not charge fees to create a pool, nor to create a position in an existing pool. However, network and rent fees are payable and if the *Match deposit ratio* function is used trading fees and network fees will also be payable on that transaction. Fees paid to mint the pool poition NFT and open associated accounts are refunded when the position is paid.
On occasion a network fee may still be charged to open store a TickArray, necessary for your selected range, these are not refundable
Users of the SDK can also openPosition without Metadata - for detail liaise with a Developer Advocate in [#❓│dev-questions](https://discord.com/channels/798712664590254081/838660851178274866).

### Solana Network Fees

| Network / Rent Fee | Typical SOL value | Refundable |
|---|---|---|
| Position creation rent fees | 0.0088 | Yes |
| Network Fee (non-SOL transaction¹)³ | 0.000010 | No |
| Network Fee (SOL transaction²)³ | 0.000005 | No |
| Priority Network Fee³ | variable⁵ | No |
| (uncommon) Account to store a TickArray⁴ | 0.07 | No |

¹ Where SOL is not tokenA or tokenB in a transaction.
² Where SOL is tokenA or tokenB in a transaction.
³ Network fees are paid per number of signers utilized in the transaction.
⁴ This fee is not common, and occurs in specific circumstances, it is possible for this fee to be charged twice with certain selected ranges, please see [here](/reference/faqs#why-was-i-charged-higher-network-fees-than-usual) for more detail.
⁵ Priority fees will vary depending on network state, note your wallet may also apply a priority fee.

### Eclipse Network Fees

| Network / Rent Fee | Typical ETH value | Refundable |
|---|---|---|
| Position creation rent fees | 0.000086 | Yes |
| Network Fee¹ | 0.000010 | No |
| Priority Network Fee¹ | variable³ | No |
| (uncommon) Account to store a TickArray² | 0.00069 | No |

¹ Network fees are paid per number of signers utilized in the transaction.
² This fee is not common, and occurs in specific circumstances, it is possible for this fee to be charged twice with certain selected ranges, please see [here](/reference/faqs#why-was-i-charged-higher-network-fees-than-usual) for more detail.
³ Priority fees will vary depending on network state, note your wallet may also apply a priority fee.

### Pool Creation Fees

When you create a new pool there will be additional fees to pay, as well as applicable fees from above. These fees will vary depending on the fee rate selected and the chosen *Price range for initial deposit.* The cost will be higher if more TickArrays need to be initialized. Tick size is proportional to fee rate, creation costs will be higher for a wider range on a lower fee rate pool. The UI will provide an estimate of fees.

![](/images/image_72.jpg)