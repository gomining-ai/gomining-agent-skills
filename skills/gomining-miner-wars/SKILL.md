---
name: gomining-miner-wars
description: "GoMining Miner Wars — competitive blockchain-based game (no entry fee) that simulates Bitcoin mining through clan battles and personal competitions. Requires owning at least one Digital Miner to play. Players earn BTC in clan battles and GOMINING tokens in personal competitions. Covers game rules, Points-per-second (PPS) mechanics, 4 leagues (Odyssey, Eclipse, Horizon, Dune), weekly cycles tied to Bitcoin blocks, round multipliers up to x256, Clans (creation requires Gold I+ VIP, 5% royalties), spells and power-ups (Instant/Power/Echo/Focus boosts, Clan Power-up, Miner Service), Spell Bot automation, BTC/GOMINING reward distribution, Bonus Miner power additivity (only on top of owned miners), Platinum+ 15% spell discount, and cross-effects with VIP tiers, GOMINING token utility, and Bonus Miners."
license: Apache-2.0
compatibility: "Compatible with Claude Code, Codex, and all Agent Skills spec tools."
metadata:
  author: gomining
  version: "1.0"
  tags:
    - miner-wars
    - game
    - clans
    - spells
    - leagues
    - btc-rewards
    - gomining-rewards
    - competitive
  triggers:
    - "miner wars"
    - "minerwars"
    - "clan battle"
    - "clan creation"
    - "clan royalties"
    - "league"
    - "odyssey league"
    - "eclipse league"
    - "horizon league"
    - "dune league"
    - "pps"
    - "points per second"
    - "round multiplier"
    - "spells"
    - "power-ups"
    - "instant boost"
    - "echo boost"
    - "focus boost"
    - "spell bot"
    - "clan power-up"
    - "miner service"
    - "miner wars rewards"
    - "miner wars mode"
    - "switch to miner wars"
---

# Miner Wars

## Overview

Miner Wars is a free, competitive blockchain-based game that simulates Bitcoin mining through **clan battles** and **personal competitions**. The game uses real Bitcoin blockchain data — each round starts and ends when a new block is confirmed on the Bitcoin network — to ensure fair and transparent outcomes.

**Players can earn two types of rewards:**

| Reward Type | Earned In | Distribution |
|-------------|-----------|--------------|
| **BTC** | Clan battles | Among Clan members based on personal mining power |
| **GOMINING** | Personal competitions | Among personal battle winners across all leagues |

**You must own at least one Digital Miner to play Miner Wars.** A Bonus Miner alone is not enough — it adds power to your stats *on top of* an owned Digital Miner.

---

## Two Earning Modes for Digital Miners

| Mode | Rewards | Participation | When to Use |
|------|---------|---------------|-------------|
| **Mining Mode** | Passive daily BTC | None — fully automatic | Hands-off, predictable, default |
| **Miner Wars Mode** | Weekly BTC + GOMINING | Active gameplay | Competitive players willing to spend on spells |

Switching is done in the miner's mode settings. See [Mode Comparison](references/MODE-COMPARISON.md) for the full tradeoff table.

---

## Game Cycle

Cycles run on a fixed weekly schedule:

| Aspect | Detail |
|--------|--------|
| **Cycle length** | 7 days |
| **Cycle start** | Tuesday 00:00 UTC |
| **Cycle end** | Next Tuesday 00:00 UTC |
| **Rounds per day** | ~120–150 (depends on Bitcoin block intervals) |
| **Round trigger** | New Bitcoin block confirmed |

Rewards are calculated and distributed at the end of each Cycle.

---

## Leagues

All gameplay takes place in **Leagues** — competitive groups where Clans battle for rewards.

| League  | Clan Slots | Multiplier Range | Description |
|---------|------------|------------------|-------------|
| **Odyssey** | 50 | x1 – x256 | Top League with the highest reward multipliers |
| **Eclipse** | 50 | x1 – x128 | Competitive mid-tier League |
| **Horizon** | 50 | x1 – x64 | League with growth potential |
| **Dune** | Dynamic | x1 – x32 | Entry-level League |

**Promotion/demotion:** 5 Clans move up or down each Cycle between Odyssey, Eclipse, and Horizon, ranked by (1) number of blocks mined and (2) total TH as tiebreaker. Dune divisions are reshuffled each Cycle for fairness.

---

## Core Mechanics (Quick Reference)

### Points-per-second (PPS) Formula

```
PPS = user TH × (base EE / user EE)
```

- `user TH` — total mining power across all your miners
- `base EE` — constant, currently **28 W/TH** (subject to change)
- `user EE` — your miners' average energy efficiency

