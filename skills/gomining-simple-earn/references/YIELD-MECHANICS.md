# Yield Mechanics — GoMining Simple Earn

## Overview

Simple Earn generates yield from multiple sources and distributes it to participants on a 4-hour reward cycle. All rewards are paid in BTC, regardless of the deposited asset. Interest is not guaranteed and may be zero in any given period.

---

## Dividend Payouts

| Parameter | Value |
|-----------|-------|
| Payout currency | **BTC** |
| Payout frequency | Every 4 hours (6 cycles per day) |
| Compounding | Auto-compounds each cycle |
| Guarantee | Interest is **NOT** guaranteed |
| Minimum yield | Can be zero |
| Principal loss | Possible in rare cases (e.g. a smart-contract vulnerability) - Simple Earn is not a bank deposit, so capital preservation cannot be guaranteed |

---

## APR and Estimated Yield

| Concept | Description |
|---------|-------------|
| Individual APR | Each supported asset has its own APR |
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

## Reward Cycle (Every 4 Hours)

Simple Earn distributes rewards on a **4-hour cycle**. Cycles start at 00:00 UTC and repeat every 4 hours (00:00 → 04:00 → 08:00 → 12:00 → 16:00 → 20:00), giving 6 cycles per day.

### Cycle Schedule

| Cycle Start (UTC) | Reward Credited |
|-------------------|----------------|
| 00:00 | End of 00:00–04:00 cycle |
| 04:00 | End of 04:00–08:00 cycle |
| 08:00 | End of 08:00–12:00 cycle |
| 12:00 | End of 12:00–16:00 cycle |
| 16:00 | End of 16:00–20:00 cycle |
| 20:00 | End of 20:00–00:00 cycle |

### How a Cycle Works

| Aspect | Details |
|--------|---------|
| Cycle length | 4 hours |
| Reward basis | The **minimum balance** held during the full 4-hour cycle |
| Payout | BTC, calculated and credited for every full cycle you've participated in |
| Balance decreases | A withdrawal, purchase, or other operation that lowers your balance mid-cycle means rewards use the lowest amount held during that cycle |
| New deposits | Counted from the **start of the next** 4-hour cycle |

### Timing Examples

| Scenario | Deposit Time | First Full Cycle Counted |
|----------|-------------|--------------------------|
| Deposit at 10:00 UTC | 10:00 UTC | 12:00–16:00 UTC cycle |
| Deposit at 03:30 UTC | 03:30 UTC | 04:00–08:00 UTC cycle |
| Deposit at 16:10 UTC | 16:10 UTC | 20:00–00:00 UTC cycle |

> **Note:** To earn for a given cycle, your balance must be held for the full 4-hour cycle. Funds deposited mid-cycle start earning from the next cycle.

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
| Frequency | Each 4-hour cycle |
| User action required | None — compounding is automatic |
| Effect | BTC rewards are added to balance, increasing the amount earning in the next cycle |

### Compounding Flow

```
Cycle 1 → BTC reward credited
         ↓
Cycle 2 earns on (original balance + Cycle 1 rewards)
         ↓
Cycle 3 earns on the larger balance
         ↓
... continues automatically every 4 hours
```

---

## Frequently Asked Questions

### Why is my yield zero?

Interest is not guaranteed. Yield can be zero in any given period depending on market conditions and yield source performance. Simple Earn works with DeFi protocols and is not a bank deposit, so capital preservation cannot be guaranteed; in rare cases (for example a smart-contract vulnerability) losses may occur. GoMining reduces this risk by selecting, monitoring, and rotating protocols, but risk cannot be fully eliminated.

### Why does APR differ between assets?

Each asset has unique staking, DeFi, and liquidity opportunities. GoMining's liquidity manager sets individual APR for each asset based on available yields in the market.

### When does my deposit start earning?

Your deposit starts earning from the next full 4-hour cycle after it lands. To earn for a cycle, the balance must be held for the entire 4-hour cycle.

### Is the APR fixed?

No. APR is variable and can change over time as market conditions and yield source performance fluctuate. GoMining's liquidity manager adjusts rates accordingly.

### How does auto-compounding work?

BTC rewards credited at the end of each 4-hour cycle are automatically added to your Simple Earn balance. The larger balance then earns in the next cycle, effectively compounding your returns without any manual action.

### What happens to my rewards if I withdraw?

There are no penalties for withdrawal. Any rewards already credited to your balance are yours to keep. Because rewards use the minimum balance held during a cycle, withdrawing mid-cycle lowers that cycle's reward.
