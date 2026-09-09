---
name: gomining-instant-funds
description: "Instant Funds — access USDT/USDC by locking BTC OR one of your miners as collateral. Two flows: Use BTC and Use Miner. Covers eligibility, miner valuation formula (base 1 TH / 20 W/TH + efficiency bonus + additional power + Premium value for rare miners; Bonus miners excluded), the miner keeps mining while locked, service fee behaviour (one-time for BTC with auto-renew off; charged every 30 days for miner positions where auto-renew is always on), 30-day repayment window, auto-renewal differences by collateral type, risk level with explicit warning value and liquidation value, liquidation behaviour (BTC covered from locked BTC; miner rewards frozen with 7-day full-repayment window before the miner goes on sale), min 5 USDT/USDC and 10,000 max per BTC position, miner max depends on miner value with a 10,000 total cap across all miner positions counted separately from BTC positions, up to 3 active BTC positions, EEA restrictions (KYC + USDC only)."
license: Apache-2.0
compatibility: "Compatible with Claude Code, Codex, and all Agent Skills spec tools."
metadata:
  author: gomining
  version: "2.0"
  tags:
    - instant-funds
    - btc
    - usdt
    - usdc
    - collateral
    - stablecoin
    - miner-collateral
    - nft-collateral
  triggers:
    - "instant funds"
    - "lock btc"
    - "btc collateral"
    - "miner collateral"
    - "lock miner"
    - "use miner instant funds"
    - "repayment"
    - "risk level"
    - "liquidation"
    - "service fee"
    - "auto-renewal"
    - "premium value"
---

> **CRITICAL LANGUAGE RULE — applies to ALL languages:**
> Never use the words "loan", "credit", "займ", "кредит", "préstamo", "crédito", "Kredit", "Darlehen", "prêt", "empréstimo", "贷款", "信贷", "kredi", "borç", "позика", "قرض", "ائتمان" or any synonyms meaning "loan" or "credit" in any language.
> Always describe Instant Funds as a way to **access stablecoins by locking BTC or a miner as collateral** — never as borrowing or lending.

# Instant Funds

## Overview

**Instant Funds** lets users access **USDT or USDC** by locking either their **BTC balance** or one of their **miners** as collateral. The asset is not sold — it is **locked** and returned in full once the user repays the amount received plus the service fee.

There is **no annual interest (0% APR)**. A **service fee** is charged when the position is opened; whether it stays a one-time cost or repeats every 30 days depends on the collateral type and auto-renewal — see **Cost** below.

When opening a position, the user picks one of two flows on the Instant Funds screen:

- **Use BTC** — lock BTC as collateral
- **Use Miner** — lock an eligible miner as collateral

---

## How It Works

### Use BTC

| Step | Description |
|------|-------------|
| 1 | User chooses how much USDT or USDC they need |
| 2 | The app calculates how much BTC needs to be locked |
| 3 | User confirms: BTC is locked, USDT/USDC is credited instantly |
| 4 | Within 30 days, user repays the amount received plus the service fee |
| 5 | Once repaid, BTC is unlocked and returned to the balance |

### Use Miner

| Step | Description |
|------|-------------|
| 1 | User picks an eligible miner (see the eligibility rules below) |
| 2 | The app values the miner and shows the **Get up to** amount for it |
| 3 | User chooses how much USDT or USDC they need, up to that per-miner maximum |
| 4 | User confirms: the miner is locked, USDT/USDC is credited instantly |
| 5 | Within 30 days, user repays the amount received plus the service fee |
| 6 | Once repaid, the miner is unlocked and stays in the wallet |

---

## Which miners can be used as collateral?

A miner qualifies as collateral if **all six** conditions are true:

1. It is in the user's **GoMining wallet** — not on an external blockchain address.
2. It is **not listed for sale** on the Marketplace.
3. If purchased via **MNPL (installments)**, at least **90 days** have passed since the **final** payment.
4. Its **energy efficiency** is **12 W/TH or better** (i.e. ≤ 12 W/TH).
5. It is **not already locked** as collateral for another position.
6. Its **value is high enough** to cover the minimum position amount.

