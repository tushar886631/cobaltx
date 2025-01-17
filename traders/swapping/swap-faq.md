# Swap FAQ



<details>

<summary>What is a swap?</summary>

A swap is an exchange of a token for another.

&#x20;Raydium swaps are performed by its smart contracts deployed on Solana. They are executed against the depositors' liquidity. Hence, they don't require any intermediary, unlike trades on custodian exchanges.

&#x20;The exchange rate is calculated following predefined mathematical formulas available on [Git Hub](https://github.com/raydium-io/raydium-docs/tree/master/dev-resources) and accounting for the available tokens in the pools.

</details>

<details>

<summary>Liquidity</summary>

Raydium's liquidity comes from its own liquidity pools. Raydium routing engine can through several pools perform a swap to find the best execution and limit slippage.

</details>

<details>

<summary>Fees</summary>

When you swap in a Raydium liquidity pool, the fees charged range from 1% to 0.01% depending on the pool you are swapping through. Those fees are distributed following this repartition: AMM pools

* 88% is redeposited into the liquidity pool and acts as a reward for liquidity providers.
* 12% is used to buy back the RAY token

CLMM pool

* 84% is redeposited into the liquidity pool and acts as a reward for liquidity providers.
* 12% is used to buy back the RAY token
* 4% goes to the protocol treasury

Network fee: A nominal amount of SOL is also required to process Solana network fees on each trade. Most transactions cost between 0.0001 — 0.001 SOL.

</details>

<details>

<summary>What is price impact?</summary>

Price impact is the difference between the current market price and the expected price for a trade. Price impact is primarily determined by the size of your trade relative to the amount of liquidity in the pool. As the number of tokens you buy from the pool increases, the price of the token increases as well. This unfavorable change in price is called price impact.

If you are swapping in a pool with very low liquidity, you may receive a very poor price for your swap. If you see a high price impact when swapping, try trading a smaller amount or swapping in a pool with higher liquidity.

</details>

<details>

<summary>Slippage tolerance</summary>

Slippage is the difference between the expected price of a swap and its execution price.

Raydium allows users to set their slippage tolerance determining the maximum difference between the expected and execution price. If the slippage exceeds the user's choice, the swap won't be executed.

Setting a high slippage tolerance may result in an unfavorable swap.

</details>

<details>

<summary>Why did my transaction fail?</summary>

**Insufficient SOL:** SOL is required to pay network fees (gas), it's recommended to keep at least 0.05 SOL in your wallet to ensure smooth transactions.

**Slippage Tolerance:** Transactions will fail if the price of the underlying pool moves past your Slippage Tolerance. Try increasing your slippage tolerance on the Swap page.

**Approving Transactions:** If you see the “Making Transaction” notification in the lower lef&#x74;**-**&#x68;and corner of your screen, you will need to approve the transaction in your SPL wallet.

</details>

<details>

<summary>Can I swap on mobile?</summary>

Yes! You'll need to use the built-in browser or your [SPL mobile wallet](https://docs.raydium.io/raydium/trading-on-serum/spl-wallets).

</details>

<details>

<summary>Wrapped Sol</summary>

There are rare occurrences where the swap and/or cleanup of your transaction don't go through. You may end up with some wrapped Sol. No worries! Wrapped Sol is a version of Sol used by the smart contracts on-chain and is redeemable for Sol 1:1.

Go to [https://raydium.io/swap](https://raydium.io/swap), the interface will automatically detect the wrapped Sol and offer to swap them for Sol.

</details>

<details>

<summary>Your question is not answered in this FAQ?</summary>

No worries, you can join the Raydium [Discord](https://discord.com/invite/6EvFwvCfpx) or [Telegram](https://t.me/raydiumprotocol) for 24/7 support! Raydium's community managers will be more than happy to help you.

</details>
