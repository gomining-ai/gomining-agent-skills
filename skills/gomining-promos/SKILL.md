---
name: gomining-promos
description: "GoMining promotional system — promo codes, GoBoxes, and bonus mechanics. Covers general, individual, and referral promo code types, discount and cashback bonuses (tokens or TH mining power), promo code parameters (percent, caps, validity, usage limits, VIP and payment restrictions), promo sources (email campaigns, GoBoxes, Referral codes), GoBox digital loot boxes with weighted prize pools per VIP level, bonus miner task-based completion model, and trait selection system."
license: Apache-2.0
compatibility: "Compatible with Claude Code, Codex, and all Agent Skills spec tools."
metadata:
  author: gomining
  version: "1.0"
  tags:
    - promos
    - promo-codes
    - goboxes
    - bonuses
    - cashback
    - referral
    - vip
  triggers:
    - "gomining promos"
    - "promo code"
    - "gobox"
    - "bonus miner"
    - "referral code"
    - "referral activity"
    - "my friends"
    - "discount code"
    - "promotional"
---

# GoMining Promos

## Overview

The GoMining promotional system provides promo codes, GoBoxes, and bonus mechanics to incentivize user engagement, purchases, and referrals. Promos are distributed through GoBoxes, referral codes, email campaigns, and in-app notifications.

---

## Promo Code Types

| Type | Description | Scope |
|------|-------------|-------|
| **General** | One code shared across a user segment | Many users, same code |
| **Individual** | Unique code generated per user | One code per user |
| **Referral** | Binds a new user to the referrer on first purchase | Referrer-specific |

### General Codes

- A single code is created and distributed to a target segment (e.g., all Gold VIP users).
- Any eligible user can redeem the code within the defined limits.

### Individual Codes

- A unique code is generated and assigned to each user individually.
- Typically distributed via email campaigns or in-app notifications.

### Referral Codes

- Each user has a unique referral code.
- Entering the code as a promo code during the first purchase is **one** of four ways to bind a new user to the referrer — the primary way is entering the code on the new user's **profile page (Account details)**. See [FAQ: Referral and Ambassador Program](references/FAQ-REFERRAL.md) for all four and the eligibility conditions.
- The binding must exist **before** the new user makes any purchase.
- Both referrer and referee may receive bonuses depending on campaign configuration.

---

## Bonus Types

| Bonus Type | Description | Unit |
|------------|-------------|------|
| **Discount** | Fixed dollar amount subtracted from purchase price | USD ($) |
| **Cashback in Tokens** | Percentage of purchase returned as GOMINING tokens | GOMINING |
| **Cashback in Mining Power** | Percentage of purchase returned as mining power | TH/s |

---

## Promo Code Parameters

| Parameter | Description | Range / Notes |
|-----------|-------------|---------------|
| **Bonus Percent** | Percentage bonus applied to the purchase | Varies by campaign |
| **Max Bonus Cap** | Maximum bonus amount regardless of percent | Optional; caps the total bonus value |
| **Validity Period** | When the code is active | Date range (start-end) or N days from issuance |
| **Min Purchase Amount** | Minimum spend required to activate the code | Optional; USD threshold |
| **Global Usage Limit** | Total number of times the code can be redeemed | Across all users |
| **Per-User Usage Limit** | Maximum redemptions per individual user | Per user |
| **VIP Level Restriction** | Restricts code to specific VIP levels | Optional; e.g., Gold+ only |
| **Payment Method Restriction** | Limits code to specific payment methods | Fiat only, Crypto only, or both |

## Promo Sources

| Source | Description |
|--------|-------------|
| **GoBoxes** | Promo codes as prizes inside GoBox loot boxes |
| **Email / In-app** | Distributed via campaigns and notifications |
| **Referral Codes** | User-generated referral codes |

---

## GoBoxes

GoBoxes are digital loot boxes earned mainly by reaching new VIP levels. Each GoBox contains a prize determined transparently via numbered cells using Bitcoin blockchain data, the box's unique number, and the winning number from the previous box. A GoBox must be opened within 7 days of receiving it, or it becomes inactive and cannot be opened.

### Prize Types

| Prize | Description |
|-------|-------------|
| **Promo Codes** | Discount or cashback codes |
| **Avatar Keys** | Unlock cosmetic avatar items |
| **GOMINING Tokens** | Direct token rewards |
| **Gameplay Boosts** | Temporary gameplay enhancements |

### VIP Collections

Each VIP level has its own GoBox collection with different prize pools:

| VIP Level | Collection | Prize Quality |
|-----------|------------|---------------|
| **Bronze** | Bronze Collection | Standard prizes |
| **Silver** | Silver Collection | Improved prizes |
| **Gold** | Gold Collection | Premium prizes |
| **Platinum** | Platinum Collection | Elite prizes |

### GoBox Rules

| Rule | Value |
|------|-------|
| How they are earned | Mainly by reaching new VIP levels |
| Open window | Must be opened within 7 days, or it becomes inactive |
| Prize determination | Numbered cells using Bitcoin blockchain data, the box's unique number, and the previous box's winning number |

> **Note:** See [GoBox Mechanics](references/GOBOXES.md) for the full collection breakdowns and prize-determination details.

---

## Bonus Miner

The Bonus Miner is a task-based reward system where users complete tasks to earn a bonus miner.

### How It Works

