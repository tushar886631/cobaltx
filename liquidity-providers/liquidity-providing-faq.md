# Liquidity providing FAQ



<details>

<summary>APR</summary>

APRs (annual percentage rate) displayed on Raydium are extrapolations of the pool and farm yield based on the daily (by default) or weekly or monthly performance.&#x20;

The provided APRs serve as examples only, and it's important to note that previous performance does not ensure future profits.

Raydium displays 3 methods for APR estimation on its CLMM pools, please read this [article](https://docs.raydium.io/raydium/liquidity-providers/providing-concentrated-liquidity-clmm/estimated-apr-calculations#overall-pool-estimated-apr) to understand the way each method works.

</details>

<details>

<summary>Where's the yield coming from?</summary>

APR displayed on pools:

The yield displayed on pools comes from the maker fees (fees paid for swaps going through the pool).

* And reward emissions for CLMM pools.

APR displayed on ecosystem farms:&#x20;

Include both maker fees and the farms' emissions.

</details>

<details>

<summary>Can I withdraw my liquidity at any time?</summary>

Yes, you can redeem liquidity tokens for a proportional share of the pool at any time.

For standard AMM pools: If you staked your LP tokens in a farm, you'll need to unstake them first.

</details>

## CLMM pools

<details>

<summary>What's the benefit of providing liquidity on Raydium CLMM pools?</summary>

[CLMMs](https://raydium.medium.com/introducing-permissionless-concentrated-pools-farms-bf0a716bcdbd) - Concentrated Liquidity Market Makers - are designed for advanced liquidity provision on DEXs. While the past iterations of Raydium's liquidity pools work on the constant product model with liquidity provided along an X\*Y=K price curve, assets were reserved for all prices on the interval \[0;∞] resulting in the majority of the liquidity never being used to earn fees.

CLMMs allow LPs to concentrate their liquidity on custom price ranges providing them the opportunity to leverage or provide more liquidity at desired prices. Solving the inactive liquidity problem, CLMM provides the best capital efficiency while increasing the liquidity depth around the actual price translating to lower slippage on swaps.

**Allowing liquidity providers to deposit liquidity in a chosen range, CLMM pools increase both the yield and the IL risk.** Moreover, giving liquidity providers more granularity while providing liquidity allows LPs to adopt different risk profiles depending on the directional exposure one wants to take on token pairs.

</details>

<details>

<summary>How to farm emissions on CLMM pools?</summary>

No additional action is needed! If there is an active farm on the CLMM pool, the rewards are distributed alongside the maker fees.

</details>

<details>

<summary>Where are my LP tokens?</summary>

For CLMM pools you won't receive LP tokens per se. Instead, you'll get a position NFT that represents your position in the pool (liquidity and price range). If it is burned or otherwise lost, the associated liquidity cannot be withdrawn or retrieved. It is possible to send or trade a pool position NFTs. However, if sold any associated liquidity is also sold and will no longer be held by the original owner.

When closing a position and withdrawing liquidity, the network fees for the NFT mint will be reimbursed.

</details>

## More



<details>

<summary>Why did my transaction fail?</summary>

**Insufficient SOL:** SOL is required to pay network fees (gas), it's recommended to keep at least 0.05 SOL in your wallet to ensure smooth transactions.

**Slippage Tolerance:** Transactions will fail if the price of the underlying pool moves past your Slippage Tolerance. Try increasing your slippage tolerance on the Swap page.

**Approving Transactions:** If you see the “Making Transaction” notification in the lower lef&#x74;**-**&#x68;and corner of your screen, you will need to approve the transaction in your SPL wallet.

</details>

<details>

<summary>Your question is not answered in this FAQ?</summary>

No worries, you can join the Raydium [discord](https://discord.com/invite/6EvFwvCfpx) or [telegram](https://t.me/raydiumprotocol) for 24/7 support! Community managers will be more than happy to help answer questions.

</details>
