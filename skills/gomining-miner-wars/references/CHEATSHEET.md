# Miner Wars Cheatsheet

One-page reference. Every number on this sheet is sourced from other files in this skill — if values change, update the source file and this cheatsheet together.

---

## Cycle

| | |
|---|---|
| Cycle length | 7 days |
| Cycle start / end | **Tuesday 00:00 UTC** |
| Rounds per day | ~120–150 (Bitcoin block intervals) |
| Round trigger | New Bitcoin block confirmed |

---

## PPS Formula

```
PPS = user TH × (base EE / user EE)
```

- `base EE` = **28 W/TH** (subject to change)
- Lower (better) user EE → more PPS per TH

---

## Leagues

| League | Slots | Multiplier Range | Notes |
|---|---|---|---|
| **Odyssey** | 50 | x1 – x256 | Extra GMT from weekly emissions |
| **Eclipse** | 50 | x1 – x128 | |
| **Horizon** | 50 | x1 – x64 | |
| **Dune** | Dynamic | x1 – x32 | Reshuffled each Cycle |

**Promotion/demotion:** 5 Clans up or down per Cycle between Odyssey/Eclipse/Horizon. Ranked by (1) blocks mined, (2) total TH as tiebreaker.

---

## Clans at a Glance

| | |
|---|---|
| Max members | **1000** |
| Types | **Public** (auto-join) / **Moderated** (owner approval) |
| Entry requirements | Owner-set TH and/or GMT (Bonus Miner power **excluded**) |
| Creation requirement | **Gold I+** VIP (100+ TH or 1000+ veGOMINING votes) |
| Clans per year | **3** max per creator |
| Owner royalty | **5%** of GOMINING won by members |
| Owner VIP drop | >24h to Cycle end: restore status by end; <24h: keep through next Cycle |
| Non-owner exclusion | No explanation required; miners auto-switch to Mining Mode |
| Logo | JPG/PNG, up to 2 MB, original, no trademarks |

---

## Spells & Power-ups — At a Glance

| Spell | Effect | Delay | Window |
|---|---|---|---|
| Power-up | ×100 base PPS for round | none | until round ends; **once/round** |
| Clan Power-up | +PPS for all members; scales with activations | none | once/member/round |
| Miner Service | +PPS × 1000 points + maintenance discount | none | **once/day** (free, daily cooldown) |
| Instant / Super / Ultra Instant | +points (×1 / ×10 / ×100) | **3s** | instant |
| Power / Super / Ultra Power | +points/sec (×1 / ×10 / ×100) | none | until round ends |
| Echo / Super / Ultra Echo | +points every 2 min, growing | none | until round ends |
| Focus / Super / Ultra Focus | large points (×1 / ×10 / ×100) | **3s** | **5 min validity** |
| Copy / Super / Ultra Copy | copies % (×1 / ×10 / ×100) of **next** boost | none | until target boost cast |

**Clan Power-up growth (boost per activation):**

| Activations | 1–4 | 5–9 | 10–29 | 30–49 | 50–99 | 100–199 | 200–499 | 500–1000 |
|---|---|---|---|---|---|---|---|---|
| Per activation | +1 | +1.3 | +1.7 | +2.2 | +2.9 | +3.8 | +4.9 | +6.4 |

---

## Maintenance Discounts (Stackable)

| Source | Max | How |
|---|---|---|
| Miner Service spell | **3%** | +0.3%/day, 10 consecutive days |
| VIP tier | **6%** | Bronze II (0.3%) → Elite (6%) |
| GOMINING token payment | **20%** | Pay maintenance in GMT |
| **Theoretical max** | **~29%** | All three combined |

---

## Reward Funds

### BTC (Clan Battles)
- Fund = pool rewards all league players would have earned in Mining Mode
- Goes to Clans that won ≥1 block during Cycle
- Within Clan: proportional to **individual mining power**

### GMT (Personal Battles)
- **97.5%** of GMT spent on spells → prize pool
- **+** Additional GMT for Odyssey winners (from weekly emissions vote)
- **+** Periodic marketing top-ups
- Withdraw: up to **30,000 GMT/day** via BEP-20 / ERC-20 / TON

---

## VIP Tiers Relevant to Miner Wars

| Tier | Threshold | Miner Wars Effect |
|---|---|---|
| Bronze II | (entry) | 0.3% maintenance discount |
| **Gold I** | **100+ TH or 1000+ votes** | **Unlocks Clan creation + 5% royalties** |
| Elite | (top tier) | **6%** maintenance discount (max) |

**Platinum+ subscription:** 15% off **every spell** (incl. Spell Bot casts). Does **not stack** with GoMiners Avatar discount — highest applies.

---

## Anti-Cheat Rules → Ban Triggers

- Third-party software or bots (Spell Bot is **allowed** — it's official)
- Multi-accounting
- Collusion / coordinated exploitation
- **League Hopping / Clan Cycling** — moving between Clans to manipulate placement

---

## Bonus Miner Quick Facts

- **Does NOT enable solo play** — has Miner Wars effect only if you own at least one Digital Miner
- Once you own a miner: Bonus Miner power **adds** to your stats
- In Clan reward math: counts only for rounds it was active
- **Excluded** from Clan entry requirements (TH/GMT minimums)
- Auto-reinvest in TH **cannot** be enabled for Bonus Miner
- Rewards withdrawal: only after buying a miner from GoMining or opening a Card

---

## Spell Bot Quick Facts

- Setup = one multiplier (x1 → x256) + ordered spell list + quantities
- Budget is **separate** from main wallet
- **Empty budget disables ALL Setups** (not just active)
- Cast order: top-down; lower-priority spells skipped if budget runs out
- Power-up / Clan Power-up costs **scale with PPS** (yellow icon)
- Miner Service: don't add to Spell Bot (free, daily cooldown)
- Same spell can't be added twice — use quantity buttons

---

## Referral (Ambassador) — Miner Wars

| | |
|---|---|
| Boost spending | **2.5%** of referrals' GMT spent on boosts (weekly) |
| Electricity rewards | Calculated **weekly** at Cycle end (not daily); weighted avg EE |

---

## When to Switch Mode

| Stay in Mining Mode | Switch to Miner Wars |
|---|---|
| Want predictable daily BTC | Willing to spend GMT on spells |
| Miner has active power upgrade subscription | Want GMT rewards too |
| Listed for sale or MNPL miner | In a strong Clan (high PPS / league) |
| No time for active play | Targeting Clan ownership (Gold I+) |
