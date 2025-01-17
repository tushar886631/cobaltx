---
layout:
  title:
    visible: true
  description:
    visible: false
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
---

# 🧬 The Raydium Protocol

**An on-chain order book AMM powering the evolution of DeFi**

In less than a year, Decentralized Finance (DeFi) has grown from a buzz word to an entire ecosystem that is setting new standards for personal financial autonomy and trust. DeFi embodies everything that decentralization and cryptocurrency is about. It allows everyone to access tools that have traditionally been the domain of large banks, corporations, venture funds and trading firms, without sacrificing autonomy.

Ethereum brought decentralized trading, lending, and yield earning to anyone with an internet connection. Furthermore, it did that while ensuring transparency, interoperability, and immutability through the blockchain. However, the current state of DeFi is far from perfect.

## Legacy Blockchains are not Ready for DeFi <a href="#legacy-blockchains-are-not-ready-for-defi" id="legacy-blockchains-are-not-ready-for-defi"></a>

While DeFi holds enormous opportunity, it is very much limited by outdated blockchains.

* **💸 DeFi transactions are expensive** In a short time, we have seen gas fees jump to a level that completely wipes out potential earnings. Slow transactions exacerbate this as users bid up the price of gas, with failed transactions multiplying losses. As interacting with DeFi becomes prohibitively expensive, we are once again seeing common users left behind.
* **🧩 Market fragmentation** The nature of automated market makers (AMMs) on Ethereum means that liquidity is fragmented, and liquidity pools on one protocol are walled off from those on others. Without any central order book to aggregate across pools, competition by AMMs for liquidity is intense and users see no benefit from liquidity held on other platforms. This will also be true for shard-based blockchains, like eth2 and Polkadot.
* **🧮 Features are limited** Many trading features considered standard on centralized exchanges, like limit orders, are difficult to implement efficiently on Ethereum DEXs due to slow transaction speeds and prohibitively high gas fees.

## **💡** The Vision for a New Industry Standard <a href="#the-vision-for-a-new-industry-standard" id="the-vision-for-a-new-industry-standard"></a>

In the DeFi summer of 2020, Serum launched a decentralized exchange with an on-chain order book. This order book was built on Solana, a high speed blockchain with extremely low transaction costs. This new paradigm presented a massive opportunity to solve the biggest issues in DeFi, by building a fast, efficient AMM that could leverage existing order book flow as well as supply the liquidity in its own pools to the rest of the ecosystem. The Solana ecosystem has pivoted to support OpenBook, a community led on-chain order-book, the opportunity for a hybrid AMM that shares pool liquidity to an order-book remains.

Raydium aims to be the solution for the issues faced with AMMs on Ethereum. By building on Solana, which features faster and cheaper transactions, users will be able to trade on AMMs without being left out of the game due to ridiculously high fees. Raydium solves the liquidity issue by utilizing a central order book.

With this in mind, Raydium was born.

## **🧬** The Raydium Protocol: **An Ecosystem Sustaining AMM** <a href="#the-raydium-protocol-an-ecosystem-sustaining-amm" id="the-raydium-protocol-an-ecosystem-sustaining-amm"></a>

Unlike other AMM platforms, Raydium provides on-chain liquidity to a central limit order book, meaning that Raydium’s users and liquidity pools have access to the order flow and liquidity of the OpenBook ecosystem, and vice versa. All of this is supercharged by building on Solana, an incredibly fast and efficient blockchain.

Raydium currently uses constant function K = Y\*X. This equation has the special property that it is stateless and given any two tokens, without any information about their relative prices or value, it can provide “infinite” liquidity to traders. Raydium utilizes this equation and prices orders on the orderbook according to the Fibonacci sequence to provide up to 20 orders at a variety of prices with spreads as small as 20bps between them. This is an optimized solution to fit the exchange instructions onto a single Solana transaction. In the future, it’s expected that other liquidity providing models will be employed to take advantage of oracles and increased liquidity usage.

Additionally, liquidity providers will be able to generate rewards from trading fees for contributing. Key pools will be incentivized with RAY tokens as farming rewards. Projects that want to reward users for providing liquidity can also add additional reward tokens. When new projects launch, they can utilize Raydium to create a new trading market and provide immediate liquidity to it. This way projects can get up and running and give traders a chance to effortlessly buy in.

## **🐛** Evolution is Imminent <a href="#evolution-is-imminent" id="evolution-is-imminent"></a>

As Raydium progresses as a foundation for Solana liquidity, it aims to partner with other DeFi and AMM communities and provide support to build out their products on Solana. This will bring both additional liquidity and faster, more efficient DeFi protocols to the ecosystem.

Raydium offers an avenue for evolution, where projects and individuals can swiftly enter the Solana universe to leverage its distinct advantages in speed and efficiency. Faster transactions, significantly lower fees, and ecosystem-wide liquidity are essential if the people, projects, and protocols of DeFi are to evolve. We hope to see you on the other side.
