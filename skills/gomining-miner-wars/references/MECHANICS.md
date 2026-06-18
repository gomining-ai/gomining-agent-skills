# Game Mechanics

## How Points Work

The main goal in each round is to accumulate points. Each player's score grows automatically every second based on the total power of their miners and their average energy efficiency. The Clan Score is the sum of all members' personal scores.

**Two factors affect your points in a round:**

1. Your Points-per-second rate (PPS)
2. Spells and Power-ups — paid effects that increase your PPS or add points directly

---

## What is the Points-per-second Rate (PPS)?

Your PPS rate shows how fast your score grows during a round. It is based on your total mining power (TH) and average energy efficiency.

```
PPS = user TH × (base EE / user EE)
```

Where:
* `user TH` — total power of all your miners (in terahashes)
* `base EE` — a constant currently set at **28 W/TH** (subject to change)
* `user EE` — your miners' average energy efficiency

**Example:** If your total power is 1 TH and your average energy efficiency is 20 W/TH, your base PPS would be:

```
1 × (28 / 20) = 1.4 points/sec
```

A miner with *better* (lower) energy efficiency than the base produces **more** points per TH than one at base EE.

---

## How do Leagues Work?

All gameplay takes place in Leagues — competitive groups where Clans battle for rewards.

There are **4 Leagues**:

| League  | Clan Slots | Description                                    |
| ------- | ---------- | ---------------------------------------------- |
| Odyssey | 50         | Top League with the highest reward multipliers |
| Eclipse | 50         | Competitive mid-tier League                    |
| Horizon | 50         | League with growth potential                   |
| Dune    | Dynamic    | Entry-level League                             |

---

## How Promotion and Demotion Work

At the end of each weekly Cycle, Clans are promoted or demoted based on:

1. Number of blocks mined
2. Total computing power (TH) — used as a tiebreaker

**5 Clans move up or down** each Cycle between Odyssey, Eclipse, and Horizon.

Dune divisions are reshuffled every Cycle for fairness.

---

## What is a Round?

Rounds are the core gameplay unit. Each round starts and ends based on real Bitcoin blockchain activity — when a new block is confirmed on the Bitcoin network.

* Round duration varies, since real Bitcoin blocks are mined at irregular intervals
* Players participate in an estimated **120–150 rounds per day**
* A new round starts instantly after the previous one ends

---

## Round Multipliers

Each round is assigned a multiplier based on how many Bitcoin blocks are mined simultaneously. The multiplier boosts the weight of that round's rewards — up to **x256**.

The range of available multipliers depends on the League:

| Dune      | Horizon   | Eclipse    | Odyssey    |
| --------- | --------- | ---------- | ---------- |
| x1 – x32  | x1 – x64  | x1 – x128  | x1 – x256  |

Winning a round with a higher multiplier counts as winning that many regular rounds. For example, winning a round with x32 counts as 32 round wins.

---

## Cycle Timing

| Aspect | Detail |
|--------|--------|
| Cycle length | 7 days |
| Cycle start | Tuesday 00:00 UTC |
| Cycle end | Next Tuesday 00:00 UTC |
| Reward distribution | At Cycle end, automatically |
