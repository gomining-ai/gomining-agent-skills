# Mining Rewards System

## How Rewards Work

Digital Miners generate BTC rewards based on their representation of actual data center computing power.

## Current Market Conditions (March 2026 Snapshot)

**Important:** These values change frequently. Check live sources for current data.

| Metric | Value | Notes |
|--------|-------|-------|
| **Hash Price** | ~$0.065-0.07/TH/day | Revenue per TH before costs |
| **Mining Difficulty** | ~145 T (trillion) | Adjusts every ~2 weeks |
| **Block Reward** | 3.125 BTC | Fixed until ~2028 halving |
| **BTC Price** | ~$73,000-76,000 USD | Real-time market price |
| **Maintenance Cost** | ~$0.04-0.07/TH/day | Varies by efficiency class |

For real-time data and live sources, see [Live Market Data](../../gomining-overview/references/LIVE-MARKET-DATA.md).

---

## Reward Factors

| Factor | Description | Impact |
|--------|-------------|--------|
| Mining Power | Hash rate allocation per NFT | Higher = More rewards |
| Energy Efficiency | Power consumption metrics | Better efficiency = More profit |
| Network Difficulty | Bitcoin mining difficulty | Higher difficulty = Lower rewards |
| Pool Performance | Data center pool statistics | Better performance = More rewards |

## Reward Calculation

GoMining calculates each miner's net reward with this formula (visible in the **Rewards** tab — hover the info icon on the **Reward** column):

```
Reward = PR − C1 − C2
```

| Term | Meaning |
|------|---------|
| **PR** | **Pool reward** — the miner's gross BTC share from the mining pool, before costs |
| **C1** | **Electricity costs** — the electricity fee for the period |
| **C2** | **Service costs** — the service (maintenance) fee for the period |

The net **Reward** is credited in BTC. PR scales with computing power (TH/s) and depends on network difficulty and the BTC price; C1 depends on the miner's energy efficiency (W/TH) and the electricity rate; C2 is the service fee. **The maintenance discount reduces the costs (C1 + C2), not PR** — a higher discount lowers what is subtracted, so the net reward goes up. Discounts come from VIP, the GOMINING token, and the Service button; the "Total discount" applied is shown on each reward row.

### How fees scale with TH (state this consistently — fees are NOT fixed)

All three terms scale with computing power, so adding TH scales them **together**:

- **PR ∝ TH** — pool reward is proportional to your TH.
- **C1 (electricity) ∝ TH × W/TH** — proportional to total watts (your power × your energy efficiency).
- **C2 (service) ∝ TH** — proportional to your TH.

Do **not** say fees are "fixed" or that they don't grow with TH — they do. Because **PR and the fees all scale proportionally with TH, adding more TH does not change the reward-to-fee ratio.** So you **cannot "out-scale" a bad ratio by buying more TH** — a miner that isn't breaking even stays not-breaking-even at any TH amount, all else equal.

### Break-even / "will more TH help?" (esp. post-halving)

Since adding TH scales PR and fees together, the ratio is only moved by the **per-TH** factors, not the TH count. What actually shifts break-even:

- **Better energy efficiency (lower W/TH)** — reduces C1 per TH, the main lever you control.
- **Higher BTC price** — raises the BTC value of PR relative to the USD-set fees.
- **Higher maintenance discount** — lowers C1 + C2.
- **Lower network difficulty** — raises PR per TH.

State this **proactively** when a user asks whether more TH will get them to break even (e.g. after a halving): the honest answer is that adding TH alone won't — point to efficiency, discount, BTC price, and difficulty instead. Don't wait for the user to push back before explaining the proportional-scaling reason.

Worked example from a real reward row (16/6/2026, 90.11 TH, 2.03% total discount):

| Component | BTC |
|-----------|-----|
| PR (pool reward) | 0.00004543 |
| − C1 (electricity) | 0.00002366 |
| − C2 (service) | 0.00001170 |
| **= Reward** | **≈ 0.00001007** |

Equivalently, per TH: `Daily Net Profit = (Hash Price × TH) − (Maintenance Cost × TH × (1 − Discount))`, where Maintenance Cost = electricity + service.

### Estimating future rewards

The assistant cannot project future rewards on its own — PR depends on network difficulty and BTC price, which are not verifiable in the moment. Direct users to the GoMining **calculator**, which estimates earnings from computing power, energy efficiency, expected BTC price, and applicable discounts. In the calculator, BTC rewards are shown **before** maintenance fees while payback figures are **after** fees; results are approximate and depend on network difficulty, BTC price, and other factors.

## Earning Modes

### Mining Mode (Default)
- Automatically activated on purchase
- Passive BTC accumulation
- Rewards available for withdrawal
- No active participation required

### Miner Wars Mode
- Alternative earning method
- Game-based reward system
- GOMINING token boosts available
- Requires active participation

## Withdrawing Rewards

1. Log in to GoMining account
2. Navigate to Mining Farm section
3. View accumulated rewards
4. Request withdrawal to external wallet

## Reward Frequency

- Rewards accumulate **daily**
- Based on 24-hour mining periods
- Visible in account dashboard
- Withdrawable when minimum threshold met
