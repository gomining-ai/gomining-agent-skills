# GoMining Travel Cashback Tiers

## Cashback Overview

GoMining Travel rewards hotel bookings with cashback in the form of TH/s mining power upgrades. The cashback rate depends on the user's VIP level within the GoMining ecosystem.

> **Important:** Cashback applies to hotel bookings.

---

## VIP Cashback Rates

| VIP Level | Cashback Rate |
|-----------|---------------|
| Bronze | 1.0% |
| Silver | 1.6% |
| Gold | 2.2% |
| Platinum | 2.8% |
| Diamond | 3.4% |
| Legend | 4.0% |

---

## Cashback Formula

```
Cashback (TH/s) = Booking Amount (USD) × VIP Cashback Rate (%) / Current TH Price
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

> **Note:** The TH price used in the formula reflects the current market rate and changes over time. The actual TH/s credited will vary based on the TH price at the time of cashback finalization.

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
| **Installment miners** | Miners on installment plans (Mine Now, Pay Later) not yet fully paid off |
| **Sale miners** | Miners currently listed for sale |
| **Low-efficiency miners** | Miners below 20 wt/th efficiency threshold |

---

## Frequently Asked Questions

### What is the TH/s cashback?

Instead of receiving cash or token refunds, GoMining Travel converts your hotel booking cashback into mining power (TH/s) that is added to one of your miners, increasing its hash rate and earning potential.

### How is the cashback rate determined?

Your cashback rate is tied to your GoMining VIP level. Higher VIP tiers earn higher cashback percentages, ranging from 1% (Bronze) to 4% (Legend).

### Do all bookings earn cashback?

Yes. Cashback is awarded on hotel bookings based on your VIP tier.

### What happens if I do not own a miner?

Your cashback TH/s is saved in your account. When you purchase your first eligible miner, the accumulated cashback is automatically applied.

### Can I choose which miner gets the cashback?

Yes, you can select any eligible miner. However, unpaid installment miners, miners listed for sale, and miners below 20 wt/th cannot be selected. If you do not choose, the system auto-selects your strongest miner.

### What is the maximum TH/s a miner can accumulate from cashback?

A single miner can accumulate cashback up to a maximum of 5000 TH. Once this limit is reached, you must select a different miner.

### When is the cashback finalized?

Cashback accrues upon booking confirmation but is only finalized after the guest checks out of the hotel. If the booking is cancelled before check-in, no cashback is awarded.

### What is the TH price used in the formula?

The TH price used in the cashback formula reflects the current market rate for 1 TH/s on GoMining. It changes over time — check the GoMining app or calculator for the current value.
