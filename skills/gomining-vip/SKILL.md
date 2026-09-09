---
name: gomining-vip
description: "GoMining VIP loyalty program — tiered benefits system based on hashrate (TH), veGOMINING votes, or referral activity. Covers tier progression from Bronze I through Elite, per-level thresholds, maintenance discounts, Launchpad access tiers, Reinvestment bonuses, Clan creation in Miner Wars, dedicated VIP managers, card cashback rates, travel cashback, GoBox rewards per tier, Platinum+ subscription for instant VIP benefits, Simple Earn APR by tier, and the referral program inside VIP."
license: Apache-2.0
compatibility: "Compatible with Claude Code, Codex, and all Agent Skills spec tools."
metadata:
  author: gomining
  version: "1.2"
  tags:
    - vip
    - loyalty
    - tiers
    - hashrate
    - vegomining
    - cashback
    - launchpad
    - subscription
    - platinum+
    - simple-earn
    - referral
  triggers:
    - "vip program"
    - "vip tiers"
    - "loyalty program"
    - "vip benefits"
    - "cashback rates"
    - "maintenance discount"
    - "launchpad access"
    - "platinum+ subscription"
    - "vip subscription"
    - "platinum subscription"
    - "grow rewards"
    - "increase rewards"
    - "simple earn apr"
    - "simple earn multiplier"
    - "vegomining lock"
    - "lock duration"
    - "wallet days"
    - "locked days"
    - "referral toggle"
    - "referral balance"
    - "referral vip"
    - "referral royalty"
---

# GoMining VIP Program

## Overview

The GoMining VIP program is a loyalty system that rewards users based on their hashrate (TH) or veGOMINING voting power. Users progress through tiers to unlock increasing benefits including maintenance discounts, Launchpad allocations, cashback rates, Simple Earn APR boosts, and exclusive perks.

---

## Tier Structure

The VIP program has the following tiers, with sub-levels as shown on the **All VIP levels** screen:

| Tier | Sub-levels | Description |
|------|------------|-------------|
| **Bronze** | I, II | Entry-level tier for all users |
| **Silver** | I, II, III | Unlocked via 10 TH or 100 veGOMINING votes |
| **Gold** | I, II | Mid-level tier with Clan creation access |
| **Platinum** | I, II, III | Premium tier with dedicated VIP manager |
| **Diamond** | I, II, III, IV, V | High-tier with Tier 1 Launchpad access (x700) |
| **Legend** | I, II, III, IV, V | Highest cashback (5%) and largest GoBox |
| **Elite** | — | Single top-tier level (no sub-levels) |

---

## Tier Progression

Your VIP tier is based on **whichever single input is highest**. The VIP status screen lists **three** qualification paths and states *"Reach it by any one of these"*:

| Path | Unit |
|------|------|
| **Power** | TH |
| **Votes** | veGOMINING |
| **Referral activity** | USD |

You don't need all three — the stronger single measure sets your tier. For the full per-level threshold table (Bronze I through Platinum I, all three paths), see [VIP Level Thresholds](references/VIP-LEVEL-THRESHOLDS.md).

### Silver I Requirements (Entry Gateway)

| Requirement | Threshold |
|-------------|----------|
| Hashrate | 10 TH |
| veGOMINING votes | 100 veGOMINING |
| Referral activity | $1K |

### Estimated veGOMINING Route Costs (March 2026)

| Tier | veGOMINING Required | Approx. Cost (at $0.30/token) |
|------|---------------------|-------------------------------|
| Silver I | 100 | ~$30 |
| Silver II | 250 | ~$75 |
| Silver III | 500 | ~$150 |
| Gold I | 1,000 | ~$300 |
| Platinum I | 5,000 | ~$1,500 |

**Note:** Tokens are locked (not spent) when converted to veGOMINING. Costs fluctuate with token price. For current GOMINING price, see [Live Market Data](../gomining-overview/references/LIVE-MARKET-DATA.md).

