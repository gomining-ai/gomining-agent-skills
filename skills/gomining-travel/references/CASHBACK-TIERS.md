# GoMining Travel Cashback Tiers

## Cashback Overview

GoMining Travel rewards hotel bookings with cashback in the form of TH/s mining power upgrades. The cashback rate depends on the user's VIP level within the GoMining ecosystem.

> **Important:** Cashback applies only to hotel bookings. Flight bookings do not earn cashback in Phase 1.

---

## VIP Cashback Rates

| VIP Level | Cashback Rate | Cashback on $650 Booking (TH/s) |
|-----------|---------------|----------------------------------|
| Bronze | 1.0% | 0.260 TH/s |
| Silver | 1.6% | 0.416 TH/s |
| Gold | 2.2% | 0.572 TH/s |
| Platinum | 2.8% | 0.728 TH/s |
| Diamond | 3.4% | 0.884 TH/s |
| Legend | 4.0% | 1.040 TH/s |

---

## Cashback Formula

```
Cashback (TH/s) = Booking Amount (USD) x VIP Cashback Rate (%) / Cost per 1 TH/s (current TH/s price)
```

### Calculation Examples

| VIP Level | Booking Amount | Cashback Rate | Cashback Value |
|-----------|----------------|---------------|----------------|
| Bronze | $650 | 1.0% | $6.50 worth of TH/s |
| Silver | $1,200 | 1.6% | $19.20 worth of TH/s |
| Gold | $650 | 2.2% | $14.30 worth of TH/s |
| Platinum | $2,000 | 2.8% | $56.00 worth of TH/s |
| Diamond | $650 | 3.4% | $22.10 worth of TH/s |
| Legend | $3,000 | 4.0% | $120.00 worth of TH/s |

> **Note:** The TH/s conversion price is displayed in the GoMining app and may be adjusted over time.

---

## Cashback Lifecycle

| Stage | Description |
|-------|-------------|
| **Accrual** | Cashback accrues immediately after booking confirmation |
| **Pending** | Remains pending during the hotel stay |
| **Finalization** | Cashback finalizes after guest check-out |
| **Application** | TH/s mining power applied to the selected miner |

```
Booking Confirmed → Cashback Accrues → Guest Check-out → Cashback Finalized → TH/s Applied to Miner
```

---

## Miner Selection Rules

When cashback is earned, the TH/s mining power is applied to a specific miner. Users can select which miner receives the upgrade, subject to the following rules.

### Selection Behavior

| Scenario | Behavior |
|----------|----------|
| User selects a miner | Cashback applied to the chosen miner |
| No miner selected | System auto-selects the strongest miner |
| No miner owned | Cashback is saved and auto-applied when first miner is purchased |

### Miner Capacity Limit

| Rule | Value |
|------|-------|
| Maximum miner capacity for cashback accumulation | **5000 TH** |

> **Note:** Miners at or above the 5000 TH capacity limit cannot receive additional cashback TH/s.

### Miner Restrictions

The following miner types **cannot** be selected as cashback targets:

| Restricted Miner Type | Reason |
|------------------------|--------|
| **Installment miners** | Miners purchased on installment plans |
| **Sale miners** | Miners acquired through promotional sales |
| **Low-efficiency miners** | Miners below 20 wt/th efficiency threshold |
| **Bonus miners** | Miners received as bonuses or rewards |

---

## Frequently Asked Questions

### What is the TH/s cashback?

Instead of receiving cash or token refunds, GoMining Travel converts your hotel booking cashback into mining power (TH/s) that is added to one of your miners, increasing its hash rate and earning potential.

### How is the cashback rate determined?

Your cashback rate is tied to your GoMining VIP level. Higher VIP tiers earn higher cashback percentages, ranging from 1% (Bronze) to 4% (Legend).

### Do flights earn cashback?

No. In the current Phase 1 rollout, cashback applies only to hotel bookings. Flight cashback may be introduced in future phases.

### What happens if I do not own a miner?

Your cashback TH/s is saved in your account. When you purchase your first eligible miner, the accumulated cashback is automatically applied.

### Can I choose which miner gets the cashback?

Yes, you can select any eligible miner. However, installment miners, sale miners, miners below 20 wt/th, and bonus miners cannot be selected. If you do not choose, the system auto-selects your strongest miner.

### What is the maximum TH/s a miner can accumulate from cashback?

A single miner can accumulate cashback up to a maximum of 5000 TH. Once this limit is reached, you must select a different miner.

### When is the cashback finalized?

Cashback accrues upon booking confirmation but is only finalized after the guest checks out of the hotel. If the booking is cancelled before check-in, no cashback is awarded.

### What TH/s price is used in the formula?

The current TH/s price is displayed in the GoMining app and may be adjusted over time based on market conditions.
