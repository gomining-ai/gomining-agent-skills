---
name: gomining-simple-earn
description: "GoMining Simple Earn — passive earning mechanism for interest on crypto asset balances. Covers one-button activation, BTC rewards every 4 hours, supported assets (non-EEA: BTC, ETH, SOL, BNB, TON, USDT, USDC; EEA: same but no USDT), VIP yield multipliers (Bronze I: none through Elite: x1.46), individual APR per asset, yield sources (staking, DeFi protocols, internal liquidity), KYC Level-1 requirement, no lockup or penalties, full withdrawal anytime. Available globally except the USA."
license: Apache-2.0
compatibility: "Compatible with Claude Code, Codex, and all Agent Skills spec tools."
metadata:
  author: gomining
  version: "1.0"
  tags:
    - simple-earn
    - yield
    - interest
    - passive-income
    - btc-rewards
    - staking
  triggers:
    - "simple earn"
    - "gomining earn"
    - "earn interest"
    - "passive income"
    - "btc yield"
    - "auto compound"
    - "earn on crypto"
    - "simple earn eligibility"
    - "simple earn yield"
---

# GoMining Simple Earn

## Overview

Simple Earn is GoMining's passive earning mechanism that lets users earn interest on their crypto asset balances. Deposits auto-compound at fixed intervals, and dividends are paid in BTC regardless of the deposited asset type. There are no lockup periods and no penalties — users can withdraw their full balance at any time.

---

## How It Works

### Activation

| Step | Description |
|------|-------------|
| 1. Invest | One-button invest from the GoMining app |
| 2. Agreement | Sign the Simple Earn agreement |
| 3. Auto-enter | All deposits automatically enter the earning cycle |
| 4. Withdraw | Full withdrawal available at any time |

### Key Principles

| Principle | Details |
|-----------|---------|
| Dividend currency | **BTC** — always paid in BTC regardless of deposited asset |
| Principal protection | Deposits never lose principal |
| Interest guarantee | Interest is **NOT** guaranteed; yield can be zero |
| APR | Each asset has an individual APR set by the liquidity manager |
| Estimated yield | Weighted average across all deposited assets |
| Lockup | **None** — no lockup, no penalties |
| Compounding | Auto-compounds at fixed intervals |

---

## Supported Assets

Assets available depend on the user's region:

| Asset | Non-EEA Users | EEA Users |
|-------|--------------|-----------|
| **BTC** | Available | Available |
| **ETH** | Available | Available |
| **SOL** | Available | Available |
| **BNB** | Available | Available |
| **TON** | Available | Available |
| **USDT** | Available | Not available |
| **USDC** | Available | Available |
| **GOMINING** | Excluded | Excluded |

> **Note:** GOMINING token is excluded from Simple Earn and has its own separate earning mechanics. Specific availability may change due to local regulations.

---

## Reward Cycle (Every 4 Hours)

Simple Earn operates on a 4-hour reward cycle:

```
┌─────────────────────────────────────────────────────────────┐
│                  Simple Earn 4-Hour Cycle                     │
├─────────────────────────────────────────────────────────────┤
│                                                              │
│  Starting 00:00 UTC — cycles repeat every 4 hours:          │
│  00:00 → 04:00 → 08:00 → 12:00 → 16:00 → 20:00 → 00:00    │
│                                                              │
│  Each cycle:                                                 │
│  ┌──────────────────────────────────────────┐               │
│  │ REWARDS CALCULATED & CREDITED             │               │
│  │ Based on minimum balance held during      │               │
│  │ the full 4-hour cycle                     │               │
│  │ BTC credited directly to wallet           │               │
│  └──────────────────────────────────────────┘               │
│                                                              │
│  IMPORTANT:                                                  │
│  Rewards use the LOWEST balance recorded during the cycle.   │
│  A withdrawal reduces the minimum and affects that cycle.    │
│  New deposits are counted from the START of the next cycle.  │
│                                                              │
└─────────────────────────────────────────────────────────────┘
```

| Parameter | Details |
|-----------|---------|
| Cycle frequency | **Every 4 hours** (6 times per day) |
| Cycle start | 00:00 UTC, then every 4 hours |
| Reward basis | Minimum balance held during the full cycle |
| Reward currency | **BTC** |
| New deposit effective | Start of next cycle |

---

## Yield Sources

Yield is generated from three primary sources:

| Source | Description |
|--------|-------------|
| **Staking** | Blockchain validation rewards |
| **DeFi Protocols** | Liquidity pools and lending platforms |
| **Internal Liquidity Management** | GoMining's own liquidity operations |

For detailed yield mechanics, see [Yield Mechanics](references/YIELD-MECHANICS.md).

---

## Eligibility

| Requirement | Details |
|-------------|---------|
| KYC | **Level-1** verification required |
| Jurisdiction | Must be in an available (non-restricted) country |
| Minimum balance | **10 USD** equivalent |
| Wallet transfer | Funds must be transferred from main wallet to Simple Earn balance |

### Restricted Jurisdictions

> **Warning:** Simple Earn is not available in several jurisdictions including the USA, Belarus, Cuba, Iran, Iraq, North Korea, Syria, Venezuela, Zimbabwe, and others.

| Region | Restriction | Reason |
|--------|-------------|--------|
| **USA** | Blocked | SEC requires Broker-Dealer license |
| **EEA** | Limited | MiCA CASP requirements |
| **UK** | Restricted | FCA license needed |

For the full list of restrictions, see [Eligibility](references/ELIGIBILITY.md).

---

## Frequently Asked Questions

### What is Simple Earn?

Simple Earn is GoMining's passive earning product that pays BTC interest on your crypto asset balances. It auto-compounds at fixed intervals with no lockup periods or penalties.

### How do I activate Simple Earn?

Tap the one-button invest option in the GoMining app, sign the Simple Earn agreement, and your deposits will automatically begin earning. You need KYC Level-1 verification and a minimum balance of 10 USD equivalent.

### What currency are rewards paid in?

All rewards are paid in **BTC**, regardless of which asset you deposited (BTC, USDT, or USDC).

### Is my principal guaranteed?

Yes, deposits never lose principal. However, interest is not guaranteed and yield can be zero in any given period.

### When do I receive rewards?

Rewards are credited daily at 07:00 UTC, based on the balance snapshot taken at 23:59 UTC the previous day.

### What if I deposit after the daily snapshot?

Deposits made after 23:59 UTC will not participate in that day's reward cycle. They will be included starting from the next snapshot.

### Can I withdraw at any time?

Yes. There are no lockup periods and no penalties. You can withdraw your full balance at any time.

### What assets are supported?

Currently BTC, USDT, and USDC. Future additions include ETH, BNB, SOL, and TON. GOMINING token is excluded and has separate mechanics.

### Why is Simple Earn not available in my country?

Simple Earn is restricted in jurisdictions including the USA (SEC Broker-Dealer license required), EEA (MiCA CASP regulations), UK (FCA license needed), and several other countries. See the full list in the Eligibility reference.

### How is APR determined?

Each asset has an individual APR set by GoMining's liquidity manager. The estimated yield displayed is a weighted average across all your deposited assets.

---

## Official Resources

| Resource | URL |
|----------|-----|
| Main Website | https://gomining.com/ |

---

## References

- [Yield Mechanics](references/YIELD-MECHANICS.md) — How yield works, snapshot system, and yield sources
- [Eligibility](references/ELIGIBILITY.md) — KYC requirements, jurisdictions, restrictions, and legal considerations
- [FAQ: Simple Earn](references/FAQ-SIMPLE-EARN.md) — How Simple Earn works, APR, eligibility, and reward mechanics
