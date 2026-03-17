# Lock and Vote

This document covers the GMT token locking mechanism, veGOMINING (VE) tokens, and the two voting systems that enable community governance within the GoMining ecosystem.

---

## Table of Contents

1. [Locking Mechanism](#locking-mechanism)
2. [veGOMINING (VE) Tokens](#vegomining-ve-tokens)
3. [Voting System #1 - Weekly Reward Distribution](#voting-system-1---weekly-reward-distribution)
4. [Voting System #2 - Re-minting Coefficient](#voting-system-2---re-minting-coefficient)
5. [Virtual vs Blockchain Locking](#virtual-vs-blockchain-locking)
6. [FAQ](#faq)

---

## Locking Mechanism

### How It Works

Users lock their GMT tokens for a chosen duration to receive vote-escrowed GoMining (VE) tokens. This mechanism serves two purposes: it grants governance power through voting and it provides price stability by reducing circulating supply.

### Lock Flow

```
User locks GMT  -->  Receives VE tokens  -->  VE grants voting power
                                          -->  VE decreases over time as lock period ends
```

### Key Parameters

| Parameter | Details |
|-----------|---------|
| **Input** | GMT tokens |
| **Output** | VE (vote-escrowed) tokens |
| **VE quantity depends on** | Lock amount and lock duration |
| **VE behavior over time** | Decreases linearly as the lock period approaches expiry |
| **Current locked supply** | ~140M tokens (~34% of total supply) |
| **Primary benefit** | Voting power, token bonuses, and price stability |

### Why Locking Matters

- **Price stability**: With ~34% of tokens locked, a significant portion of the supply is removed from circulation, reducing sell pressure.
- **Governance participation**: Only VE token holders can participate in voting.
- **Bonus rewards**: Locked-token holders receive a share of post-mint distribution (20% of all newly minted tokens).
- **Alignment of incentives**: Longer lock periods yield more VE tokens, aligning holder interests with long-term protocol health.

---

## veGOMINING (VE) Tokens

### Overview

VE tokens are non-transferable governance tokens received in exchange for locking GMT. They represent a user's voting power and commitment to the ecosystem.

### VE Token Properties

| Property | Description |
|----------|-------------|
| **Transferable** | No |
| **Source** | Locking GMT tokens |
| **Determines** | Voting power in both voting systems |
| **Decay** | Linear decrease as lock expiry approaches |
| **Smart contract** | VEGoMining contract |

### VE Calculation

The number of VE tokens received depends on two factors:

1. **Lock amount**: More GMT locked results in more VE tokens.
2. **Lock duration**: Longer lock periods produce more VE tokens for the same GMT amount.

As the lock period progresses toward expiry, VE tokens decrease linearly. At the moment of unlock, VE balance reaches zero and the user can withdraw their original GMT.

### VE Token Lifecycle

| Stage | VE Balance | Action |
|-------|-----------|--------|
| **Lock start** | Maximum (based on amount and duration) | GMT locked, VE issued |
| **Mid-lock** | Decreasing linearly | Voting power reduces over time |
| **Lock expiry** | Zero | User can withdraw GMT |

---

## Voting System #1 - Weekly Reward Distribution

### Purpose

VE token holders vote on how weekly rewards are distributed across different product categories in the GoMining ecosystem.

### Current Distribution

| Category | Allocation | Description |
|----------|-----------|-------------|
| **Game rewards** | 39.8% | Rewards for game participation |
| **Solo miners discount** | 26.8% | Discount for solo mining operations |
| **Greedy Machines holders** | 18.9% | Rewards for Greedy Machines NFT holders |
| **Liquidity leaderboard** | 7.4% | Incentives for liquidity providers |
| **Bank Bounty** | 6.9% | Bank Bounty pool rewards |

### How Voting Works

1. Users hold VE tokens from locking GMT.
2. During voting periods, VE holders allocate their voting power across the categories above.
3. The aggregate vote determines the percentage split for the upcoming reward cycle.
4. Voting power is proportional to VE token balance at the time of the vote.

### Voting Impact

- Higher allocation to a category means more rewards flow to participants of that category.
- Community members tend to vote in favor of categories where they are most active.
- The distribution shifts over time as community priorities evolve.

---

## Voting System #2 - Re-minting Coefficient

### Purpose

VE token holders also vote on the re-minting coefficient, which directly controls the burn rate of GMT tokens. This is a key lever for the deflationary supply reduction strategy.

### How It Works

| Parameter | Details |
|-----------|---------|
| **Coefficient range** | 0 to 1 |
| **Higher coefficient** | More tokens re-minted, lower effective burn rate |
| **Lower coefficient** | Fewer tokens re-minted, higher effective burn rate |
| **Voter influence** | VE holders set the coefficient through voting |

### Relationship to Burn & Mint

The re-minting coefficient directly feeds into the Burn & Mint system:

```
Tokens burned daily  x  Re-minting coefficient  =  Tokens minted back
```

- A coefficient of 1.0 means all burned tokens are re-minted (zero net burn).
- A coefficient of 0.0 means no tokens are re-minted (maximum burn).
- The community balances between rewarding participants (higher coefficient) and reducing supply (lower coefficient).

For full details on the Burn & Mint system, see [BURN-AND-MINT.md](BURN-AND-MINT.md).

---

## Virtual vs Blockchain Locking

GoMining supports two methods of locking tokens:

| Feature | Blockchain Locking | Virtual Locking |
|---------|-------------------|-----------------|
| **Storage** | On-chain smart contracts | Backend servers |
| **Speed** | Standard blockchain transaction time | Fast (2 clicks) |
| **VE issuance** | On-chain VE contract | Backend-tracked, synced to contracts |
| **User experience** | Requires wallet interaction | Streamlined in-app flow |
| **Sync** | Native on-chain | Periodically synced to on-chain contracts |

Virtual locking was introduced to lower the barrier to entry. Users can lock tokens quickly through the app interface, and the state is synchronized to on-chain contracts to maintain data integrity.

---

## FAQ

### General

**Q: What happens to my GMT when I lock them?**
A: Your GMT tokens are held in the VEGoMining smart contract (or tracked on the backend for virtual locks). You receive VE tokens in return. When the lock period ends, your VE balance reaches zero and you can withdraw your original GMT.

**Q: Can I unlock my GMT early?**
A: Lock periods are fixed. Tokens remain locked until the chosen duration expires. Plan your lock duration carefully.

**Q: Are VE tokens transferable?**
A: No. VE tokens are non-transferable and bound to the account that locked the GMT.

### Voting

**Q: How often does voting occur?**
A: Voting follows the weekly cycle aligned with the Burn & Mint epochs (Tuesday to Tuesday).

**Q: What if I do not vote?**
A: Your VE tokens remain but you forfeit your governance influence for that cycle. There is no penalty, but you miss the opportunity to shape reward distribution and the burn rate.

**Q: Can I vote in both voting systems simultaneously?**
A: Yes. VE holders can participate in both the weekly reward distribution vote and the re-minting coefficient vote during the same period.

### Locking Strategy

**Q: Should I lock for a longer or shorter period?**
A: Longer locks yield more VE tokens and therefore more voting power and locked-token bonuses. However, your GMT is inaccessible for the full duration. Consider your liquidity needs.

**Q: What percentage of GMT supply is currently locked?**
A: Approximately 140M tokens, representing about 34% of the total supply.

**Q: Does locking earn me direct token rewards?**
A: Yes. 20% of all post-mint tokens are distributed to users with locked tokens. Additionally, VE holders benefit from governance influence and potential bonus mechanisms.
