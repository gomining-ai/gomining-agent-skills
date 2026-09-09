---
name: gomining-simple-earn
description: "GoMining Simple Earn — passive earning mechanism for interest on crypto asset balances. Covers one-button activation, rewards every 4 hours paid by default in BTC or optionally in TH (computing power added to a selected miner, with a 10% TH bonus and a $0.10/cycle minimum), supported assets (non-EEA: BTC, ETH, SOL, BNB, TON, USDT, USDC; EEA: same but no USDT), VIP yield multipliers (Bronze I: none through Elite: x1.46), individual APR per asset, yield sources (staking, DeFi protocols, internal liquidity), KYC Basic requirement, no lockup or penalties, full withdrawal anytime. Available globally except the USA."
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
    - "simple earn th"
    - "simple earn rewards in th"
    - "simple earn to miner"
    - "switch simple earn rewards"
---

# GoMining Simple Earn

## Overview

Simple Earn is GoMining's passive earning mechanism that lets users earn interest on their crypto asset balances. Deposits auto-compound at fixed intervals. **Rewards are paid in BTC by default; a user can opt in to receive rewards as TH (computing power) added to one of their miners instead — with a 10% TH bonus, subject to a $0.10 per-cycle minimum. See the *Reward type — BTC or TH* section for the full rules.** There are no lockup periods and no penalties — users can withdraw their full balance at any time.

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
| Reward type | **BTC** by default (paid to the virtual wallet). Optional: switch to **TH** (added to one of your miners, with a 10% TH bonus, subject to a $0.10/cycle minimum) — see *Reward type — BTC or TH* below. Do not describe rewards as "always BTC". |
| Principal protection | Capital preservation is **not absolutely guaranteed** — Simple Earn uses DeFi protocols; in rare cases (e.g. smart contract vulnerability) losses may occur. GoMining actively monitors and rebalances to reduce risk. |
| Interest guarantee | Interest is **NOT** guaranteed; yield can be zero |
| APR | Each asset has an individual APR set by the liquidity manager |
| Estimated yield | Weighted average across all deposited assets |
| Lockup | **None** — no lockup, no penalties |
| Compounding | Auto-compounds at fixed intervals |

---

## VIP Yield Multipliers

Your VIP level applies a multiplier to the base APR for each asset. Higher tiers earn more.

| Tier | Multiplier |
|------|------------|
| Bronze I | x1 (base APR) |
| Bronze II | x1.08 |
| Silver I | x1.1 |
| Silver II | x1.12 |
| Silver III | x1.14 |
| Gold I | x1.16 |
| Gold II | x1.18 |
| Platinum I | x1.2 |
| Platinum II | x1.22 |
| Platinum III | x1.24 |
| Diamond I | x1.26 |
| Diamond II | x1.28 |
| Diamond III | x1.3 |
| Diamond IV | x1.32 |
| Diamond V | x1.34 |
| Legend I | x1.36 |
| Legend II | x1.38 |
| Legend III | x1.4 |
| Legend IV | x1.42 |
| Legend V | x1.44 |
| Elite | x1.46 |

> **Note:** The "Maximum APR" shown in the app reflects the Elite VIP rate. Platinum+ subscription grants a x1.2 multiplier (equivalent to Platinum I) without changing your VIP tier.

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
| KYC | **KYC Basic** verification required |
| Jurisdiction | Must be in an available (non-restricted) country |
| Minimum balance | **10 USD** equivalent |
| Wallet transfer | Funds must be transferred from main wallet to Simple Earn balance |

### Restricted Jurisdictions

> **Warning:** Simple Earn is not available in several jurisdictions including the USA, Belarus, Cuba, Iran, Iraq, North Korea, Syria, Venezuela, Zimbabwe, and others.

