# Yield Mechanics — GoMining Simple Earn

## Overview

Simple Earn generates yield from multiple sources and distributes it to participants via a snapshot-based daily cycle. All rewards are paid in BTC, regardless of the deposited asset. Interest is not guaranteed and may be zero in any given period.

---

## Dividend Payouts

| Parameter | Value |
|-----------|-------|
| Payout currency | **BTC** |
| Payout frequency | **Every 4 hours** (6 times per day) |
| Compounding | Auto-compounds every 4-hour cycle |
| Guarantee | Interest is **NOT** guaranteed; yield can be zero |
| Capital safety | Not absolutely guaranteed — DeFi protocol risks apply (smart contract vulnerabilities). GoMining actively monitors and rebalances to reduce risk. |

---

## APR and Estimated Yield

| Concept | Description |
|---------|-------------|
| Individual APR | Each supported asset (BTC, ETH, SOL, BNB, TON, USDT, USDC) has its own APR |
| APR setter | GoMining's liquidity manager sets and adjusts APR per asset |
| VIP multiplier | Your VIP level applies a multiplier to your APR (Bronze I: base rate; Elite: x1.46) |
| Estimated yield | Weighted average APR across all assets in user's Simple Earn balance |
| Variability | APR can change over time based on market conditions and yield sources |

### Estimated Yield Calculation

The estimated yield shown to users is a **weighted average** across all deposited assets:

```
Estimated Yield = Σ (Asset Balance × Asset APR) / Σ (Asset Balance)
```

For example, if a user has:
- 0.1 BTC at 3% APR
- 1,000 USDT at 5% APR

The estimated yield reflects the weighted combination of both positions.

---

## 4-Hour Reward Cycle

Simple Earn uses a **4-hour cycle** to calculate and distribute rewards. Cycles repeat 6 times per day.

### Cycle Schedule

| Cycle Start (UTC) | Reward Credited |
|-------------------|----------------|
| 00:00 | End of 00:00–04:00 cycle |
| 04:00 | End of 04:00–08:00 cycle |
| 08:00 | End of 08:00–12:00 cycle |
| 12:00 | End of 12:00–16:00 cycle |
| 16:00 | End of 16:00–20:00 cycle |
| 20:00 | End of 20:00–00:00 cycle |

### Cycle Rules

| Rule | Details |
|------|---------|
| Reward basis | **Minimum balance** held during the full 4-hour cycle |
| New deposits | Counted from the **start of the next cycle** |
| Withdrawals | Reduce the minimum balance; rewards calculated on the lowest amount held |
| Reward currency | BTC — credited directly to wallet after each cycle |

### Timing Examples

| Scenario | Deposit Time | First Eligible Cycle | First Reward |
|----------|-------------|---------------------|--------------|
| Deposit at 01:30 UTC | 01:30 UTC | 04:00–08:00 cycle | ~08:00 UTC |
| Deposit at 07:50 UTC | 07:50 UTC | 08:00–12:00 cycle | ~12:00 UTC |
| Deposit at 23:45 UTC | 23:45 UTC | 00:00–04:00 cycle (next day) | ~04:00 UTC |

> **Tip:** Deposits take effect at the start of the next cycle — timing within a cycle does not matter.

---

## Yield Sources

Simple Earn yield is generated from three primary sources:

### 1. Staking (Blockchain Validation)

| Aspect | Details |
|--------|---------|
| Method | Proof-of-Stake blockchain validation |
| Mechanism | Deposited assets are staked to earn validation rewards |
| Risk | Low — established blockchain networks |

### 2. DeFi Protocols

| Aspect | Details |
|--------|---------|
| Liquidity Pools | Assets deployed to decentralized exchange liquidity pools |
| Lending | Assets lent through DeFi lending platforms |
| Yield type | Variable — depends on protocol activity and market conditions |

### 3. Internal Liquidity Management

| Aspect | Details |
|--------|---------|
| Method | GoMining's proprietary liquidity management operations |
| Control | Managed by GoMining's liquidity team |
| Optimization | Dynamically allocated across opportunities |

---

## Auto-Compounding

| Parameter | Details |
|-----------|---------|
| Mechanism | Rewards are automatically reinvested |
| Frequency | Every 4-hour cycle |
| User action required | None — compounding is automatic |
| Effect | BTC rewards are added to balance, increasing the minimum for subsequent cycles |

### Compounding Flow

```
Cycle 1 ends → BTC reward credited
         ↓
Cycle 2 starts (balance now includes Cycle 1 rewards)
         ↓
Cycle 2 ends → larger BTC reward credited
         ↓
... continues automatically, 6 times per day
```

---

## Frequently Asked Questions

### Why is my yield zero?

Interest is not guaranteed. Yield can be zero in any given period depending on market conditions and yield source performance. Your principal is always protected.

### Why does APR differ between assets?

Each asset has unique staking, DeFi, and liquidity opportunities. GoMining's liquidity manager sets individual APR for each asset based on available yields in the market.

### When does my deposit start earning?

Your deposit is counted from the start of the next 4-hour cycle after it is made. Rewards are credited at the end of that cycle (every 4 hours: 04:00, 08:00, 12:00, 16:00, 20:00, 00:00 UTC).

### Is the APR fixed?

No. APR is variable and can change over time as market conditions and yield source performance fluctuate. GoMining's liquidity manager adjusts rates accordingly. Your VIP level also affects your effective APR via a multiplier.

### How does auto-compounding work?

BTC rewards are credited every 4 hours and automatically added to your Simple Earn balance. This larger balance then serves as the basis for the next cycle's reward calculation, compounding your returns without any manual action.

### What happens to my rewards if I withdraw?

There are no penalties for withdrawal. Any rewards already credited to your balance are yours to keep. If you withdraw during a cycle, the reward for that cycle is calculated based on the lowest balance held — so partial withdrawals mid-cycle reduce that cycle's reward proportionally.