---

### Complete Tier Criteria & Benefits

| Tier | Min TH | Min veGOM | Maint. Discount | Card Cashback | SE Multiplier | Travel Cashback | Instant Funds Fee | Launchpad | GoBox | Feature |
|------|--------|-----------|----------------|--------------|--------------|----------------|-------------------|-----------|-------|---------|
| **Bronze I** | 0 | 0 | 0% | 0.5% | x1 | 1% | 2.5% | — | — | — |
| **Bronze II** | 5 | 50 | 0.3% | 0.5% | x1.08 | 1% | 2.43% | — | Bronze | — |
| **Silver I** | 10 | 100 | 0.6% | 1% | x1.1 | 1.6% | 2.36% | x1 (Tier 1) | Silver | Reinvestment in TH (+5%) |
| **Silver II** | 25 | 250 | 0.9% | 1% | x1.12 | 1.6% | 2.29% | x2.5 (Tier 2) | Silver | — |
| **Silver III** | 50 | 500 | 1.2% | 1% | x1.14 | 1.6% | 2.21% | x5.3 (Tier 3) | Silver | — |
| **Gold I** | 100 | 1,000 | 1.5% | 1.5% | x1.16 | 2.2% | 2.14% | x11 (Tier 4) | Gold | Clan ownership (5% royalties) |
| **Gold II** | 200 | 2,000 | 1.8% | 1.5% | x1.18 | 2.2% | 2.07% | x23 (Tier 5) | Gold x2 | — |
| **Platinum I** | 500 | 5,000 | 2.1% | 2% | x1.2 | 2.8% | 2% | x60 (Tier 6) | Platinum | VIP-support & special offers |
| **Platinum II** | 1,000 | 10,000 | 2.4% | 2% | x1.22 | 2.8% | 1.96% | x125 (Tier 7) | Platinum x2 | — |
| **Platinum III** | 2,500 | 25,000 | 2.7% | 2% | x1.24 | 2.8% | 1.92% | x330 (Tier 8) | Platinum x3 | — |
| **Diamond I** | 5,000 | 50,000 | 3% | 3% | x1.26 | 3.4% | 1.88% | x700 (Tier 9) | Diamond | Reinvestment in TH (+10%) |
| **Diamond II** | 7,000 | 70,000 | 3.3% | 3% | x1.28 | 3.4% | 1.85% | x700 (Tier 9) | Diamond x2 | — |
| **Diamond III** | 9,000 | 90,000 | 3.6% | 3% | x1.3 | 3.4% | 1.81% | x700 (Tier 9) | Diamond x3 | — |
| **Diamond IV** | 12,000 | 120,000 | 3.9% | 3% | x1.32 | 3.4% | 1.77% | x700 (Tier 9) | Diamond x4 | — |
| **Diamond V** | 20,000 | 200,000 | 4.2% | 3% | x1.34 | 3.4% | 1.73% | x700 (Tier 9) | Diamond x5 | — |
| **Legend I** | 50,000 | 500,000 | 4.5% | 5% | x1.36 | 4% | 1.69% | x700 (Tier 9) | Legend | Coming soon |
| **Legend II** | 100,000 | 1,000,000 | 4.8% | 5% | x1.38 | 4% | 1.65% | x700 (Tier 9) | Legend x2 | — |
| **Legend III** | 250,000 | 2,500,000 | 5.1% | 5% | x1.4 | 4% | 1.62% | x700 (Tier 9) | Legend x3 | — |
| **Legend IV** | 400,000 | 4,000,000 | 5.4% | 5% | x1.42 | 4% | 1.58% | x700 (Tier 9) | Legend x4 | — |
| **Legend V** | 750,000 | 7,500,000 | 5.7% | 5% | x1.44 | 4% | 1.54% | x700 (Tier 9) | Legend x5 | — |
| **Elite** | 1,000,000 | 10,000,000 | 6% | 5% | x1.46 | 4% | 1.5% | x700 (Tier 9) | Legend x6 | Coming soon |

