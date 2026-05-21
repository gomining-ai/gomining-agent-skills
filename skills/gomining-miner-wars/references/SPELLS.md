# Spells & Power-ups

Spells and Power-ups let you boost your score and gain an advantage during a round. The exact value of each spell may vary from cycle to cycle and is displayed directly on the item in the game.

All spells and power-ups are paid for in **GOMINING tokens**.

---

## Power-ups

### Power-up

Multiplies your base PPS by **100** until the end of the round.

* Can only be used once per round
* Cost scales with your base PPS

---

### Clan Power-up

Increases the base PPS of **every Clan member** for the current round. The more Clan members activate it, the stronger the effect.

* Each Clan member can activate it once per round
* Every activation increases the base PPS for all members

**Growth table**

| Activations | Boost per activation |
| ----------- | -------------------- |
| 1–4         | +1                   |
| 5–9         | +1.3                 |
| 10–29       | +1.7                 |
| 30–49       | +2.2                 |
| 50–99       | +2.9                 |
| 100–199     | +3.8                 |
| 200–499     | +4.9                 |
| 500–1000    | +6.4                 |

---

## Spells

### Miner Service

Gives you extra points and a **cumulative maintenance discount**.

* **Instant points:** equal to your PPS × 1000
* **Maintenance discount:** +0.3% per consecutive day of use, up to a maximum of **3%** (after 10 days in a row)
* **Free to cast** — but has a **daily cooldown** (once per day). Cast it manually rather than adding it to a Spell Bot Setup.

---

### Instant Boosts

Add points to your score instantly. Useful at any point in the round.

Instant boosts take effect with a **3-second delay**. If the round ends during those 3 seconds, you will not receive points.

| Boost               | Effect                                |
| ------------------- | ------------------------------------- |
| Instant Boost       | Adds extra points instantly           |
| Super Instant Boost | Adds 10× the points of Instant Boost  |
| Ultra Instant Boost | Adds 100× the points of Instant Boost |

---

### Power Boosts

Increase your PPS until the end of the round. **Most effective when used early.**

| Boost             | Effect                                              |
| ----------------- | --------------------------------------------------- |
| Power Boost       | Adds extra points every second until the round ends |
| Super Power Boost | Adds 10× the points of Power Boost every second     |
| Ultra Power Boost | Adds 100× the points of Power Boost every second    |

---

### Echo Boosts

Grant points every 2 minutes, with the amount increasing over time. **No immediate effect** — the longer the round, the more powerful they become.

| Boost            | Effect                                           |
| ---------------- | ------------------------------------------------ |
| Echo Boost       | Grants points every 2 min, increasing over time  |
| Super Echo Boost | Grants 10× the points of Echo Boost every 2 min  |
| Ultra Echo Boost | Grants 100× the points of Echo Boost every 2 min |

---

### Focus Boosts

Grant a large number of points after a 3-second delay. Points are valid for **5 minutes** — if the round ends within that window, you receive them.

| Boost             | Effect                                              |
| ----------------- | --------------------------------------------------- |
| Focus Boost       | Grants points for 5 minutes only                    |
| Super Focus Boost | Grants 10× the points of Focus Boost for 5 minutes  |
| Ultra Focus Boost | Grants 100× the points of Focus Boost for 5 minutes |

---

### Copy Boosts

Copy a **percentage of the next boost** cast in the same round. They don't generate points on their own — they amplify whatever boost comes after them.

| Boost            | Effect                                          |
| ---------------- | ----------------------------------------------- |
| Copy Boost       | Copies a % of the next boost                    |
| Super Copy Boost | Copies 10× the % of Copy Boost                  |
| Ultra Copy Boost | Copies 100× the % of Copy Boost                 |

> **Ordering matters:** in Spell Bot, place Copy boosts **earlier** in the cast order than the boost they should copy. Cast manually before the target boost.

---

## When Each Spell Type Helps Most

| Round expectation | Best fit | Why |
|-------------------|----------|-----|
| Short rounds, high multiplier | Instant boosts | Points land before the block resolves |
| Long rounds, high multiplier | Power Boosts (early) | Per-second points compound over duration |
| Long rounds | Echo Boosts | Reward scales with time elapsed |
| Round of unknown length, want safety | Focus Boosts | 5-minute validity covers typical block intervals |
| Coordinating with Clan | Clan Power-up | Effect grows with each member activation |
| Daily streak play | Miner Service | Stacks toward 3% maintenance discount (free, daily cooldown) |
| Amplifying a single big cast | Copy Boost | Copies % of the next boost; order before target |

> Spell values change per Cycle. Always check current in-game values before relying on the table above for optimization.

---

## Spell Bot

For a full step-by-step setup walkthrough, see **[How-to: Set Up Spell Bot](INSTRUCTION-SPELL-BOT.md)**. Quick reference below.

### Is Spell Bot safe to use? Will I get banned?

**Spell Bot is completely safe to use.** It's an official GoMining feature, not a third-party tool — you won't get banned for using it. Manual casting still works while the bot is active, so you can layer extra spells on top during key rounds.

### How it works (concept)

* You create **Setups** — each Setup binds a group of spells to **one multiplier** (x1, x2, x4, x8, x16, x32, x64, x128, x256)
* When a round with a matching multiplier starts, the bot casts that Setup's spells in the order you specified
* If the budget runs low mid-round, the bot casts top-to-bottom and skips lower-priority spells

### Budget

Spell Bot uses its own budget, **separate from your main wallet** — you transfer GMT in (and back out) via the Spell Bot UI.

> **Empty budget disables every Setup**, not just the active one.

### Cost notes

* **Power-up** and **Clan Power-up** costs **scale with PPS** — Setup TOTAL can shift between rounds even without edits. The UI flags these with a **yellow icon**.
* **Miner Service** is free with a daily cooldown — cast manually, don't add it to a Setup.
* You can't add the same spell twice — use the quantity buttons (− / +) instead.

### Does Platinum+ work with Spell Bot?

Yes. With Platinum+, every spell the bot casts is **15% cheaper**. Heavy bot users typically save more than the subscription cost. The 15% discount **does not stack** with GoMiners Avatar discounts — the highest applies.
