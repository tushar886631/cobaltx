---
description: >-
  Raydium trade API is the fastest and easiest way to interact with Raydium
  liquidity. It allows you to swap for any asset with 2 requests and a
  signature.
---

# Trade API

## Get quote parameters



| Parameter   |  Type  | Required | Description                                                     |
| ----------- | ------ | -------- | --------------------------------------------------------------- |
| inputMint   | string | yes      | Input token mint address                                        |
| outputMint  | string | yes      | Output token mint address                                       |
| amount      | number | yes      | Either inputAmount or outpoutAmount depending on the swap mode. |
| slippageBps | number | yes      | Slippage tolerance in base points (0.01%).                      |

## Post parameters

<table><thead><tr><th width="215">Parameter</th><th>Parameter</th><th>Required</th><th>Description</th></tr></thead><tbody><tr><td>version</td><td>string</td><td>yes</td><td>Use 'V0' for versioned transaction, and 'LEGACY' for legacy transaction.</td></tr><tr><td>wrapSol</td><td>boolean</td><td>no</td><td>Need to be true to accept SOL as inputToken.</td></tr><tr><td>unwrapSol</td><td>boolean</td><td>no</td><td>Need to set to true to unwrap wSol received as outputToken.</td></tr><tr><td>computeUnitPriceMicroLamports</td><td>string</td><td>yes</td><td><p>You can type it in manually or use Raydium priority fee API to set an automatic amount with 'String(data.data.default.h)'. The 'h' here stands for high priority.</p><p>'vh' for very high and 'm' for medium are also accepted value.</p></td></tr><tr><td>wallet</td><td>string</td><td>yes</td><td>pubkey</td></tr><tr><td>inputTokenAccount</td><td>string</td><td>no</td><td>default to ATA</td></tr><tr><td>outpoutTokenAccount</td><td>string</td><td>no</td><td>default to ATA</td></tr></tbody></table>
