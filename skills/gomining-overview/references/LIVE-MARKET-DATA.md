# Live Market Data Reference

## Overview

GoMining operations depend on several dynamic market variables that change frequently. This reference explains each metric, provides approximate current values, and directs users to authoritative real-time sources.

**Important:** Values in this document are snapshots and will become outdated. Always check live sources for current data.

---

## Current Values (March 2026 Snapshot)

| Metric | Approximate Value | Update Frequency |
|--------|-------------------|------------------|
| **TH Price** | ~$20-30 per TH | Varies by efficiency (W/TH) |
| **GOMINING Token Price** | ~$0.30 USD | Real-time (market) |
| **BTC Price** | ~$73,000-76,000 USD | Real-time (market) |
| **Maintenance Cost per TH** | ~$0.04-0.07/TH/day | Daily (depends on efficiency) |
| **Simple Earn APR** | ~9.8-14.4% | Variable (set by liquidity manager) |
| **Bitcoin Mining Difficulty** | ~145 T (trillion) | ~Every 2 weeks (2016 blocks) |
| **Hash Price** | ~$0.065-0.07/TH/day | Daily (market-driven) |
| **Block Reward** | 3.125 BTC | Fixed until next halving (~2028) |

---

## Metric Definitions

### TH Price (Cost per Terahash)

The purchase price for 1 TH of mining power on GoMining.

| Aspect | Details |
|--------|---------|
| **What it is** | One-time cost to acquire 1 TH of digital miner hashrate |
| **Factors** | Energy efficiency (W/TH), current demand, promotions |
| **Range** | Varies significantly based on miner efficiency class |
| **Where to check** | GoMining app marketplace or calculator |

**Why it matters:** Lower TH price = faster ROI. More efficient miners (lower W/TH) typically cost more upfront but have lower maintenance costs.

---

### GOMINING Token Price

The current market price of the GOMINING utility token.

| Aspect | Details |
|--------|---------|
| **What it is** | Exchange rate for GOMINING to USD |
| **Current price** | ~$0.30 USD (March 2026) |
| **Where to check** | CoinGecko, CoinMarketCap, exchanges |