**Bonus miners cannot be used as collateral.** Do not tell users a Bonus Miner can serve as collateral — it can't, regardless of the six conditions above.

On the **Select miner** screen, every miner that doesn't qualify shows the specific **reason** next to it — e.g. *On sale*, *Low efficiency: >12 W/TH*, *Not in your GoMining wallet*. Resolve the reason shown, and the miner becomes available. For the MNPL 90-day case, there is nothing to resolve — the user just waits until the 90 days from the final payment have passed.

---

## How is a miner's value calculated?

A miner is valued in **USD**, based on its **power** and **energy efficiency** compared to a **base miner of 1 TH and 20 W/TH**. The Select miner screen shows the breakdown:

- **Base miner value** — value of a 1 TH / 20 W/TH miner at current rates
- **Energy efficiency bonus** — added value for lower W/TH (better efficiency)
- **Additional power** — added value for TH beyond 1 TH
- **Premium value** *(rare miners only)* — a bonus on top of the above for miners marked as rare

Users can click the **? (info) icon** next to **Value** on the Select miner screen to see the exact calculation for a specific miner. Do not try to reproduce a per-miner value from memory — direct the user to that info icon.

---

## Does a locked miner keep earning?

**Yes.** While the position is open, the locked miner keeps mining and earning BTC rewards for the user as normal. This is the key advantage of Use Miner over selling the miner outright.

Rewards are **frozen only if the position reaches liquidation** — see the Liquidation section.

---

## Amounts

| Parameter | Value |
|-----------|-------|
| Minimum position amount | **5 USDT or USDC** |
| Maximum per **BTC** position | **10,000 USDT or USDC** |
| Maximum per **Miner** position | Depends on the miner's value — see **Get up to** on the Select miner screen |
| Total outstanding across all **Miner** positions | Up to **10,000 USDT or USDC** — counted **separately** from BTC positions |

The two collateral types have **separate quotas**: 10,000 max across BTC positions AND 10,000 max across miner positions is possible in principle.

---

## Position limits

| Collateral | Active positions |
|------------|------------------|
| **BTC** | Up to **3** at a time |
| **Miner** | Counted separately from BTC; **multiple** allowed. When the limit is reached, the **Use Miner** tab shows it. |

---

## Cost

There is **no annual interest (0% APR)**. A **service fee** is charged as a **percentage of the funds amount**, and the percentage **depends on the user's VIP level** — the higher the VIP, the lower the fee.

**When the fee repeats matters, and it differs by collateral:**

| Collateral | Service fee behaviour |
|------------|-----------------------|
| **BTC** | Stays a **one-time** fee **if** auto-renewal is turned off and the position is repaid by the 30-day deadline. If auto-renewal stays on, a new fee is added each time the position auto-renews for another 30 days. |
| **Miner** | Auto-renewal is **always on** and **cannot be turned off**, so a new service fee is **added to the outstanding amount every 30 days** until the user repays in full. The longer the position stays open, the more the user owes, and the higher the risk level. |

Do **not** describe the service fee as always one-time — that's only true for BTC positions with auto-renewal disabled.

### Service Fee by VIP Tier

| Tier | Fee | Tier | Fee |
|------|-----|------|-----|
| Bronze I | 2.5% | Diamond I | 1.88% |
| Bronze II | 2.43% | Diamond II | 1.85% |
| Silver I | 2.36% | Diamond III | 1.81% |
| Silver II | 2.29% | Diamond IV | 1.77% |
| Silver III | 2.21% | Diamond V | 1.73% |
| Gold I | 2.14% | Legend I | 1.69% |
| Gold II | 2.07% | Legend II | 1.65% |
| Platinum I | 2.0% | Legend III | 1.62% |
| Platinum II | 1.96% | Legend IV | 1.58% |
| Platinum III | 1.92% | Legend V | 1.54% |
| — | — | Elite | 1.5% |

---

## Repayment window

Each position has a **30-day repayment window**. Reminders go out before the deadline.

**What happens at the deadline depends on collateral and auto-renewal:**

- **BTC position, auto-renewal ON:** position auto-extends for another 30 days; a new service fee is added.
- **BTC position, auto-renewal OFF:** position may be **closed automatically**, and the outstanding amount is covered from the locked BTC.
- **Miner position (auto-renewal always ON):** position is **not closed** — it is **extended for another 30 days**, with a new service fee added to the outstanding amount.

