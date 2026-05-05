# Burn and Mint

This document covers the GMT Burn & Mint deflationary mechanism, epoch structure, re-minting coefficient, post-mint distribution, and the long-term supply reduction strategy.

---

## Table of Contents

1. [Overview](#overview)
2. [How Burn & Mint Works](#how-burn--mint-works)
3. [Epochs and Cycles](#epochs-and-cycles)
4. [Re-minting Coefficient](#re-minting-coefficient)
5. [Post-Mint Distribution](#post-mint-distribution)
6. [Supply Reduction Strategy](#supply-reduction-strategy)
7. [Worked Example](#worked-example)
8. [FAQ](#faq)

---

## Overview

The Burn & Mint system is the core deflationary mechanism of the GoMining tokenomics model. Tokens are burned daily from user spending (service fees and electricity costs), then a portion is re-minted based on a community-governed coefficient. The difference between burned and minted tokens represents permanent supply reduction.

### Key Principle

```
Tokens Burned  -  Tokens Minted  =  Tokens Permanently Destroyed
```

This system works toward the long-term goal of reducing total GMT supply from 500M to 100M tokens.

---

## How Burn & Mint Works

### Step-by-Step Flow

| Step | Action | Description |
|------|--------|-------------|
| 1 | **User spending** | Users pay service fees and electricity costs in GMT |
| 2 | **Daily burn** | Spent tokens are burned (removed from circulation) |
| 3 | **Apply coefficient** | Burned amount is multiplied by the re-minting coefficient |
| 4 | **Mint new tokens** | Result from step 3 is minted as new tokens |
| 5 | **Distribute** | Minted tokens are distributed according to post-mint rules |
| 6 | **Net reduction** | Difference between burned and minted is permanently destroyed |

### Sources of Burned Tokens

Tokens enter the burn pool from two primary sources:

| Source | Description |
|--------|-------------|
| **Service fees** | Fees paid by users for platform services |
| **Electricity costs** | Mining electricity expenses paid in GMT |

All user spending in GMT contributes to the daily burn, creating a direct link between platform usage and the deflationary mechanism.

---

## Epochs and Cycles

The Burn & Mint system operates in epochs, each consisting of weekly cycles.

### Current Status

| Parameter | Value |
|-----------|-------|
| **Current epoch** | Epoch 5 |
| **Cycle duration** | 1 week |
| **Cycle boundaries** | Tuesday to Tuesday |

### Epoch Structure

Each epoch defines the operating parameters for the Burn & Mint system over a set of weekly cycles. The epoch number advances as the system evolves and parameters are adjusted.

### Weekly Cycle Timeline

| Day | Activity |
|-----|----------|
| **Tuesday** | New cycle begins; previous cycle's mint is distributed |
| **Tuesday - Monday** | Daily burns accumulate throughout the week |
| **Monday** | Cycle closes; total burn calculated |
| **Tuesday** | Re-minting coefficient applied; new tokens minted and distributed |

---

## Re-minting Coefficient

The re-minting coefficient is the multiplier applied to burned tokens to determine how many new tokens are minted. It is governed by community voting (see [LOCK-AND-VOTE.md](LOCK-AND-VOTE.md) for voting details).

### Coefficient Properties

| Property | Details |
|----------|---------|
| **Range** | 0 to 1 |
| **Set by** | VE token holder voting (Voting System #2) |
| **Applied** | At the end of each weekly cycle |

### Coefficient Impact

| Coefficient | Burned | Minted | Net Destroyed | Burn Effectiveness |
|-------------|--------|--------|---------------|-------------------|
| **0.00** | 100,000 | 0 | 100,000 | Maximum burn |
| **0.25** | 100,000 | 25,000 | 75,000 | High burn |
| **0.50** | 100,000 | 50,000 | 50,000 | Balanced |
| **0.75** | 100,000 | 75,000 | 25,000 | Low burn |
| **0.98** | 100,000 | 98,000 | 2,000 | Minimal burn |
| **1.00** | 100,000 | 100,000 | 0 | No net burn |

### Trade-off

- **Lower coefficient**: Faster supply reduction, but fewer tokens distributed to participants.
- **Higher coefficient**: More tokens flow to stakers and service providers, but slower supply reduction.

The community continuously balances these competing interests through the voting mechanism.

---

## Post-Mint Distribution

After tokens are minted each cycle, they are distributed according to fixed allocation rules.

### Distribution Breakdown

Minted tokens are distributed across four categories: platform operations, users with locked tokens, product redistribution (governed by community voting), and core operations. The exact percentages are governed by the tokenomics model and can be viewed in the **Governance** section of the GoMining app.

### Product Redistribution

The product redistribution share is split across five categories according to the weekly reward distribution vote (Voting System #1):

- Game rewards
- Solo miners discount
- Greedy Machines holders
- Liquidity leaderboard
- Bank Bounty

The current split for each category is determined by VE token holder votes and is visible in the GoMining app.

---

## Supply Reduction Strategy

### Long-term Target

| Metric | Value |
|--------|-------|
| **Initial supply** | 500,000,000 GMT |
| **Target supply** | 100,000,000 GMT |
| **Reduction target** | 400,000,000 GMT (80% reduction) |

### Two-Vector Approach

The strategy uses two parallel vectors to achieve the 100M target:

**Vector 1 - Gradual Token Reduction**
- Systematic burns through the Burn & Mint mechanism.
- Each weekly cycle permanently removes tokens when the coefficient is below 1.
- Cumulative effect compounds over time.

**Vector 2 - Increase Token Utility**
- Expand use cases for GMT to drive demand.
- Current utility: electricity discounts, game boosts, hashrate reinvestment, voting bonuses.
- Higher utility increases spending, which increases burns, accelerating supply reduction.

### Current Locked Supply Impact

With approximately 140M tokens (34%) locked, the effective circulating supply is already significantly reduced. Combined with ongoing burns, the path to 100M total supply is supported by both demand-side (locking) and supply-side (burning) mechanisms.

---

## Worked Example

The following example illustrates a single weekly cycle using real-world approximate figures.

### Scenario

| Parameter | Value |
|-----------|-------|
| **Total burned in week** | 248,000 GMT |
| **Re-minting coefficient** | ~0.984 |
| **Total minted** | 244,000 GMT |
| **Net destroyed** | 4,000 GMT |

### Step-by-Step Calculation

**Step 1: Burn**
Users spend 248,000 GMT on service fees and electricity during the week. All 248,000 tokens are burned.

**Step 2: Apply Coefficient**
```
248,000  x  0.984  =  244,032 (approximately 244,000)
```

**Step 3: Mint and Distribute**

244,000 tokens are distributed across platform operations, locked token holders, product redistribution, and core operations according to the tokenomics model.

**Step 4: Net Effect**
```
248,000 burned  -  244,000 minted  =  4,000 GMT permanently destroyed
```

This 4,000 GMT is removed from the total supply forever, contributing to the long-term 500M to 100M reduction goal.

---

## FAQ

### Burn Mechanics

**Q: Where do the burned tokens come from?**
A: Burned tokens come from user spending within the GoMining platform, specifically service fees and electricity costs paid in GMT.

**Q: Are tokens burned immediately when spent?**
A: Tokens are burned on a daily basis. User spending accumulates and is processed in daily burn batches.

**Q: Can burned tokens ever be recovered?**
A: The net destroyed tokens (burned minus minted) are permanently removed from the total supply and cannot be recovered.

### Re-minting

**Q: Who decides the re-minting coefficient?**
A: VE token holders vote on the coefficient through Voting System #2. The community collectively sets the value between 0 and 1.

**Q: How often does the coefficient change?**
A: The coefficient can change every weekly cycle based on the ongoing community vote.

**Q: What happens if the coefficient is set to 0?**
A: All burned tokens would be permanently destroyed with no re-minting. This would maximize the burn rate but eliminate all post-mint distributions.

### Distribution

**Q: How do I receive post-mint rewards?**
A: You need to lock GMT tokens to receive VE tokens. Locked token holders receive 20% of all minted tokens, distributed proportionally to VE balances.

**Q: What is the product redistribution share used for?**
A: The 10% product redistribution is split across five categories (game rewards, solo miners discount, Greedy Machines holders, liquidity leaderboard, Bank Bounty) based on the weekly reward distribution vote.

### Epochs

**Q: What is the current epoch?**
A: The system is currently in Epoch 5.

**Q: When do weekly cycles start and end?**
A: Each cycle runs from Tuesday to Tuesday.

**Q: What changes between epochs?**
A: Epochs represent major phases of the Burn & Mint system. Parameters and mechanics may be adjusted between epochs as the system evolves toward the long-term supply target.

### Supply Goals

**Q: How long will it take to reach 100M supply?**
A: The timeline depends on the re-minting coefficient (governed by community voting) and overall platform usage (which drives burns). There is no fixed date; it is a gradual, community-governed process.

**Q: What happens when the supply reaches 100M?**
A: The long-term target of 100M tokens represents the desired equilibrium. Governance decisions at that point will determine whether burns continue, stabilize, or the mechanism is adjusted.