| Region | Restriction | Reason |
|--------|-------------|--------|
| **USA** | Not available | GoMining does not offer Simple Earn in the USA |
| **EEA** | Limited assets | Available; USDT is not supported in the EEA (USDC is) |
| **UK** | Available | All supported assets are available in the UK — see the UK onboarding notes in [Eligibility](references/ELIGIBILITY.md#uk-onboarding-notes) |

For the full list of restrictions, see [Eligibility](references/ELIGIBILITY.md).

---

## Frequently Asked Questions

### What is Simple Earn?

Simple Earn is GoMining's passive earning product that pays BTC interest on your crypto asset balances. It auto-compounds at fixed intervals with no lockup periods or penalties.

### How do I activate Simple Earn?

Tap the one-button invest option in the GoMining app, sign the Simple Earn agreement, and your deposits will automatically begin earning. You need KYC Basic verification and a minimum balance of 10 USD equivalent.

### What currency are rewards paid in?

By **default**, rewards are paid in **BTC**, regardless of which asset you deposited. You can **switch the reward type to TH** (computing power added to one of your miners) on the Simple Earn screen — TH rewards carry a **+10% bonus** vs. a straight BTC-to-TH conversion, are added in a single **daily upgrade**, and only apply to 4-hour cycles whose reward is **$0.10 USD or more** (sub-threshold cycles stay paid in BTC without any user action). Full rules (miner eligibility ≤ 20 W/TH, no MNPL, not listed for sale, has room; auto-fallback to BTC if you sell the selected miner) are in the [FAQ — *Simple Earn rewards in TH*](references/FAQ-SIMPLE-EARN.md#simple-earn-rewards-in-th).

### Is my principal guaranteed?

Simple Earn is built to preserve capital, but preservation is **not absolutely guaranteed** — it relies on DeFi protocols, and in rare cases (e.g. a smart contract vulnerability) losses may occur. GoMining actively monitors and rebalances to reduce risk. Interest is also not guaranteed, and yield can be zero in any given period.

### When do I receive rewards?

Rewards are **calculated** for every full 4-hour cycle you've participated in — cycles run from 00:00 UTC and repeat every 4 hours. Each cycle's reward is based on the **minimum balance** held during that full 4-hour cycle. **When and how the reward lands depends on the reward type:**

- **BTC (default):** credited to your virtual wallet at the end of each 4-hour cycle.
- **TH:** the 4-hour calculation is the same, but the TH is **added to your selected miner in a single daily upgrade** covering everything earned since the previous one, priced at the live TH price at the moment of that upgrade. Sub-$0.10-USD cycles still pay out in BTC that day.

### What if I deposit mid-cycle?

A new deposit is counted from the start of the next 4-hour cycle. Within a cycle, rewards use the lowest balance held — so a withdrawal or purchase that lowers your balance during the cycle reduces that cycle's reward.

### Can I withdraw at any time?

Yes. There are no lockup periods and no penalties. You can withdraw your full balance at any time.

### What assets are supported?

Supported assets depend on your region and may change due to local regulations (e.g., USDT is not available to EEA users). See the Supported Assets table above for the current list. The GOMINING token is excluded and has separate earning mechanics.

### Why is Simple Earn not available in my country?

Simple Earn is **not available in the USA**. Sanctioned countries (Belarus, Cuba, Iran, Iraq, North Korea, Syria, Venezuela, Zimbabwe) are also blocked. Simple Earn **is available in the UK** and **available in the EEA** (with USDT unsupported for EEA users; USDC is). See the full list in the Eligibility reference.

### How is APR determined?

Each asset has an individual APR set by GoMining's liquidity manager. The estimated yield displayed is a weighted average across all your deposited assets.

---

## Official Resources

| Resource | URL |
|----------|-----|
| Main Website | https://gomining.com/ |

---

## References

- [Simple Earn Screen Layout](references/SIMPLE-EARN-SCREEN.md) — Where each figure and control lives on the Simple earn screen
- [Yield Mechanics](references/YIELD-MECHANICS.md) — How yield works, the 4-hour reward cycle, and yield sources
- [Eligibility](references/ELIGIBILITY.md) — KYC requirements, jurisdictions, restrictions, and legal considerations
- [FAQ: Simple Earn](references/FAQ-SIMPLE-EARN.md) — How Simple Earn works, APR, eligibility, and reward mechanics
