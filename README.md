# Kessai
![Kessai logo](assets/logo.png)

**Instant stablecoin invoice settlement for Japanese SMEs, funded by a 10M yen liquidity pool.**

## Overview

Kessai lets small businesses in Japan get paid immediately on B2B invoices by converting them into stablecoin-backed instant payments, instead of waiting the usual 30-60 days. A liquidity pool, seeded with a 10M yen budget, advances the funds and earns a small discount fee, while buyers repay on the original due date. This creates a sustainable, yield-generating lending business from day one.

## Problem

Japanese SMEs and freelancers routinely wait 30-60 days for B2B invoice payment. This delay creates serious cash flow problems, and traditional banks are too slow and too expensive to offer short-term financing that solves it.

## Solution

Kessai tokenizes approved invoices on-chain and instantly advances stablecoins from a liquidity pool to the SME. When the buyer pays on the original due date, the pool is repaid plus a small discount fee, which becomes yield for liquidity providers.

## Features (MVP)

- Upload & verify invoice, mint on-chain claim via Solana program
- Instant stablecoin payout to SME wallet from the liquidity pool
- Automated repayment collection from the buyer on the due date
- LP dashboard showing pool yield and risk exposure
- Simple KYC / credit-scoring flow for first pilot invoices

## Tech Stack

- Anchor (Solana smart contracts)
- Solana Pay
- USDC
- Next.js
- Supabase
- Chainlink / Pyth price feeds
- Metaplex (invoice NFT)

## How It Works

```
SME uploads invoice
       |
       v
KYC + credit check (Supabase)
       |
       v
Invoice minted as NFT claim (Anchor + Metaplex, on Solana)
       |
       v
Liquidity pool pays SME instantly in USDC (Solana Pay)
       |
       v
Buyer repays pool on due date -> pool earns discount fee
       |
       v
LP dashboard tracks yield & risk (Chainlink/Pyth price feeds)
```

All invoice claims, pool accounting, and repayment logic run on-chain via the Anchor program, with Supabase handling off-chain data like KYC status and credit scores.

## Roadmap

- Run a pilot with 5-10 real SMEs using the seed liquidity pool
- Add a credit-scoring model and an insurance/reserve fund for defaults
- Partner with Japanese accounting SaaS providers for invoice data integration

## Pitch

- [Pitch deck (PDF)](docs/pitch.pdf)
- [Pitch script](docs/pitch-script.md)

## Team

- Name / Role — placeholder
- Name / Role — placeholder
- Name / Role — placeholder

Built for the Colosseum hackathon (Solana and other chains).

---

🎬 Pitch video: [docs/pitch-video.mp4](docs/pitch-video.mp4)


## Prototype

Live prototype: https://haruki1234567.github.io/kessai/

The source is [docs/index.html](docs/index.html) (served with GitHub Pages from the /docs folder). All data is simulated.
