# ROI Examples

Concrete return calculations for each investment tier using market data. These are **illustrative estimates** — actual returns depend on BTC price, mining difficulty, maintenance costs, and Simple Earn APR changes.

> **Important:** Always fetch live data via `get_ticker_prices`, `get_simple_earn_config`, and `get_nft_mining_rewards` before presenting ROI numbers to users. The examples below use snapshot data and will become stale.

---

## Market Data Used

| Metric | Value | Source |
|--------|-------|--------|
| BTC Price | ~$76,589 | `get_ticker_prices` |
| GMT Price | ~$0.298 | `get_ticker_prices` |
| USDT/USDC Simple Earn APR | 9.85% | `get_simple_earn_config` |
| BTC Simple Earn APR | 2.27% | `get_simple_earn_config` |
| TON Simple Earn APR | 13.20% | `get_simple_earn_config` |

> Mining profitability (hash price, maintenance cost, net profit per TH) varies by miner efficiency class. Use `get_nft_mining_rewards` for a specific miner's actual performance.

---

## $10 Tier — Simple Earn Only

### Scenario: $10 in USDT deposited to Simple Earn

| Metric | Value |
|--------|-------|
| Deposit | $10 USDT |
| Base APR | 9.85% |
| VIP Multiplier | 1.0x (Bronze I) |
| Effective APR | 9.85% |
| **Annual yield** | **~$0.99** (paid in BTC) |
| Daily yield | ~$0.0027 |
| Monthly yield | ~$0.082 |

### With Higher VIP (Silver I, 1.08x multiplier)

| Metric | Value |
|--------|-------|
| Effective APR | 10.64% |
| Annual yield | ~$1.06 |

**Takeaway:** At $10, Simple Earn is about building the habit and learning the platform. Real returns require larger deposits.

---

## $100 Tier — Entry Miner + Simple Earn

### Scenario A: $70 Entry Miner + $30 Simple Earn

**Miner component (illustrative):**

| Metric | Value |
|--------|-------|
| Investment | $70 |
| Estimated TH/s | ~2–3 TH |
| Gross daily BTC revenue | Variable (use `get_nft_mining_rewards`) |
| Maintenance cost | Deducted daily |
| Net daily profit | Gross revenue minus maintenance |

**Simple Earn component:**

| Metric | Value |
|--------|-------|
| Deposit | $30 USDT |
| APR | 9.85% |
| Annual yield | ~$2.96 |
| Monthly yield | ~$0.25 |

**Combined annual estimate:** Miner net profit + ~$3 from Simple Earn.

> At this tier, the miner is the primary income source. Simple Earn is supplementary.

### Scenario B: $100 on GoMining Card

| Metric | Value |
|--------|-------|
| Card balance | $100 |
| Monthly spend | Assume $500 |
| Cashback rate | 0.5% (Bronze) |
| Monthly TH/s earned | $500 × 0.005 = $2.50 in TH |
| Annual TH/s earned | ~$30 in TH |

**Takeaway:** Card cashback compounds — earned TH/s mines BTC forever. Over time, accumulated TH/s from cashback can become a meaningful mining position.

---

## $1,000 Tier — Diversified Portfolio

### Scenario: $650 Miner + $200 Tokens + $150 Simple Earn

**Miner component:**

| Metric | Value |
|--------|-------|
| Investment | $650 |
| Estimated TH/s | ~15–20 TH |
| VIP trigger | Silver I (at 10+ TH) |
| Gross daily BTC revenue | Variable |
| Maintenance discount | 20% (GOMINING) + Silver VIP + 3% (Service Button) |

**Token locking component:**

| Metric | Value |
|--------|-------|
| Investment | $200 (~670 GMT at $0.298) |
| If locked for 4 years | ~670 veGOMINING |
| If locked for 1 year | ~168 veGOMINING |
| Staking rewards | 20% of weekly Burn & Mint distribution (proportional to VE) |
| Governance | Vote on reward allocation + burn coefficient |

**Simple Earn component:**

| Metric | Value |
|--------|-------|
| Deposit | $150 USDT |
| APR | 9.85% × 1.08 (Silver I) = 10.64% |
| Annual yield | ~$15.96 |
| Monthly yield | ~$1.33 |

**Reinvestment bonus (Silver I):**

| Metric | Value |
|--------|-------|
| Bonus | +5% on reinvested mining rewards |
| Effect | Every BTC reinvested buys 5% more TH |

### Combined Annual Estimate

| Income Source | Estimated Annual Value |
|---------------|----------------------|
| Mining rewards (net) | Variable — use `get_mining_income` for actual data |
| Simple Earn yield | ~$16 |
| Staking rewards (veGOMINING) | Proportional to locked VE share of total pool |
| Card cashback (if using) | Depends on spending volume |
| Reinvestment bonus | +5% on any reinvested mining BTC |