```
┌─────────────────────────────────────────────────────────────┐
│                   Bonus Miner Flow                          │
├─────────────────────────────────────────────────────────────┤
│                                                             │
│  1. TASK ASSIGNMENT                                         │
│     ┌──────────────────────────────────────────┐           │
│     │ User receives a set of tasks to complete │           │
│     │ Tasks vary by campaign and VIP level     │           │
│     └──────────────────────────────────────────┘           │
│                         │                                   │
│                         ▼                                   │
│  2. TASK COMPLETION                                         │
│     ┌──────────────────────────────────────────┐           │
│     │ Complete all required tasks              │           │
│     │ Progress tracked automatically           │           │
│     └──────────────────────────────────────────┘           │
│                         │                                   │
│                         ▼                                   │
│  3. TRAIT SELECTION                                         │
│     ┌──────────────────────────────────────────┐           │
│     │ Choose miner traits upon completion      │           │
│     │ Traits affect miner appearance/stats     │           │
│     └──────────────────────────────────────────┘           │
│                         │                                   │
│                         ▼                                   │
│  4. MINER AWARDED                                           │
│     ┌──────────────────────────────────────────┐           │
│     │ Bonus miner added to user's collection   │           │
│     │ Miner begins generating rewards          │           │
│     └──────────────────────────────────────────┘           │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

### Trait Selection System

- Upon completing all tasks, users select traits for their bonus miner.
- Traits determine visual appearance and may affect miner characteristics.
- Trait options depend on the specific bonus miner campaign.

---

## Promo Code Redemption Flow

```
┌─────────────────────────────────────────────────────────────┐
│                Promo Code Redemption Flow                    │
├─────────────────────────────────────────────────────────────┤
│                                                             │
│  1. USER ENTERS CODE                                        │
│     ┌──────────────────────────────────────────┐           │
│     │ Code entered at checkout or promo page   │           │
│     └──────────────────────────────────────────┘           │
│                         │                                   │
│                         ▼                                   │
│  2. VALIDATION                                              │
│     ┌──────────────────────────────────────────┐           │
│     │ Check: code exists and is active         │           │
│     │ Check: within validity period            │           │
│     │ Check: global usage limit not reached    │           │
│     │ Check: per-user limit not reached        │           │
│     │ Check: VIP level eligible (if set)       │           │
│     │ Check: payment method matches (if set)   │           │
│     │ Check: min purchase amount met (if set)  │           │
│     └──────────────────────────────────────────┘           │
│                         │                                   │
│                         ▼                                   │
│  3. BONUS APPLIED                                           │
│     ┌──────────────────────────────────────────┐           │
│     │ Calculate bonus (percent x purchase)     │           │
│     │ Apply max bonus cap (if set)             │           │
│     │ Apply discount / queue cashback          │           │
│     └──────────────────────────────────────────┘           │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

---

## Frequently Asked Questions

### What types of promo codes does GoMining offer?

GoMining offers three types: General codes (shared across a user segment), Individual codes (unique per user), and Referral codes (binds a new user to a referrer on first purchase).

### What bonuses can a promo code provide?

Promo codes can provide a fixed dollar discount, cashback in GOMINING tokens, or cashback in mining power (TH/s).

### How long are promo codes valid?

Validity depends on configuration: either a fixed date range (start and end dates) or a number of days from the date of issuance.

### Can promo codes be restricted to certain users?

Yes. Codes can be restricted by VIP level (e.g., Gold and above only) and by payment method (fiat only, crypto only, or both). They can also have minimum purchase requirements.

### What is a GoBox?

A GoBox is a digital loot box earned mainly by reaching new VIP levels. The prize is determined transparently via numbered cells using Bitcoin blockchain data, the box's unique number, and the winning number from the previous box. Prizes include promo codes, avatar keys, GOMINING tokens, and gameplay boosts.

### Do GoBoxes expire?

Yes. A GoBox must be opened within 7 days of receiving it. If it is not opened within that window, it becomes inactive and can no longer be opened.

### Are GoBox prizes the same for all VIP levels?

No. Each VIP level (Bronze, Silver, Gold, Platinum) has its own collection with different prize pools. Higher VIP levels have access to better prizes.

### What is the Bonus Miner?

The Bonus Miner is a task-based reward system. Users complete a set of assigned tasks and, upon completion, select traits for a bonus miner that is added to their collection.

### How do referral codes work?

Each user has a unique referral code. The new user can be bound to the referrer in four ways — entering the code on their **profile page (Account details)**, which is the most reliable, opening a referral **link**, entering the code as a **promo code** during the first purchase, or activating a qualifying **gift link**. The binding must happen **before** they make any purchase, and only if they registered within the last 30 days, own no miner yet, have no advertising attribution, and aren't already linked to another referrer. Both parties may receive bonuses depending on the active campaign configuration. Full rules: [FAQ: Referral and Ambassador Program](references/FAQ-REFERRAL.md).

---

## Official Resources

| Resource | URL |
|----------|-----|
| Main Website | https://gomining.com/ |

---

## References

- [GoBox Mechanics](references/GOBOXES.md) — GoBox prize pools, VIP collections, and probability mechanics
- [FAQ: Promos Overview](references/FAQ-OVERVIEW.md) — Overview of all GoMining promotional programs
- [FAQ: Bonus Miner](references/FAQ-BONUS-MINER.md) — How the free Bonus Miner works and how to use it
- [FAQ: Bounty Program](references/FAQ-BOUNTY.md) — Earning GOMINING tokens through weekly Bounty tasks
- [FAQ: Raffles and Contests](references/FAQ-RAFFLES.md) — How raffles and contests work, tickets, and prize claiming
- [FAQ: Referral and Ambassador Program](references/FAQ-REFERRAL.md) — Referral rewards, ambassador benefits, and program rules