**Note:** Only one condition (TH or veGOMINING) needs to be met. Tokens are locked (not spent) when converted to veGOMINING. For current GOMINING price, see [Live Market Data](../gomining-overview/references/LIVE-MARKET-DATA.md).

---

## veGOMINING Locking Mechanics

When you lock GOMINING tokens, you receive **veGOMINING votes** that count toward your VIP tier. Understanding how the lock works is important for maintaining your tier over time.

### How Votes Decrease Over Time

veGOMINING votes **gradually decrease** as your lock period progresses. This is by design — the system rewards longer, more committed locks with more votes. As time passes and your lock approaches its end date, your vote count falls, which can cause your VIP tier to drop if you don't act.

### Wallet Days vs. Locked Days

The GoMining locking interface shows two separate day counts:

- **Locked days** — the number of days remaining in your active lock period
- **Wallet days** — additional days accumulated in your wallet that are not yet locked

These two values are **not automatically combined**. Your current veGOMINING votes are calculated from your locked days only. Wallet days represent potential voting power that you can apply by extending or creating a new lock.

**Example from a user query:** If you have 365 locked days and 123 wallet days, your votes are based on the 365 locked days. The 123 wallet days are available but not yet contributing to your VIP tier until you lock them.

### Adding TH and Its Interaction with Lock Periods

Adding TH (mining power) to your farm is **independent** of your veGOMINING lock. Your VIP tier is always set by whichever is higher — TH or veGOMINING votes — so:

- If your TH-based tier is higher than your current veGOMINING-based tier, your VIP level will reflect the TH value immediately.
- Adding TH does **not** extend, reset, or modify your veGOMINING lock period.
- If you want to combine both paths (e.g., target 500 days of effective lock with a specific TH level), you need to manage the lock extension separately from your TH purchases.

### Maintaining Your veGOMINING Tier

Because votes decrease over time, you may need to:
1. **Extend your lock period** — adds more days to your lock, restoring or increasing your vote count
2. **Lock additional tokens** — increases the base amount locked, which raises your vote count
3. **Switch to TH-based progression** — if your mining power exceeds your veGOMINING tier, TH takes over automatically