---

## $10,000 Tier — Option A (Direct Purchase)

### Scenario: $6,500 Miner + $1,500 Tokens + $1,500 Earn + $500 Card

**Premium Miner:**

| Metric | Value |
|--------|-------|
| Investment | $6,500 |
| Estimated TH/s | ~50–80 TH |
| VIP trigger | Gold I (at 50+ TH) |
| Maintenance discount | 20% (GOMINING) + Gold VIP + 3% (Service Button) |

**Token locking:**

| Metric | Value |
|--------|-------|
| Investment | $1,500 (~5,034 GMT) |
| Locked 4 years | ~5,034 veGOMINING |
| Locked 1 year | ~1,259 veGOMINING |
| VIP boost | Contributes to Gold I+ regardless of hashrate |
| Staking rewards | Larger proportional share of Burn & Mint |

**Simple Earn:**

| Metric | Value |
|--------|-------|
| Deposit | $1,500 USDT |
| APR | 9.85% × 1.16 (Gold I) = 11.43% |
| Annual yield | ~$171 |
| Monthly yield | ~$14.27 |

**Card:**

| Metric | Value |
|--------|-------|
| Balance | $500 |
| Cashback rate | 1.5% (Gold I) |
| If spending $2K/month | $2,000 × 0.015 = $30/month in TH |
| Annual TH accumulation | ~$360 in TH/s |

**Clan (Gold I):**

| Metric | Value |
|--------|-------|
| Royalties | 5% GOMINING from all clan member activity |
| Potential | Scales with number and activity of clan members |

### Combined Annual Estimate

| Income Source | Estimated Annual Value |
|---------------|----------------------|
| Mining rewards (net) | Variable — primary income stream |
| Simple Earn yield | ~$171 |
| Card cashback (at $2K/month spend) | ~$360 in TH/s |
| Staking rewards | Proportional to VE share |
| Clan royalties | Depends on clan size and activity |
| Reinvestment bonus | +5% on reinvested mining BTC |

---

## $10,000 Tier — Option B (MNPL Leverage)

### Scenario: $5K MNPL + $3K Miner + $1.5K Tokens + $500 Earn/Card

**MNPL Miner:**

| Metric | Value |
|--------|-------|
| Down payment | $5,000 |
| Total miner value | $20,000 |
| Estimated TH/s | ~80–100 TH |
| Monthly installment | ~$625 (24 months) or ~$417 (36 months) |
| Mining starts | Day one (immediate) |
| APR | 0% |

**Second Miner (direct):**

| Metric | Value |
|--------|-------|
| Investment | $3,000 |
| Estimated TH/s | ~20–30 TH |
| Combined total TH | ~100–130 TH (MNPL + direct) |

**Token + Earn + Card:** Same as Option A but at reduced amounts.

### MNPL Cash Flow Analysis

| Monthly Item | Amount |
|-------------|--------|
| MNPL mining BTC revenue | Variable (from ~80–100 TH) |
| MNPL maintenance cost | Variable (offset by discounts) |
| MNPL installment payment | ~$417–625/month |
| Second miner net revenue | Variable (from ~20–30 TH) |
| Simple Earn yield | ~$4/month (on $500) |

**Key question:** Does the MNPL miner's net BTC revenue exceed the monthly installment? If yes, the miner pays for itself. If no, you need to cover the gap from personal funds or other GoMining income.

---

## Comparative ROI Summary

| Tier | Primary Income | Simple Earn | VIP Benefits | Total Streams |
|------|---------------|-------------|--------------|---------------|
| $10 | — | ~$1/year | None | 1 |
| $100 | Small mining | ~$3/year | Bronze | 2 |
| $1,000 | Mining (15–20 TH) | ~$16/year | Silver I (+5% reinvest) | 3–4 |
| $10K Direct | Mining (50–80 TH) | ~$171/year | Gold I (clan, royalties) | 4–5 |
| $10K MNPL | Mining (100–130 TH) | ~$50/year | Gold I+ | 4–5 |

---

## Important Disclaimers

- All figures are **illustrative estimates** based on point-in-time data
- Mining profitability changes with BTC price and network difficulty (adjusts every ~2 weeks)
- Simple Earn APR is **variable and not guaranteed** — can be zero
- GOMINING token price fluctuates — locked positions may decrease in value
- Past performance does not guarantee future results
- **Always use live data tools** (`get_ticker_prices`, `get_simple_earn_config`, `get_nft_mining_rewards`, `get_mining_income`) for current numbers
- This is not financial advice — users should do their own research
