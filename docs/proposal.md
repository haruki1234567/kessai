# Kessai

_Instant stablecoin invoice settlement for Japanese SMEs, funded by a 10M yen liquidity pool_

## Summary

Kessai lets small businesses get paid immediately on B2B invoices by converting them into stablecoin-backed instant payments instead of waiting 30-60 days. A liquidity pool (seeded with the 10M yen budget) advances funds and earns a discount fee, while buyers repay on the original due date, creating a sustainable yield-generating lending business from day one.

## Target users

Japanese SMEs and freelancers waiting on B2B invoice payments, and crypto liquidity providers seeking yield

## Problem

Japanese SMEs often wait 30-60 days for invoice payment, causing cash flow problems, while banks are slow/expensive for short-term financing.

## Solution

Tokenize approved invoices on-chain and instantly advance stablecoins from a liquidity pool, collecting a small discount fee when the invoice is repaid.

## MVP features

- Upload & verify invoice, mint on-chain claim via Solana program
- Instant stablecoin payout to SME wallet from liquidity pool
- Automated repayment collection from buyer on due date
- LP dashboard showing pool yield and risk exposure
- Simple KYC/credit scoring flow for first pilot invoices

## Chains

Solana

## Tech

Anchor, Solana Pay, USDC, Next.js, Supabase, Chainlink/Pyth price feed, Metaplex (invoice NFT)

## Category

DeFi

## Why now

Stablecoin payment rails and RWA tokenization are maturing fast on Solana, and Japan's SMEs face chronic late-payment cash flow issues that fintechs haven't fully solved.

## Roadmap

- Run pilot with 5-10 real SMEs and the seed liquidity pool
- Add credit-scoring model and insurance/reserve fund for defaults
- Partner with Japanese accounting SaaS for invoice data integration
