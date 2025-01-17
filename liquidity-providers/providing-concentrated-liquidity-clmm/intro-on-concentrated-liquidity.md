# Intro on Concentrated Liquidity

## **What is a CLMM?**

**Concentrated Liquidity Market Maker (CLMM)** pools allow liquidity providers to select a specific price range at which liquidity is active for trades within a pool. This is in contrast to constant product Automated Market Maker (AMM) pools, where all liquidity is spread out on a price curve from 0 to ∞. For LPs, CLMM design enables capital to be deployed with higher efficiency and earn increased yield from trading fees. For traders, CLMMs improve liquidity depth around the current price which translates to better prices and lower price impact on swaps.

While CLMMs come with the benefits of higher capital efficiency, [impermanent loss](https://www.gemini.com/cryptopedia/decentralized-finance-impermanent-loss-defi) is magnified by the design, so a **full understanding the implications of impermanent loss and concentrated liquidity is critical!**

The design for CLMMs means capital can be more efficiently allocated towards market making within a price range. However, users should be aware that actively monitoring positions and market fluctuations is critical to mitigating the potential for increased impermanent loss.

## **How do liquidity price ranges work?**

In CLMM pools, users are able to select a specific price range in which to provide liquidity. LPs earn fees in proportion to their share of the liquidity at the current price. As such, LPs have a strong incentive to actively manage positions to ensure the current price of a pool is actively trading within their selected price range.

**If price moves out of the selected price range**, a position will no longer actively trade or earn fees and the LP may experience significant [impermanent loss](https://www.gemini.com/cryptopedia/decentralized-finance-impermanent-loss-defi). In a standard AMM pool, if the price of a base token rises it means that users are trading the quote token for the base token. As such, the pool and LPs now have more of the quote token and less of the base token.

CLMMs work in the same manner, however this is accelerated within the selected price range. For example, if the price trades below the position's min price, the position will then be comprised of 100% base token. If price trades above the max price, the position will effectively sell the base token and then be 100% comprised of the quote token.

Continue to the next page to learn more about providing liquidity in concentrated pools!