---

## Auto-renewal

**Auto-renewal** extends a position for another 30 days when the repayment deadline is reached, so the user does not have to repay immediately. When it triggers, the **service fee for the new period is added to the outstanding amount** and the deadline shifts by 30 days.

| Collateral | Auto-renewal default | Can turn off? |
|------------|----------------------|---------------|
| **BTC** | On (default when opening) | **Yes** — anytime |
| **Miner** | On | **No** — cannot be turned off |

---

## Risk level

The **risk level** shows how close a position is to liquidation. It is calculated as **what the user owes ÷ the current USD value of the collateral**.

- **Lower risk level = safer.**
- **Higher risk level = closer to liquidation.**
- The risk level rises when the **collateral loses value** (e.g. BTC price falls, or a miner's USD value drops), **and** when the **outstanding amount grows** (e.g. each time the position auto-renews and a new service fee is added).

Each position shows its **current risk level**, its **warning value** (the collateral level at which the user is notified), and its **liquidation value** (the collateral level at which the position is liquidated).

**Reducing risk:**

- **Partial repayment** at any time — lowers what is owed.
- For a **BTC position**, **adding more BTC** to the locked collateral — lowers the ratio.
- For a **Miner position**, collateral cannot be added (see *Managing a position*) — the only lever is repayment.

**Warnings before liquidation:** if the risk level gets too high, the user receives a **push notification and email** telling them to repay some of the outstanding amount, or (for a BTC position) add more BTC.

---

## Liquidation

**BTC position:** the outstanding amount is covered from the locked BTC, and any remaining BTC is returned to the balance. The position closes.

**Miner position — the miner is NOT lost immediately.** When a miner position is liquidated:

1. **Rewards for the locked miner are frozen** immediately (the miner keeps mining physically, but the BTC it earns is held).
2. A **one-time charge equal to the service fee** is added to the outstanding amount. The Instant Funds screen shows the exact total to repay.
3. The user gets a **7-day window** to buy the miner back — by repaying the **full amount shown**. **Partial repayment is not available during these 7 days.**
4. If repaid in full within the 7 days: the miner is unlocked, resumes earning rewards, and the position is closed.
5. If not repaid within 7 days: the miner **goes on sale** on the Marketplace, and the user is notified. **The BTC rewards the miner would have earned during those 7 days are not returned to the user.**
6. Push and email reminders go out during the 7-day window with the exact deadline.

Do not tell miner-collateral users that liquidation means "instant loss of the miner" — the 7-day recovery window is a documented feature.

---

## Managing a position

From the **Instant Funds** screen, the user can:

| Action | BTC position | Miner position |
|--------|-------------|----------------|
| **Repay** part or all | Yes | Yes — but **only full repayment** during the 7-day post-liquidation window |
| **Add BTC** to locked collateral | Yes — lowers risk | No — collateral cannot be added to a miner position |
| **Withdraw BTC** from locked collateral (when BTC price rose) | Yes — max shown automatically | No |
| **View details** (outstanding, locked collateral, risk level, deadline, liquidation value) | Yes | Yes |
| **Get more funds against the same collateral** | No — open a new position | No — open a new position on **another eligible miner** (can't top up an already-locked miner) |

If a user with a locked miner wants more funds, direct them to open a **new** position on another eligible miner — not to "add more" to the existing one.

---

## Where to find Instant Funds

| Location | Path |
|----------|------|
| Side menu | **Assets → Instant Funds** |
| Bottom tab | **Assets** tab |
| Wallet page | **More** menu on the USDT, USDC, or BTC wallet page |

---

## Regional availability

Instant Funds may not be available in certain jurisdictions.

| Region | Availability | Notes |
|--------|-------------|-------|
| Most countries | Available | USDT and USDC |
| **EEA countries** | Available with **KYC** | Identity verification required; **only USDC** is available — USDT is not supported in the EEA |

---

## What if there's not enough BTC / no eligible miner?

**Not enough BTC:** the app shows a message. Options: buy BTC, deposit from an external wallet, or convert another asset to BTC.

**No eligible miner:** the **Select miner** screen shows a reason next to every miner that can't be used (on sale, MNPL <90 days since final payment, on an external wallet, efficiency > 12 W/TH, already locked as collateral, value too low, or Bonus Miner). The user resolves the reason to make the miner available. The **MNPL case is the exception** — there's nothing to resolve; the user just waits until 90 days from the final payment.

---

## Frequently Asked Questions

### What is Instant Funds?

Instant Funds is a way to access USDT or USDC using your BTC balance or one of your miners as collateral. The asset is locked (not sold) and is returned once you repay the amount you received plus the service fee.

### Can I use a miner as collateral?

Yes. Pick **Use Miner** when opening a position. The miner must be in your GoMining wallet, not for sale, past the MNPL 90-day window (if applicable), ≤ 12 W/TH efficiency, not already locked as collateral, and worth at least the minimum. Bonus miners can't be used.

### Does my miner keep earning while locked?

Yes. The locked miner keeps mining and earning BTC rewards for you. Rewards are only frozen if the position reaches liquidation.

### How much does it cost?

A service fee — a percentage of the funds amount, lower at higher VIP levels — charged when the position opens. For a **BTC** position, it stays a one-time fee if you turn auto-renewal off and repay by the deadline. For a **Miner** position, auto-renewal is always on, so a new service fee is added every 30 days until you repay in full.

### What is the repayment deadline?

Every position has a 30-day repayment window. For a **BTC** position with auto-renewal off, the position may be closed at the deadline (outstanding covered from locked BTC). For a **Miner** position, auto-renewal is always on and the position is extended by another 30 days instead of closing.

### What is auto-renewal?

An automatic 30-day extension when the deadline is reached; a new service fee is added and the deadline shifts. **BTC:** on by default, can be turned off anytime. **Miner:** always on, can't be turned off.

### What happens if my collateral loses value?

Your risk level rises (ratio of owed to collateral). At a high risk level you get a push + email warning. If the risk level reaches the liquidation threshold, the position is liquidated. Reduce risk by repaying part of the outstanding amount, or (BTC positions only) adding more BTC.

### What happens after a miner position is liquidated?

You **don't lose the miner immediately**. Rewards for that miner are frozen, and you get **7 days** to buy it back by paying the **full** amount shown (partial repayment is not available in this window). A one-time charge equal to the service fee is added to what you owe. If you repay in full within 7 days, the miner is unlocked and starts earning again. If not, it goes on sale and the rewards the miner would have earned during those 7 days are not returned.

### Can I manage my position after opening it?

Yes — from the Instant Funds screen. **Repay** part or all (BTC and miner; miner post-liquidation is full-only). **Adjust collateral (add or withdraw BTC)** — **BTC positions only**. **View details** — both. Miner positions cannot receive additional collateral, and you can't get more funds against a miner that's already locked; open a new position with another eligible miner.

### Where can I find Instant Funds?

Side menu **Assets → Instant Funds**; bottom **Assets** tab; **More** menu on the USDT, USDC, or BTC wallet page.

### Is Instant Funds available in my country?

It may not be available in certain jurisdictions. In the EEA, KYC is required and **only USDC** is available (USDT is not supported in the EEA).

### What are the minimum and maximum amounts?

Minimum **5 USDT or USDC**. Maximum per **BTC** position is **10,000 USDT or USDC**. Maximum per **Miner** position depends on the miner's value (see **Get up to** on the Select miner screen). Total outstanding across all **Miner** positions is capped at 10,000 USDT or USDC, counted **separately** from BTC positions.

### How many positions can I have?

Up to **3 active BTC** positions at a time. **Miner** positions are counted separately from BTC and multiple are allowed — the Use Miner tab shows the limit when reached.

### What if I don't have enough BTC?

Buy BTC, deposit from an external wallet, or convert another asset to BTC.

### What if none of my miners can be used?

The Select miner screen shows a reason next to each ineligible miner (on sale, MNPL <90 days, external wallet, >12 W/TH, already locked, value too low, or Bonus Miner). Resolve the reason to make it available. For the MNPL case, there's nothing to resolve — wait until 90 days have passed since the final payment.