**Example:** 1 TH at 20 W/TH average → `1 × (28 / 20) = 1.4 points/sec`

Full mechanics in [Game Mechanics](references/MECHANICS.md).

---

## Clans

A **Clan** is the basic game unit. It combines its members' total hash power and average energy efficiency. Clan capacity: **1000 members**. Joining a Clan is required to participate.

**Key Clan facts:**

| Fact | Detail |
|------|--------|
| Clan types | **Public** (auto-join) or **Moderated** (owner approval) |
| Entry requirements | Owner sets minimum TH and/or GOMINING balance (Bonus Miner power excluded) |
| Clan creation | Requires **Gold I+** VIP (100+ TH or 1000+ votes) — up to **3 Clans/year** |
| Owner royalties | **5%** of GOMINING tokens won by Clan members |
| Owner VIP drop | Ownership transfers to highest-TH member if Gold I is not restored |
| Exclusion | Non-owner members can be removed; their miners auto-switch to Mining Mode |

Full details in [Clans](references/CLANS.md).

---

## Spells & Power-ups

Boosts purchased with GOMINING tokens that increase your score during a round.

| Category | Examples | Effect Pattern |
|----------|----------|----------------|
| **Power-up** | Power-up, Clan Power-up | Multiplies base PPS for the round |
| **Instant Boosts** | Instant / Super / Ultra Instant Boost | Add points instantly (3s delay) |
| **Power Boosts** | Power / Super / Ultra Power Boost | Extra points every second until round ends |
| **Echo Boosts** | Echo / Super / Ultra Echo Boost | Points every 2 min, growing over time |
| **Focus Boosts** | Focus / Super / Ultra Focus Boost | Large points, valid for 5 min |
| **Copy Boosts** | Copy / Super / Ultra Copy Boost | Copy a % of the next boost cast in the round |
| **Miner Service** | Miner Service spell | Instant PPS × 1000 + maintenance discount (+0.3%/day, max 3%); free, daily cooldown |

**Spell Bot:** Official GoMining feature that automates spell casting based on round multiplier. Has its own budget separate from main wallet. Safe to use — won't trigger bans.

Full table and tactics in [Spells & Power-ups](references/SPELLS.md).

---

## Rewards (Quick Reference)

### BTC Rewards (Clan Battles)

- Prize fund = pool rewards all league players would have earned in Mining Mode
- Distributed among Clans that won at least 1 block during the Cycle
- Split among Clan members proportional to **individual mining power**

### GOMINING Rewards (Personal Battles)

Prize fund formed from **three sources**:

1. **97.5%** of GOMINING spent on boosts/spells → prize pool
2. **Additional GOMINING** for Odyssey League winners (from weekly emissions, voted via veGOMINING)
3. **Periodic marketing additions** from GoMining campaigns

Full reward mechanics in [Rewards](references/REWARDS.md).

### Maintenance Discounts in Miner Wars

| Discount | Maximum | How |
|----------|---------|-----|
| Miner Service spell | **3%** | Cumulative, +0.3%/day, 10 consecutive days |
| VIP discount | **6%** | Reach Elite tier (starts 0.3% at Bronze II) |
| GOMINING token payment | **20%** | Largest available — pay maintenance in GMT |

---

## Game Rules & Anti-cheat

The following actions cause **temporary suspension or permanent ban**:

