---
description: Raydium now supports the new Token-2022 Solana token program
---

# Token-2022 Support

The [**Token-2022 program**](https://spl.solana.com/token-2022) **is a new token standard on Solana** that provides additional fungible and non-fungible token functionality by enabling token creators to use a variety of [extension](https://spl.solana.com/token-2022/extensions)[s](https://spl.solana.com/token-2022/extensions) when minting tokens on Solana. Raydium’s permissionless Concentrated Liquidity Market Maker (CLMM) pools now support Token-2022 assets.

## **Interacting with Token-2022 assets on Raydium**

Token-2022 on Raydium is an advanced feature. As such, **users will have to manually enter the mint address in the search bar to locate a tradable asset**. For the time being, Token-2022 assets will not display a token name or logo unless manually added by a user. Anyone interacting with a Token-2022 asset will be required to confirm and acknowledge the risks associated with the assets they are interacting with.

Users that manually confirm interactions with a Token-2022 asset will then be able to route swaps through other pools that contain Token-2022 assets. Users who have not confirmed a Token-2022 asset or that are only swapping standard SPL tokens will only route through pools that contain standard SPL tokens.

**Transfer Fee Extension:**

A common Token-2022 extension is Transfer Fees. This mint extension allows token creators to charge a fee for each token transfer that is executed programmatically and goes to a token account determined by the token creator. Transfer fees are displayed on the Raydium UI when possible, however Raydium has no control over any Token-2022 transfer fees. Transfer fees may apply to token interactions like swaps or even adding and removing liquidity. Transfer fees are not necessarily immutable, which means the token issuer could **update the transfer fee at any time without warning.**

**Unsupported Token-2022 Extensions**

Raydium’s permissionless Concentrated Liquidity Market Maker (CLMM) pools now support Token-2022 assets. However, some extension types are limited on the program-level. Out of an abundance of caution, Token-2022 assets with the following extensions enabled are currently unable to create a permissionless pool:

**Permanent Delegate**: With Token-2022, it's possible to specify a permanent account delegate for a mint. This authority has unlimited delegate privileges over any account for that mint, meaning that it can burn or transfer any amount of tokens.

**Non-Transferable Tokens**: The Non-Transferable mint extension allows for "soul-bound" tokens that cannot be moved to any other entity. This extension is very similar to issuing a token and then freezing the account but allows the owner to burn and close the account if they want.

**Default Account State**: A mint creator may use the DefaultAccountState extension, which can force all new token accounts to be frozen. **Confidential Transfers**: With Token-2022, it's possible to use ZK proofs to encrypt balances and transfers amounts, providing transaction privacy to token holders. **Transfer Hook**: A mint creator can set custom transfer parameters to execute functions upon transfers of the token.