For detailed veGOMINING mechanics, see the [veGOMINING and Governance FAQ](https://help.token.gomining.com/faq/tokenomics/vegomining-and-locks).

---

## Perks by Tier

### Maintenance Discounts

All VIP tiers receive progressive maintenance fee discounts that increase with each tier. Higher tiers enjoy significantly reduced operating costs for their miners.

### Simple Earn APR by Tier

Your VIP tier directly affects your Simple Earn yield through a **multiplier** applied to the base APR. Multipliers rise by **+0.02** per sub-tier from Platinum I upward, ending at **x1.46** for Elite:

| Tier | Simple Earn Multiplier |
|------|------------------------|
| Bronze / Silver / Gold | Base and progressive (see the app **All VIP levels** screen) |
| Platinum I | x1.20 |
| Platinum II | x1.22 |
| Platinum III | x1.24 |
| Diamond I | x1.26 |
| Diamond II | x1.28 |
| Diamond III | x1.30 |
| Diamond IV | x1.32 |
| Diamond V | x1.34 |
| Legend I | x1.36 |
| Legend II | x1.38 |
| Legend III | x1.40 |
| Legend IV | x1.42 |
| Legend V | x1.44 |
| Elite | x1.46 |

Platinum I is also the multiplier granted by the **Platinum+ subscription** (see subscription section below). Full per-tier benefits (Discount, Card/Travel Cashback, Instant Funds Fee, Referral Royalty, Launchpad, Feature, GoBox) are in [VIP Benefits](references/VIP-BENEFITS.md).

### Launchpad Access

| Tier | Launchpad Multiplier | Launchpad Tier |
|------|----------------------|----------------|
| Bronze / Silver / Gold | See the app All VIP levels screen | (Sub-Tier 9) |
| Platinum I | x60 | Tier 6 |
| Platinum II | x125 | Tier 7 |
| Platinum III | x330 | Tier 8 |
| Diamond I through Elite | x700 | Tier 9 |

The biggest single step is **Platinum III → Diamond I** (x330 → x700). Every tier above Diamond I gives the same **x700 / Tier 9** allocation.

### Tier-Specific Perks

| Tier | Perk | Details |
|------|------|---------|
| **Silver I** | Reinvestment Bonus | +5% bonus on all reinvestments |
| **Silver I** | Launchpad Allocations | Access to Launchpad token sales |
| **Gold I** | Clan Creation | Create Clans in Miner Wars |
| **Gold I** | GOMINING Royalties | 5% GOMINING royalties from Clan activity |
| **Platinum I** | VIP-support and special offers | Includes the dedicated VIP manager (see below) |
| **Diamond I** | Reinvestment in TH (+10%) | +10% bonus specifically on TH reinvestment |
| **Diamond I+** | Tier 1 Launchpad | Priority access — x700 / Tier 9 allocation |
| **Legend I** | "Coming soon" feature | Not yet detailed in the source screen |
| **Elite** | "Coming soon" feature | Not yet detailed in the source screen |

---

## Card Cashback Rates

VIP tier determines the cashback percentage for GoMining Card transactions and travel bookings. Within Platinum / Diamond / Legend bands the cashback is **flat across sub-levels** — Platinum I, II, and III all pay the same Card Cashback, and similarly for Diamond I–V and Legend I–V.

| Tier | Card Cashback | Travel Cashback |
|------|--------------|------------------|
| **Bronze** | 0.5% | 1.0% |
| **Silver** | 1.0% | 1.6% |
| **Gold** | 1.5% | 2.2% |
| **Platinum I / II / III** | 2% | 2.8% |
| **Diamond I / II / III / IV / V** | 3% | 3.4% |
| **Legend I / II / III / IV / V** | 5% | 4% |
| **Elite** | 5% | 4% |

**Notes:**
- Cashback is applied automatically to eligible transactions.
- Travel cashback applies to bookings made through the GoMining Travel service.
- Elite Card Cashback (5%) and Travel Cashback (4%) match Legend rates — Elite differentiates on Discount, Simple Earn multiplier, Instant Funds Fee, and GoBox, not on cashback.

---

## How to Actively Grow Your Rewards

There are several strategies to maximize your earnings within the VIP program:

### 1. Reinvest Mining Rewards into TH

From Silver I onward, you can reinvest your BTC mining rewards into additional mining power with a **+5% bonus** on top of the reinvestment amount. This compounds your earnings by:
- Increasing your TH, which may push you to a higher VIP tier
- Generating more BTC rewards from the additional power
- Potentially unlocking better maintenance discounts at higher tiers

**Workflow:** Go to your mining dashboard → select Reinvest → your BTC rewards are converted to TH with the +5% bonus applied automatically.

### 2. Maximize Simple Earn APR

Your Simple Earn yield scales with your VIP tier multiplier. To grow Simple Earn returns:
- Advance your VIP tier to unlock a higher multiplier
- Use the Platinum+ subscription (x1.2 multiplier) if you want the boost without accumulating TH or veGOMINING
- Deposit more into Simple Earn products — the multiplier applies to your full balance

### 3. Lock GOMINING Tokens for veGOMINING

Locking tokens gives you veGOMINING votes that can raise your VIP tier without purchasing additional TH. Higher tiers unlock better maintenance discounts and cashback rates, which reduce costs and increase net returns.

### 4. Compound the Cycle

A compounding approach:
1. Earn BTC from mining
2. Reinvest BTC into TH (+5% bonus at Silver I+)
3. Higher TH → higher VIP tier → better maintenance discount
4. Lower maintenance costs → more net BTC retained
5. Repeat

---

## Platinum+ Subscription

The **Platinum+ Subscription** is an alternative path to premium VIP benefits without accumulating TH or veGOMINING votes.

### How It Works

- Pay a subscription fee to instantly unlock Platinum I-level benefits
- **Does not change your VIP tier** — benefits are granted independently
- Ideal for new users or those who prefer subscription over asset accumulation

### Subscription Benefits

| Benefit | Value |
|---------|-------|
| Card Cashback | 2% on purchases |
| Maintenance Discount | 2.1% savings |
| Spell Discounts | 15% off (Miner Wars) |
| Simple Earn APR Boost | x1.2 multiplier |
| Dedicated VIP Manager | Yes |
| Launchpad | Tier 6 allocations (x60) |

### Free Platinum+ via Referrals

When you refer a friend, the referred **friend** (the new user) receives **1 month of VIP Platinum+ free**, activatable within 30 days of the friend's registration.

---

## Referral Program Inside VIP

The referral program is integrated into the VIP system in two directions:

- **Referral activity as a VIP progression path (live).** The VIP status screen lists **Referral activity** (a USD figure) alongside Power and Votes as one of the three ways to reach the next level, and the All VIP levels screen shows a referral threshold for every level — see [VIP Level Thresholds](references/VIP-LEVEL-THRESHOLDS.md). Referral activity reflects your referrals' **last 180 days** and updates once a day (see [Referral FAQ](../gomining-promos/references/FAQ-REFERRAL.md)).
- **Referral royalty rate tied to VIP tier (live).** The mining royalty on referrals' miner purchases and upgrades is a **progressive rate that rises with your VIP level** — not a flat 5%. The VIP status screen shows the current rate as a **Referral mining royalty** card. Exact per-tier rates are shown in the user's own VIP section; quote them from there rather than from memory.

---

## Referral Balance in the VIP Area

Some users see a dollar amount (e.g., **$20.00**) displayed next to the referral toggle on their VIP or home screen, but then see **$0.00** when they navigate into the full referral section.

This discrepancy typically occurs because:
- The toggle/widget shows a **pending or recently credited** referral reward that has not yet been claimed or processed in the referral dashboard
- The referral section may display only **settled/available** balances, while the widget reflects a broader or real-time figure

If the amounts don't reconcile after refreshing, contact GoMining support through your account for clarification on the specific balance state.

---

## Key Rules

1. **Progression is dynamic:** If your hashrate or veGOMINING drops below the threshold, your tier may be adjusted downward.
2. **Benefits are cumulative:** Higher tiers retain all benefits from lower tiers.
3. **Reinvestment bonus:** The +5% reinvestment bonus at Silver I applies on top of base reinvestment returns.
4. **Clan royalties:** The 5% GOMINING royalties at Gold I are earned from members' Clan activity in Miner Wars.
5. **Platinum+ is independent:** Subscription benefits apply separately from tier-based benefits.
6. **veGOMINING votes decrease over time:** You may need to extend your lock or lock more tokens to maintain your tier.
7. **Three inputs:** VIP tier is based on power (TH), veGOMINING votes, or referral activity (USD) — whichever single path is highest. The VIP status screen shows all three with the wording "Reach it by any one of these".

---

## FAQ

### How do I check my current VIP tier?
Your VIP tier is displayed in your GoMining dashboard profile. It updates automatically when your hashrate or veGOMINING balance changes.

### How is my VIP tier determined?
Your tier is set by **whichever single path is highest**: mining power (TH), veGOMINING votes, or referral activity (in USD). You don't need all three — the VIP status screen lists them under "Reach it by any one of these" and marks the one you're closest to.

### How quickly does my tier update after increasing hashrate?
Tier updates happen in **real time** — as soon as your TH or veGOMINING votes change, your level is updated instantly.

### What are wallet days vs. locked days in veGOMINING?
**Locked days** are the days remaining in your active lock — these determine your current vote count. **Wallet days** are additional days available in your wallet that are not yet locked and therefore not yet contributing to your VIP tier. To use wallet days, you need to extend or create a lock.

### If I add TH, does it affect my veGOMINING lock?
No. Adding TH is completely independent of your veGOMINING lock. Your VIP tier will simply reflect whichever is higher — your TH-based tier or your veGOMINING-based tier — at any given moment.

### Why do my veGOMINING votes decrease over time?
The locking mechanics are designed so that votes gradually decrease as your lock period progresses toward its end date. To maintain your tier, you can extend your lock period or lock additional tokens.

### How do I grow my rewards?
The main strategies are: (1) reinvest BTC rewards into TH for the +5% bonus at Silver I+, (2) advance your VIP tier to unlock a higher Simple Earn APR multiplier, (3) lock GOMINING tokens to raise your tier via veGOMINING votes, and (4) compound the cycle — more TH → higher tier → better discounts → more net BTC retained.

### What Simple Earn APR multiplier do I get at each tier?
Multipliers rise by **+0.02** per sub-tier from Platinum I upward: **Platinum I x1.20, Platinum II x1.22, Platinum III x1.24, Diamond I x1.26, Diamond II x1.28, Diamond III x1.30, Diamond IV x1.32, Diamond V x1.34, Legend I x1.36, Legend II x1.38, Legend III x1.40, Legend IV x1.42, Legend V x1.44, Elite x1.46.** For Bronze / Silver / Gold multipliers, refer users to the in-app **All VIP levels** screen. Platinum+ subscription grants the Platinum I x1.20 multiplier.

### I see $20 next to my referral toggle but $0 in the referral section — why?
The toggle/widget may show a pending or recently credited referral reward, while the referral section displays only settled/available balances. If the discrepancy persists after refreshing, contact GoMining support for clarification.

### Do maintenance discounts stack with other promotions?
Maintenance discounts from VIP tiers are applied as the base discount. Promotional discounts may or may not stack depending on the specific promotion terms.

### What happens to my Clan if I drop below Gold I?
If your tier drops below Gold I, you may lose the ability to manage your Clan. Existing Clans remain but management features are restricted until the tier is restored.

### Is Elite tier invitation-only?
**No.** Elite is the highest tier but it is reached by the same three-path rule as every other tier — any one of **1M TH**, **10M veGOMINING votes**, or **$100M referral activity** qualifies. Do not tell users Elite is invitation-only or has hidden extra requirements; it is a threshold like the others (just much higher). The "Coming soon" feature on Elite is a benefit-slot, not a qualification.

### What is Platinum+ Subscription?
Platinum+ is a paid subscription ($29.99/30 days) that grants Platinum I-level benefits (2% cashback, 2.1% maintenance discount, 15% spell discounts, x1.2 Simple Earn APR boost, Tier 6 Launchpad allocations) without requiring TH or veGOMINING holdings. It does not change your actual VIP tier.

### Can I have both Platinum+ Subscription and a higher VIP tier?
Yes. If you're already Diamond or Legend tier, Platinum+ subscription-specific benefits like the APR boost and 15% Miner Wars spell discount still apply on top of your existing tier benefits.

---

## References

- [VIP Level Thresholds](references/VIP-LEVEL-THRESHOLDS.md) — Per-level power / votes / referral-activity thresholds and the VIP status screen layout
- [FAQ: VIP Program](references/FAQ-VIP-PROGRAM.md) — How the VIP program works, tier progression, and benefits
- [FAQ: Platinum+ Subscription](references/FAQ-VIP-SUBSCRIPTION.md) — The Platinum+ subscription, pricing, and what it includes
- [FAQ: GoBoxes](references/FAQ-GOBOXES.md) — GoBox mystery boxes, collections, and prize mechanics
- [FAQ: VIP Progression Rules](references/FAQ-VIP-PROGRESSION-RULES.md) — Secondary market, wallet linkage, GoBox eligibility, August 2025 policy