**Live Sources:**
- [CoinMarketCap - GOMINING](https://coinmarketcap.com/currencies/gomining-token/)
- [CoinGecko - GOMINING](https://www.coingecko.com/en/coins/gomining-token)

**Why it matters:**
- **veGOMINING route cost:** To calculate how much it costs to reach a VIP tier via veGOMINING (locking tokens), multiply tokens needed by current price
- **Maintenance payments:** Paying maintenance in GOMINING grants up to 20% discount
- **Marketplace purchases:** Token price affects miner and avatar purchase costs

---

### BTC Price

The current market price of Bitcoin.

| Aspect | Details |
|--------|---------|
| **What it is** | Exchange rate for BTC to USD |
| **Current price** | ~$73,000-76,000 USD (March 2026) |
| **Where to check** | Any crypto exchange or price aggregator |

**Why it matters:**
- **Daily reward value:** Multiply your daily BTC reward by BTC price to get USD value
- **ROI calculations:** Higher BTC price = faster ROI on miner purchases
- **Hash price impact:** BTC price directly affects hash price (revenue per TH)

---

### Maintenance Cost per TH

The daily operating cost for each TH of mining power.

| Aspect | Details |
|--------|---------|
| **What it is** | Daily electricity + service fee per TH |
| **Components** | Electricity cost + service fee |
| **Calculation** | `NetReward = PoolReward - ((Electricity + Service) × (1 - Discounts))` |

**Discount Stack:**
| Discount Type | Maximum | How to Get |
|--------------|---------|------------|
| GOMINING Token | 20% | Hold 360+ days of maintenance in tokens |
| VIP Level | 6% | Reach Elite tier |
| Service Button | 3% | Click daily for 10 consecutive days |
| Mining Mode | Variable | Based on Burn & Mint cycles |

**Why it matters:** Maintenance is deducted from gross mining rewards. Lower maintenance = higher net profit.

---

### Simple Earn APR

The annual percentage rate for Simple Earn deposits.

| Aspect | Details |
|--------|---------|
| **What it is** | Estimated annual yield on deposited assets |
| **Current range** | ~9.8-14.4% APR |
| **Setter** | GoMining liquidity manager |
| **Variability** | Changes based on market conditions |

**Important Notes:**
- APR is **not guaranteed** and can be zero
- Each asset (BTC, USDT, USDC, SOL) has its own APR
- VIP tier provides APR boost (Platinum+ gets x1.2 multiplier)
- Rewards paid in BTC regardless of deposited asset

**Where to check:** GoMining app Simple Earn section shows current APR per asset.

---

### Bitcoin Mining Difficulty

The network-wide difficulty of mining a Bitcoin block.

| Aspect | Details |
|--------|---------|
| **What it is** | Measure of how hard it is to mine a block |
| **Current value** | ~145 T (trillion) as of March 2026 |
| **Adjustment** | Every 2,016 blocks (~2 weeks) |
| **Where to check** | Blockchain explorers, mining statistics sites |

**Live Sources:**
- [CoinWarz Difficulty Chart](https://www.coinwarz.com/mining/bitcoin/difficulty-chart)
- [Minerstat BTC Difficulty](https://minerstat.com/coin/btc/difficulty)

**Why it matters:**
- Higher difficulty = lower BTC reward per TH
- Difficulty adjusts based on total network hashrate
- Affects profitability calculations and ROI projections

---

### Hash Price

Revenue generated per TH per day.

| Aspect | Details |
|--------|---------|
| **What it is** | USD earned per 1 TH/s per day |
| **Current value** | ~$0.065-0.07/TH/day (March 2026) |
| **Calculation** | Based on BTC price, block reward, and difficulty |

**Historical Context:**
- Post-halving low (2024): ~$0.045/TH/day
- Profitability threshold: ~$0.04/TH/day (below this, many miners operate at loss)

**Why it matters:** Hash price is the gross revenue before maintenance costs. Compare to your maintenance cost to determine profitability.

---

## Quick Reference: Where to Find Live Data

| Metric | Primary Source | Alternative |
|--------|---------------|-------------|
| TH Price | GoMining app/marketplace | [GoMining Calculator](https://gomining.com/calculator) |
| GOMINING Price | [CoinMarketCap](https://coinmarketcap.com/currencies/gomining-token/) | [CoinGecko](https://www.coingecko.com/en/coins/gomining-token) |
| BTC Price | [CoinDesk](https://www.coindesk.com/price/bitcoin) | Any exchange |
| Maintenance Cost | GoMining app (miner details) | [GoMining Calculator](https://gomining.com/calculator) |
| Simple Earn APR | GoMining app (Simple Earn section) | — |
| Mining Difficulty | [CoinWarz](https://www.coinwarz.com/mining/bitcoin/difficulty-chart) | [Minerstat](https://minerstat.com/coin/btc/difficulty) |
| Hash Price | Mining statistics sites | [Third-party calculators](https://www.gominingcalculator.com/) |

---

## Calculating Key Values

### Daily Net Profit per TH

```
Daily Net Profit = Hash Price - Maintenance Cost
```

Example (March 2026):
- Hash Price: $0.065/TH/day
- Maintenance: $0.045/TH/day (after discounts)
- **Net Profit: $0.02/TH/day**

### veGOMINING Route Cost (for VIP tiers)

```
Cost = (Required veGOMINING) × (GOMINING Token Price)
```

Example for Silver I (100 veGOMINING):
- Required: 100 veGOMINING = 100 GOMINING tokens locked
- Token price: $0.30
- **Cost: $30 USD** (tokens locked, not spent)

### ROI Estimation

```
ROI Days = TH Purchase Price / (Daily Net Profit × TH)
```

Example (at current market rates from the GoMining app):
- Purchase: see current TH/s price in the GoMining app
- Daily Net Profit: $0.02/TH (example, varies with BTC price and difficulty)
- **ROI:** depends on purchase price and network conditions

**Note:** ROI calculations are estimates. Actual returns depend on BTC price, difficulty changes, and maintenance costs over time.

---

## FAQ

### Why do values change so frequently?
Cryptocurrency markets operate 24/7. BTC price, token prices, and hash price respond to market supply/demand in real-time. Mining difficulty adjusts every ~2 weeks based on network hashrate.

### How often should I check these metrics?
- **BTC/GOMINING price:** Daily or when making decisions
- **Maintenance costs:** Weekly or when calculating profitability
- **Simple Earn APR:** Before making deposits
- **Mining difficulty:** After each adjustment (~every 2 weeks)

### Where can I see my actual daily earnings?
Your GoMining dashboard shows real-time mining rewards. The values in this document are for planning and calculation purposes.
