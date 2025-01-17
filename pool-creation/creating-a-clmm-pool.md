---
description: Intro on CLMM pool and farm creation
---

# Creating a CLMM Pool

{% hint style="warning" %}
_It's **highly suggested** to read this **entire guide** before creating a pool_
{% endhint %}

{% hint style="warning" %}
If you haven't heard about Concentrated liquidity we recommend reading the following [article](https://docs.raydium.io/raydium/liquidity-providers/providing-concentrated-liquidity/intro-on-concentrated-liquidity).
{% endhint %}

Similar to creating a liquidity pool and ecosystem farm, any project team or user can create a CLMM pool and farm on Raydium. CLMM pools are designed for advanced market making. They offer more capital efficiency to liquidity providers, and reduce slippage on swaps. By creating a farm, project teams can crowdsource liquidity from the community in a decentralized manner, which results in deeper liquidity and better prices for users.

**IMPORTANT - points to keep in mind before creating CLMM pool and farm:**

* \
  **Token selection**: any token on Solana token list can be used to create a CLMM pool. Each pool will consist of two tokens, usually what is considered a base and quote token.
* **To prevent duplicate pools**, there can only be one token pair for each fee-tier on Raydium.
* **Fee Tiers**: pool creators can choose from 4 fee tiers 0.01% - best for very stable assets 0.05% - best for pegged-assets and high volume pairs 0.25% - best for most pairs 1% - best for exotic
* **Starting price**: the number of Quote Tokens needed to purchase 1 Base Token.
* **Initial price range**: the interval of which the pool creator’s liquidity is initially provided upon pool creation. Initial liquidity will be concentrated in the initial price range.
* **Only the pool creator can create a farm** for the given CLMM pool. Pool creators can choose 2 token rewards. One of chosen reward mints must be related to the token pair. The remaining reward can be any SPL token. For example, if a pool is created for RAY-SOL, one reward can be any token on the Solana Token list but the other reward must be either RAY or SOL.
* **Rewards and APR**:
  * APR is a function of rewards, token price and liquidity in the pool, specifically the $value of rewards for a period divided by the $value of liquidity in the pool, then annualized. Determining suitable rewards emissions and APR for Constant Product AMMs is a difficult task but it is even more complex for Concentrated Liquidity AMMs.
  * Unlike constant product farms, liquidity providers compete for both trading fees and token emissions, which are divided among liquidity providers within the current trading range. Liquidity providers with a tighter range around the mid-price will earn a higher share of fees and token emissions.
* **Key points to consider when calculating rewards**:
  * **Liquidity around the mid-price:** How much liquidity do you want in the trading range and how much active liquidity do you want near the mid-price?
  * **Price of reward token:** The reward token price has a direct effect on APR % for the farm. You may want to estimate a price range over the farming period to estimate APR.
  * **APR calculation:** Raydium’s UI features three different [estimated APR](https://docs.raydium.io/raydium/concentrated-liquidity/estimated-apr-calculations) calculations to give concentrated liquidity providers and pool creators a reference for potential yield.
* **Rewards allocated to farms are final** and cannot be withdrawn once the farm is created. Extending or adjusting the rewards rate can only be done 72 hours prior to the end of the current farming period, make sure to read part 2 of the guide below for specifics!

## **Creating a CLMM pool**

{% hint style="warning" %}
CLMM pools should be live on the UI approx 5 minutes after creation.
{% endhint %}

Users and project teams can create a concentrated liquidity pool on Raydium in 3 easy steps.

After connecting your wallet, navigate to “Liquidity” on the top of the page. Click on the “Create" button on the top right of the page.

Select “Concentrated Liquidity” to get started!

1. **First, select tokens & fee tier**

The Base Token is the first token that appears in a token pair quotation. Consequently, the second token in the pair is a Quote Token. Quote Tokens represent the number of tokens needed to purchase 1 Base Token.

Common quote tokens include SOL, USDC or other stablecoins.

The selected fee is the amount traders will pay to trade the pair. Liquidity providers earn 100% of token emissions and 84% of trading fees, with 12% and 4% of fees allocated to RAY buybacks and treasury, respectively.

**Fee** **Tiers:** Pool creators can choose from 4 fee tiers

* 0.01% - best for very stable assets
* 0.05% - best for pegged-assets and high volume pairs
* 0.25% - best for most pairs
* 1% - best for exotic pairs

**2. Set the Starting Price & Range**

* The starting price determines the number of Quote Tokens needed to purchase 1 Base Token when the pool is created.
* Select a price range for your initial liquidity position of the pool. You can remove liquidity or create a new position with different price range at any time once the pool is live.
* The pool creation tool will automatically populate a price range that is 50% above and below the Starting Price. Pool creators can choose a custom range around the starting price. You can also choose to deposit in a full range.

The price of the token pair will change as the tokens are traded. If the price trades below the position’s min price, the position will then be comprised of 100% base token. If price trades above the max price, the position will effectively sell the base token and then be 100% comprised of the quote token.

**3. Deposit Amount**

The deposit amount represents the amount of Base and Quote tokens that will be used to add liquidity when the pool is initialized. The deposit ratio will be populated automatically based on previous settings. The amount of liquidity added for the Base and Quote token can be manually adjusted by the pool creator.

**4. Preview Pool and Confirm**

The pool creator can preview the pool after determining the deposit amount. Click “Confirm Deposit” and approve the transaction. Congratulations you have created a concentrated liquidity pool on Raydium!

Please note: Gas fees will be higher than usual due to the initialization transaction.

**IMPORTANT**: The concentrated liquidity pool will be created after approving the transaction. The pool creator cannot edit the starting price or initial liquidity until the pool opens for trading. However, after the pool is created the pool creator can manage a current position or add additional liquidity in a chosen range.

##
