# GoMining Travel Booking Flow

## Overview

GoMining Travel is accessible directly within the GoMining app. Currently hotel bookings are available. Users search for hotels, pay with GM tokens, and receive cashback as TH/s mining power. Flight bookings are planned for a future phase.

---

## Booking Lifecycle

### Status Transitions

| Status | Description |
|--------|-------------|
| **Pending** | Booking submitted, awaiting confirmation from the provider |
| **Success** | Booking confirmed by the provider, cashback accrues (hotels) |
| **Cancelled** | Booking cancelled by user or provider, refund processed if eligible |

```
                    ┌──────────┐
                    │ PENDING  │
                    └────┬─────┘
                         │
                ┌────────┴────────┐
                ▼                 ▼
         ┌──────────┐     ┌──────────────┐
         │ SUCCESS  │     │  CANCELLED   │
         └────┬─────┘     └──────────────┘
              │                   │
              ▼                   ▼
       ┌─────────────┐    ┌─────────────┐
       │  Check-out  │    │   Refund    │
       │  Cashback   │    │  (if before │
       │  finalized  │    │  deadline)  │
       └─────────────┘    └─────────────┘
```

---

## Payment Process

### Step-by-Step Flow

| Step | Action | Details |
|------|--------|---------|
| 1 | **Search** | User searches hotels in the GoMining app Travel section |
| 2 | **Select** | User chooses a hotel from results |
| 3 | **Review** | Booking details displayed including price in GM tokens |
| 4 | **Pay** | User confirms payment in GM tokens (or BTC/USDT) |
| 5 | **Confirm** | Booking moves to Pending, then Success upon provider confirmation |
| 6 | **Cashback** | For hotels: cashback accrues and finalizes after check-out |

### Supported Payment Methods

| Payment Method | Role | Processing |
|----------------|------|------------|
| **GM tokens** | Primary | Direct payment |
| **BTC** | Alternative | Converted to GM at transaction time |
| **USDT** | Alternative | Converted to GM at transaction time |

> **Note:** Regardless of the payment asset chosen, the booking is ultimately processed in GM tokens. BTC and USDT are converted at the current exchange rate.

---

## Cancellation and Refunds

### Cancellation Policy

| Rule | Details |
|------|---------|
| Cancellation allowed | Up to the cancellation deadline specified at booking time |
| Cancellation deadline | Displayed during booking, varies by hotel provider |
| After deadline | Cancellation may not be available or may incur penalties |

### Refund Process

| Scenario | Refund | Cashback |
|----------|--------|----------|
| Cancelled before deadline | Full refund issued | No cashback awarded |
| Cancelled after deadline | Subject to provider policy | No cashback awarded |
| Successful stay (check-out) | No refund | Cashback finalized and applied |
| Provider cancellation | Full refund issued | No cashback awarded |

> **Important:** Cashback is only finalized after a successful hotel check-out. If a booking is cancelled at any stage, no cashback is awarded.

---

## Hotel Bookings

| Aspect | Details |
|--------|---------|
| Availability | Phase 1 (launched Feb 20, 2026) |
| Payment | GM tokens (primary), BTC, USDT |
| Cashback | Yes, based on VIP tier (1%--4%) |
| Cancellation | Allowed up to provider-specified deadline |
| Cashback timing | Accrues at confirmation, finalizes after check-out |

---

## Flight Bookings

| Aspect | Details |
|--------|---------|
| Availability | Phase 2 (planned) |
| Payment | GM tokens (primary), BTC, USDT |
| Cashback | Not available initially |
| Cancellation | Subject to airline policy |

---

## Phased Rollout

### Phase 1 — Hotels (Launched February 20, 2026)

| Feature | Status |
|---------|--------|
| Hotel search and booking | Available |
| GM token payments | Available |
| VIP-tiered cashback (TH/s) | Available |
| Miner selection for cashback | Available |
| Seamless login via GoMining account | Available |

### Phase 2 — Flights (Planned)

| Feature | Status |
|---------|--------|
| Flight search and booking | Planned |
| GM token payments | Planned |
| Flight cashback | To be determined |

### Phase 3 — Multi-Asset Payments (Planned)

| Feature | Status |
|---------|--------|
| Expanded payment asset support | Planned |
| Additional cryptocurrencies | To be determined |
| Fiat payment options | To be determined |

---

## Frequently Asked Questions

### How do I access GoMining Travel?

GoMining Travel is accessible directly within the GoMining app. Navigate to the Travel section to search and book hotels.

### Do I need a separate account?

No. GoMining Travel uses your existing GoMining account — no separate login or registration required.

### What happens after I book a hotel?

Your booking enters Pending status. Once the hotel provider confirms, it moves to Success. Cashback accrues at confirmation and finalizes after you check out.

### Can I cancel a booking?

Yes, you can cancel up to the cancellation deadline shown during the booking process. Refunds are issued for eligible cancellations. Cancellation policies vary by provider.

### What if the provider cancels my booking?

You receive a full refund. No cashback is awarded for provider-cancelled bookings.

### When will flight bookings be available?

Flight bookings are not yet available. They are planned for a future phase — no launch date has been announced.

### What currencies can I pay with?

The primary payment method is GM tokens. You can also pay with BTC or USDT, which are automatically converted to GM at the current exchange rate.

