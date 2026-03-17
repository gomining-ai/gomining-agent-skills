# Cashback Rates Reference

## Overview

This document contains all cashback rate tables, calculation formulas, and miner selection rules for the GoMining Cashback service covering both Cards and Travel products.

---

## Card Cashback Rates

Card cashback is calculated as a percentage of each successful transaction amount, converted to TH/s mining power.

| VIP Level | Cashback Rate | Example ($100 spend) |
|-----------|---------------|----------------------|
| **Bronze** | 0.5% | $0.50 in TH/s |
| **Silver** | 1% | $1.00 in TH/s |
| **Gold** | 1.5% | $1.50 in TH/s |
| **Platinum** | 2% | $2.00 in TH/s |
| **Diamond** | 3% | $3.00 in TH/s |
| **Legend** | 5% | $5.00 in TH/s |

### Card Cashback Rules

| Rule | Value |
|------|-------|
| Accrual | Daily |
| Eligible | Successful transactions only |
| Ineligible | Failed, reversed, or refunded transactions |
| Redemption | Miner TH/s upgrades only (not tokens, not fiat) |

---

## Travel Cashback Rates

Travel cashback is calculated as a percentage of the hotel booking amount in USD, converted to TH/s using the cost-per-TH formula.

| VIP Level | Cashback Rate | Example ($1,000 booking) |
|-----------|---------------|--------------------------|
| **Bronze** | 1.0% | $10 worth of TH/s |
| **Silver** | 1.6% | $16 worth of TH/s |
| **Gold** | 2.2% | $22 worth of TH/s |
| **Platinum** | 2.8% | $28 worth of TH/s |
| **Diamond** | 3.4% | $34 worth of TH/s |
| **Legend** | 4.0% | $40 worth of TH/s |

### Travel Cashback Formula

```
TH/s Cashback = Booking Amount (USD) x VIP Cashback Rate (%) / Current TH/s price
```

> **Note:** The current TH/s price is displayed in the GoMining app and is subject to change based on market conditions.

### Travel Cashback Rules

| Rule | Value |
|------|-------|
| Eligible bookings | Hotels only |
| Ineligible | Flights (not supported initially) |
| Accrual | Upon booking confirmation (pending status) |
| Finalization | After guest check-out |
| Cancellation | Pending cashback reversed |

### Travel Cashback Lifecycle

| Stage | Status | Description |
|-------|--------|-------------|
| Booking confirmed | **Pending** | Cashback calculated and reserved |
| Guest checks out | **Finalized** | Cashback applied to miner |
| Booking cancelled | **Reversed** | Pending cashback removed |

---

## Rate Comparison: Card vs Travel

| VIP Level | Card Rate | Travel Rate | Difference |
|-----------|-----------|-------------|------------|
| Bronze | 0.5% | 1.0% | Travel +0.5% |
| Silver | 1.0% | 1.6% | Travel +0.6% |
| Gold | 1.5% | 2.2% | Travel +0.7% |
| Platinum | 2.0% | 2.8% | Travel +0.8% |
| Diamond | 3.0% | 3.4% | Travel +0.4% |
| Legend | 5.0% | 4.0% | Card +1.0% |

> **Note:** Travel rates are higher than Card rates for most VIP levels. However, at Legend level, Card cashback (5%) exceeds Travel cashback (4%).

---

## Miner Selection Rules

### Auto-Selection Priority

The system automatically selects a miner to receive cashback using the following priority:

| Priority | Criterion | Description |
|----------|-----------|-------------|
| 1 | Previously used miner | If the user has a previously assigned cashback miner and it is still eligible |
| 2 | Strongest miner | The user's miner with the highest mining power that meets eligibility |

### Eligibility Criteria

A miner must meet **all** of the following criteria to be eligible for cashback:

| Criterion | Requirement |
|-----------|-------------|
| Ownership | Not purchased via installment plan |
| Sale status | Not currently listed for sale |
| Efficiency | At least 20 wt/th |
| Type | Not a bonus miner |

### Ineligible Miner Types

| Miner Type | Reason |
|------------|--------|
| **Installment miners** | Ownership not fully transferred |
| **Miners on sale** | Ownership may change |
| **Low efficiency (<20 wt/th)** | Below minimum efficiency threshold |
| **Bonus miners** | Promotional miners excluded from cashback upgrades |

### Accumulation Limits

| Limit | Value | Impact |
|-------|-------|--------|
| **Max TH per miner** | 5,000 TH | Once reached, user must select a different eligible miner |

### Miner Selection Behavior

| Scenario | Behavior |
|----------|----------|
| First-time cashback user | Strongest eligible miner auto-selected |
| Returning user | Previously used miner re-selected (if eligible) |
| Selected miner becomes ineligible | User prompted to select new miner |
| Selected miner reaches 5,000 TH cap | User must manually select new miner |
| No eligible miners | Cashback cannot be applied until eligible miner is available |

---

## Shared Miner Rule

A single miner is selected to receive cashback from **all** sources:

| Source | Miner Used |
|--------|------------|
| Card cashback | Selected miner |
| Travel cashback | Selected miner |

The user cannot assign Card cashback to one miner and Travel cashback to another. Both always go to the same selected miner.

---

## Calculation Examples

### Example 1: Card Cashback (Gold VIP)

| Step | Value |
|------|-------|
| Transaction amount | $200 |
| VIP level | Gold |
| Cashback rate | 1.5% |
| Cashback value | $200 x 1.5% = $3.00 |
| TH/s awarded | $3.00 ÷ current TH/s price |

### Example 2: Travel Cashback (Platinum VIP)

| Step | Value |
|------|-------|
| Booking amount | $2,000 |
| VIP level | Platinum |
| Cashback rate | 2.8% |
| Cashback value | $2,000 x 2.8% = $56.00 |
| TH/s awarded | $56.00 ÷ current TH/s price |

### Example 3: Legend VIP Monthly Summary

| Source | Monthly Spend | Rate | Cashback Value |
|--------|---------------|------|----------------|
| Card transactions | $5,000 | 5% | $250 |
| Hotel bookings | $3,000 | 4% | $120 |
| **Total** | **$8,000** | — | **$370** |

> TH/s received depends on the current TH/s price in the GoMining app.

---

## Frequently Asked Questions

### Can the TH/s conversion rate change?

Yes. The current TH/s price is subject to change based on market conditions and GoMining pricing updates. Always check the GoMining app for the current rate.

### Do both Card and Travel cashback share the same miner?

Yes. A single miner is selected for all cashback sources. You cannot split cashback across multiple miners.

### What if I have no eligible miners?

Cashback cannot be applied until you have at least one eligible miner (not installment, not on sale, at least 20 wt/th, not a bonus miner). Earned cashback may be held pending until an eligible miner is available.

### Is there a minimum transaction for Card cashback?

Card cashback applies to all successful transactions regardless of amount. There is no minimum transaction threshold.

### How does VIP level affect my total earnings?

Higher VIP levels significantly increase cashback returns. A Legend user earns 10x the Card cashback rate (5%) compared to Bronze (0.5%), and 4x the Travel rate (4% vs 1%).