- Unauthorized third-party software or bots (Spell Bot is allowed — it's official)
- Multiple accounts
- Collusion / coordinated exploitation
- **League Hopping or Clan Cycling** — intentionally moving between Clans/accounts to manipulate league placement, bypass difficulty scaling, or monopolize promotion slots

---

## Cross-skill Effects

Miner Wars interacts with several other GoMining products. Key effects:

| Source | Effect on Miner Wars |
|--------|----------------------|
| **VIP Gold I+** | Unlocks Clan creation + 5% GOMINING royalties from Clan activity |
| **VIP Elite** | Maximum 6% maintenance discount in Miner Wars Mode |
| **Platinum+ subscription** | 15% discount on every spell (and on Spell Bot casts) |
| **Bonus Miner** | Adds power to your stats — only effective once you own at least one Digital Miner |
| **GOMINING token** | Currency for all spells, power-ups, Spell Bot budget; 20% maintenance discount |
| **veGOMINING votes** | Decide weekly allocation to the Miner Wars prize fund |
| **Referral program** | 2.5% of referrals' GOMINING spent on boosts (calculated weekly) |
| **Avatar discounts** | GoMiners Avatar discount stacks against Platinum+ — highest applies |

Detailed breakdown in [Cross-skill Effects](references/CROSS-SKILL-EFFECTS.md).

---

## Getting Started

1. **Own a Digital Miner** — required to play. Buy from the GoMining marketplace, OpenSea, Magic Eden, or Getgems. (A Bonus Miner can boost your stats but cannot stand alone.)
2. **Switch mode** — in miner settings, switch from Mining Mode to Miner Wars Mode (per-miner setting).
3. **Join a Clan** — browse public Clans, check PPS rate, league, members; apply to moderated ones.
4. **Watch your PPS grow** — score accumulates every second based on TH and energy efficiency.
5. **(Optional) Cast spells** — buy boosts with GOMINING tokens; configure Spell Bot for hands-off play.
6. **Wait for Cycle end** — Tuesday 00:00 UTC; rewards distributed automatically.

---

## Frequently Asked Questions

### Do I need to own a Digital Miner to play?

**Yes.** A Bonus Miner on its own does not let you participate in Miner Wars — its power only contributes to your in-game stats *if you already own at least one Digital Miner*. Buy through GoMining (marketplace, MNPL installments) or on a secondary marketplace (OpenSea / Magic Eden / Getgems).

Note: Clan entry requirements (TH/GOMINING) **don't count Bonus Miner power** either — they look only at your owned miners' TH and your GMT balance.

### How long is a Cycle?

7 days, running Tuesday 00:00 UTC to next Tuesday 00:00 UTC.

### How are BTC rewards split inside a Clan?

Proportional to each member's individual mining power.

### What happens if I lose my Clan?

If you are not the Clan Owner, the Owner can revoke your membership without explanation. Your miners auto-switch to Mining Mode.

### Can I get banned for using a bot?

Third-party bots are banned. **Spell Bot is the only allowed automation** — it's an official GoMining feature.

### How are GOMINING rewards calculated?

97.5% of all GOMINING spent on spells in the Cycle goes to the personal-battle prize pool, plus Odyssey League gets additional GOMINING from weekly emissions, plus periodic marketing top-ups.

### Is the round multiplier random?

It's determined by how many Bitcoin blocks are mined simultaneously on the real Bitcoin network. Higher leagues unlock higher max multipliers (up to x256 in Odyssey).

---

## Glossary (Top Terms)

| Term | Definition |
|------|------------|
| **PPS** | Points-per-second — how fast your score grows |
| **Cycle** | 7-day reward period (Tue 00:00 UTC → Tue 00:00 UTC) |
| **Round** | Single gameplay unit, bounded by Bitcoin block confirmations |
| **Multiplier** | Round weight multiplier (x1 – x256), based on simultaneous blocks |
| **League** | Competitive group of Clans (Odyssey / Eclipse / Horizon / Dune) |
| **Clan** | Team of up to 1000 players competing together |
| **Spell** | Paid in-game boost activated during a round |
| **Power-up** | Multiplier-style boost active for the entire round |
| **Spell Bot** | Official automation that casts spells based on multiplier |
| **Bonus Miner** | Free promotional miner — adds power to your Miner Wars stats only if you own a Digital Miner |

Full list: [Glossary](references/GLOSSARY.md).

---

## Official Resources

| Resource | URL |
|----------|-----|
| Miners FAQ | https://help.nft.gomining.com/ |
| Main Website | https://gomining.com/ |

---

## References

- [Game Mechanics](references/MECHANICS.md) — PPS formula, leagues, rounds, multipliers, promotion/demotion
- [Clans](references/CLANS.md) — joining, creating, ownership, entry rules, logo requirements
- [Spells & Power-ups](references/SPELLS.md) — every spell type (Power-up, Clan Power-up, Miner Service, Instant/Power/Echo/Focus/Copy boosts) and tactics
- [How-to: Set Up Spell Bot](references/INSTRUCTION-SPELL-BOT.md) — step-by-step Spell Bot setup, budget, priority ordering, tips
- [Rewards](references/REWARDS.md) — BTC/GOMINING prize fund formation, distribution, maintenance discounts
- [Mode Comparison](references/MODE-COMPARISON.md) — Mining Mode vs Miner Wars Mode side-by-side
- [Cross-skill Effects](references/CROSS-SKILL-EFFECTS.md) — how VIP, Platinum+, tokens, Bonus Miner, referrals interact with Miner Wars
- [Cheatsheet](references/CHEATSHEET.md) — one-page reference with all key formulas, thresholds, multipliers, and limits
- [FAQ & Troubleshooting](references/FAQ-TROUBLESHOOTING.md) — common pain points: spell delays, empty Spell Bot budget, clan exclusion, withdrawal issues, ban triggers
- [Glossary](references/GLOSSARY.md) — full term dictionary
