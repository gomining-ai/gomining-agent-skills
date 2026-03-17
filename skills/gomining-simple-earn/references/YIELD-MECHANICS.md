# Yield Mechanics — GoMining Simple Earn

## Overview

Simple Earn generates yield from multiple sources and distributes it to participants via a snapshot-based daily cycle. All rewards are paid in BTC, regardless of the deposited asset. Interest is not guaranteed and may be zero in any given period.

---

## Dividend Payouts

| Parameter | Value |
|-----------|-------|
| Payout currency | **BTC** |
| Payout frequency | Daily |
| Compounding | Auto-compounds at fixed intervals |
| Guarantee | Interest is **NOT** guaranteed |
| Minimum yield | Can be zero |
| Principal loss | Never — deposits are principal-protected |

---

## APR and Estimated Yield

| Concept | Description |
|---------|-------------|
| Individual APR | Each supported asset (BTC, USDT, USDC) has its own APR |
| APR setter | GoMining's liquidity manager sets and adjusts APR per asset |
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

## Snapshot System

Simple Earn uses a **snapshot-based** daily cycle to determine reward distribution.

### Daily Timeline

| Time (UTC) | Event | Description |
|------------|-------|-------------|
| 23:59 | **Snapshot** | System captures all Simple Earn balances |
| 00:00–06:59 | Processing | Rewards calculated based on snapshot data |
| 07:00 (T+1) | **Reward Credit** | BTC dividends credited to user balances |

### Snapshot Rules

| Rule | Details |
|------|---------|
| Participation | Only balances present at snapshot time (23:59 UTC) participate |
| Late deposits | Deposits made after 23:59 UTC do **not** count for that day |
| Early withdrawals | Funds withdrawn before 23:59 UTC are excluded from snapshot |
| Next-day inclusion | New deposits are included starting from the next 23:59 UTC snapshot |

### Timing Examples

| Scenario | Deposit Time | First Eligible Snapshot | First Reward Credit |
|----------|-------------|------------------------|---------------------|
| Deposit at 10:00 UTC, Day 1 | 10:00 UTC, Day 1 | 23:59 UTC, Day 1 | 07:00 UTC, Day 2 |
| Deposit at 23:30 UTC, Day 1 | 23:30 UTC, Day 1 | 23:59 UTC, Day 1 | 07:00 UTC, Day 2 |
| Deposit at 00:15 UTC, Day 2 | 00:15 UTC, Day 2 | 23:59 UTC, Day 2 | 07:00 UTC, Day 3 |

> **Tip:** To maximize earning, deposit well before 23:59 UTC to ensure inclusion in that day's snapshot.

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
| Frequency | Fixed intervals (daily cycle) |
| User action required | None — compounding is automatic |
| Effect | BTC rewards are added to balance, increasing next snapshot amount |

### Compounding Flow

```
Day 1 Snapshot → Day 2 Reward Credit (BTC)
         ↓
Day 2 Snapshot (original balance + Day 2 rewards)
         ↓
Day 3 Reward Credit (based on larger balance)
         ↓
... continues automatically
```

---

## Frequently Asked Questions

### Why is my yield zero?

Interest is not guaranteed. Yield can be zero in any given period depending on market conditions and yield source performance. Your principal is always protected.

### Why does APR differ between assets?

Each asset has unique staking, DeFi, and liquidity opportunities. GoMining's liquidity manager sets individual APR for each asset based on available yields in the market.

### When does my deposit start earning?

Your deposit starts earning from the first snapshot it is included in. If you deposit before 23:59 UTC, it will be captured in that day's snapshot, and you will receive rewards at 07:00 UTC the following day.

### Is the APR fixed?

No. APR is variable and can change over time as market conditions and yield source performance fluctuate. GoMining's liquidity manager adjusts rates accordingly.

### How does auto-compounding work?

BTC rewards credited at 07:00 UTC are automatically added to your Simple Earn balance. This larger balance is then captured in the next 23:59 UTC snapshot, effectively compounding your returns without any manual action.

### What happens to my rewards if I withdraw?

There are no penalties for withdrawal. Any rewards already credited to your balance are yours to keep. Withdrawing before the 23:59 UTC snapshot means that balance will not participate in that day's reward cycle.
