# How-to: Set Up Spell Bot

**Spell Bot** is an official GoMining feature that auto-casts your chosen spells at the start of every round with a matching multiplier. It's useful when you can't be online for all 120–150 rounds per day, or when you want to reserve specific spell combos for specific multipliers.

Manual spell casting still works while the bot is active — you can layer extra spells on top during key rounds.

---

## Step 1: Open Spell Bot

Two access paths:

* **From the Spells menu** — open **Spells**, then tap **Spell Bot**
* **From the Main Screen** — tap the **Spell Bot** indicator above your score

The first time you open it, you'll see an empty state with **NO SETUPS YET** and a budget of 0.00.

---

## Step 2: Top Up the Budget

Spell Bot uses its **own budget**, separate from your main wallet. To enable auto-casting, move GOMINING tokens into the Spell Bot budget first.

1. Tap **+** on the **SPELL BOT BUDGET** card
2. In the **TRANSFER TOKENS** dialog, enter an amount or use the quick buttons (**1**, **10**, **100**, **500**, **ALL**)
3. Tap **TRANSFER**

You can move tokens back to your main wallet at any time using the same dialog (toggle direction with the arrow icon). If your wallet is empty, tap **BUY GOMINING** to top it up.

> **Empty budget = all Setups disabled.** It's not just the active one — every Setup turns off until you top up.

---

## Step 3: Create a Setup

A **Setup** is a group of spells tied to **one multiplier**. Each multiplier (x1, x2, x4, x8, x16, x32, x64, x128, x256) can have its own Setup, so you can run a low-cost mix on x1 rounds and a heavier combo on x32+.

1. Tap **CREATE SETUP** (or **+ NEW SETUP** if you already have one)
2. Under **MULTIPLIER**, pick the multiplier this Setup applies to

The available multipliers depend on your League (see [MECHANICS.md](MECHANICS.md) round multipliers section).

---

## Step 4: Add Spells

1. Tap **+ ADD SPELL**
2. Check every spell you want to include. You can pick from any category — Power-up, Clan Power-up, Miner Service, Instant / Power / Echo / Focus / Copy boosts (regular, Super, Ultra)
3. Tap **ADD**
4. For each added spell, use the **−** and **+** buttons to set how many times the bot should cast it per round

The **TOTAL** field at the bottom shows the GOMINING cost per round for the current Setup. This is what the bot deducts from your budget every time the Setup runs.

> **Power-up and Clan Power-up costs scale with PPS.** TOTAL can shift between rounds even if you don't change anything — adding TH or upgrading energy efficiency increases the price. The bot flags these spells with a **yellow icon** as a reminder.

You can't add the same spell twice — use the **+** button to increase its quantity instead.

---

## Step 5: Order Spells by Priority

If your budget runs low mid-round, the bot casts spells **in the order they appear in your Setup**, top to bottom, until tokens run out. Spells lower in the list may be skipped.

Drag the handle on the right side of each spell row to reorder. **Put the most important spells at the top.**

---

## Step 6: Save and Manage Setups

Tap **SAVE**. The Setup appears in the main Spell Bot screen as a row showing:

| UI Element | Purpose |
|------------|---------|
| Multiplier badge | x1, x2, …, x256 |
| Spell icons | Everything in the Setup |
| Cost per use | In GOMINING |
| Toggle | Enable / disable without deleting |
| Gear icon | Edit the Setup |
| Trash icon | Delete it |

Toggle individual Setups on or off any time. When a multiplier with an active Setup starts, the bot automatically casts the saved spells.

---

## Tips

### Budget Management

* **Estimate weekly spend** — multiply each Setup's cost per round by how often that multiplier appears (most rounds are x1; average across the Cycle is ~x2). Add a buffer for Power-up cost growth as your PPS climbs.
* **Top up before Tuesday 00:00 UTC** — a new Cycle usually means a fresh strategy; start the week with a full budget.
* **Empty budget disables every Setup**, not just the active one.

### Match Setup Strength to Multiplier

Higher multipliers count as more round wins (a x128 win = 128 round wins), so concentrate spending where it pays off most:

| Multiplier | Strategy |
|------------|----------|
| **x1 – x4** | Keep it cheap. A single Power Boost or Instant Boost is often enough. |
| **x8 – x32** | Mid-tier. Add Super boosts; consider Power-up if your PPS is solid. |
| **x64+** | Go heavy. Stack Ultra boosts, Power-up, and Clan Power-up for maximum impact. |

> **Miner Service** has a daily cooldown and is free — cast it manually once per day rather than adding it to a Spell Bot Setup.

### Pick Spell Types by Round Behavior

| Spell Type | When It Shines |
|------------|----------------|
| **Echo boosts** | Grow over time, ticks every 2 minutes — good when rounds tend to run long |
| **Focus boosts** | Only pay out if round ends within 5 minutes — skip if your League's rounds run long |
| **Instant boosts** | Safe default — independent of round length |
| **Power boosts** | Safe default — per-second value compounds with round length |
| **Copy boosts** | Copy a % of the next boost — place **earlier** in the order than the boost they should copy |

### Stack with Platinum+

With a Platinum+ subscription, every spell the bot casts is **15% cheaper**. Heavy bot users typically save more than the subscription cost.

### Mix Manual and Automated Casting

The bot handles your baseline; manual casts handle the spikes. When you spot a high-multiplier round (x64+), manually fire an Ultra Power-up or extra Clan Power-up activation on top of what the bot already casts.

### Test Before Scaling Up

Build a low-cost Setup for x1 rounds first to confirm the bot is firing as expected, then duplicate and scale the Setup for higher multipliers.

---

## Cross-references

* [Spells & Power-ups](SPELLS.md) — full spell catalog and effects
* [Mechanics](MECHANICS.md) — multiplier ranges per League
* [Cross-skill Effects](CROSS-SKILL-EFFECTS.md) — Platinum+ stacking rules with Avatar discounts
