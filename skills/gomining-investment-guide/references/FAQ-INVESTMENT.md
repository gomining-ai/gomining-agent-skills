# Investment FAQ

Common questions about investing in the GoMining ecosystem.

---

## Getting Started

### What is the minimum amount to start with GoMining?

The absolute minimum is **$10 for Simple Earn** — deposit BTC, USDT, or USDC and earn daily BTC dividends. For a Digital Miner, expect to start around **$50–100** for entry-level options.

### Do I need KYC to use GoMining?

**KYC Level-1** (government ID + selfie) is required for withdrawals, buying miners, marketplace access, and Simple Earn. **KYC Level-2** (address proof + tax info) is only needed for the GoMining Card. Deposits and token purchases work without KYC.

### What should I buy first — a miner or Simple Earn?

It depends on your budget and region:
- **Under $50:** Simple Earn is your only option (if available in your region)
- **$50–100:** An entry-level miner that mines BTC
- **$100+:** Combine both — miner for mining income, Simple Earn for yield on remaining balance
- **USA, EEA, UK users:** Simple Earn is restricted; focus on miners and the Card

### How do I fund my GoMining wallet?

Several options:
- **Crypto deposit** — send BTC, ETH, USDT, USDC, GMT, or other supported tokens from any wallet
- **Card payment** — buy crypto directly via Ecommpay card processing
- **On-ramp services** — Ecommpay On-Ramp or Mercuryo for fiat-to-crypto conversion
- **Open Banking (PSD2)** — available in select EU countries (France, Spain, Estonia, Belgium, Hungary) with lowest fees

---

## Digital Miners

### Should I buy a miner or use Simple Earn for passive income?

Both generate BTC, but they serve different purposes:
- **Miner:** You own a miner with mining power (TH/s). Generates daily BTC rewards. Has maintenance costs. The miner itself can appreciate or be sold. Contributes to your VIP tier via hashrate.
- **Simple Earn:** Simpler — deposit and earn yield. No lockup, no maintenance costs. But you don't own a mining asset, and it's not available in USA/EEA/UK.

For maximum income, use both: miner for mining rewards + Simple Earn on idle balances.

### How much does a miner earn per day?

Earnings depend on many factors:
- **Your hashrate (TH/s):** More TH = more BTC
- **Bitcoin mining difficulty:** Changes every ~2 weeks; higher difficulty = less BTC per TH
- **BTC price:** Doesn't affect BTC amount, but affects USD value
- **Maintenance costs:** Deducted daily; reduce with discounts (GOMINING token 20%, VIP, Service Button 3%)
- **Efficiency (W/TH):** Lower is better — less electricity cost per TH

Use `get_nft_mining_rewards` or `get_mining_income` for a specific miner's actual earnings.

### What blockchain should I buy my miner on?

Miners are available on Ethereum, BSC, Solana, and TON. The blockchain affects:
- **Gas fees:** TON and Solana are cheapest for transactions
- **Secondary marketplace:** Different marketplaces per chain (OpenSea for ETH/BSC, Magic Eden for Solana, Getgems for TON)
- **Mining performance:** Identical — the blockchain only affects where the miner is stored, not mining output

### Can I sell my miner later?

Yes. Miners can be sold on:
- **GoMining secondary marketplace** (in-platform)
- **External marketplaces:** OpenSea (ETH/BSC), Magic Eden (Solana), Getgems (TON)

You can also list your miner for sale directly within the GoMining app.

---

## Simple Earn

### What APR can I expect from Simple Earn?

APRs vary by asset and are not guaranteed. Current rates (fetch live data via `get_simple_earn_config`):
- **Stablecoins (USDT, USDC):** ~9.85% base APR
- **TON:** ~13.2% base APR
- **SOL:** ~3.35% base APR
- **BTC:** ~2.27% base APR
- **ETH:** ~1.5% base APR

VIP level multipliers range from 1.0x (Bronze) to 1.46x (max level). Platinum+ subscription gives x1.2.

### When do Simple Earn rewards pay out?

- **23:59 UTC:** System snapshots all Simple Earn balances
- **07:00 UTC (next day):** BTC dividends credited
- Only balances present at the 23:59 UTC snapshot earn for that cycle
- Rewards auto-compound — BTC earned is reinvested automatically

### Is Simple Earn risk-free?

No. Key risks:
- APR is **variable and not guaranteed** — can be zero in any period
- Yields come from blockchain staking, DeFi protocols, and internal liquidity management
- Platform risk — your funds are held in GoMining's custody (Fireblocks-powered)
- Not available in USA, EEA, UK, and sanctioned countries

---

## VIP & Progression

### How do I reach Silver VIP level?

Two paths (either qualifies):
1. **Hashrate:** Accumulate 10 TH/s of mining power (~$250–500 in miners)
2. **Voting power:** Lock enough GOMINING tokens to have 100 veGOMINING (~$30–60 in tokens at current prices, plus lock period)

### What's the cheapest way to reach Silver I?

Locking GOMINING tokens for veGOMINING is usually cheaper than buying hashrate. At ~$0.30/token, 100 veGOMINING costs roughly $30–60 in tokens (depending on lock duration — longer lock = more VE per token). Compare this to ~$250–500 for 10 TH/s via miners.

### Is the Platinum+ subscription worth it?

Platinum+ costs ~$49/month and instantly gives:
- 2% card cashback (vs 0.5% at Bronze)
- x1.2 Simple Earn APR multiplier
- 2.1% maintenance discount
- 15% spell discounts in Miner Wars

**Worth it if:** You have significant Simple Earn balances, use the Card actively, or play Miner Wars. The earn multiplier alone on a $5K+ Simple Earn balance can offset the subscription cost.

**Not worth it if:** You're at $100–500 total investment — the monthly cost exceeds the benefits.

---

## MNPL (Mine Now, Pay Later)

### Is MNPL worth it?

MNPL lets you control a larger miner with 25% down at **0% APR**. Key considerations:
- **Upside:** 4x mining power vs spending the same amount directly. Miner generates BTC immediately.
- **Downside:** Monthly payments are an obligation. If mining rewards don't cover installments, you pay from pocket.
- **Best for:** Investors with $5K+ budget who believe in long-term BTC mining profitability.
- **Not available in:** India and restricted territories.

### Can mining rewards cover MNPL payments?

Potentially, but not guaranteed. It depends on:
- BTC price and mining difficulty at time of payments
- Your miner's efficiency (W/TH)
- Maintenance costs
- Monthly installment amount

Conservative approach: budget for payments from personal funds, treat mining rewards as bonus.

---

## Returns & Risk

### How long until I see returns?

- **Mining rewards:** Credited daily — you see BTC from day one
- **Simple Earn:** Credited at 07:00 UTC daily — first payout within 24–48 hours
- **Break-even on investment:** Depends on BTC price, mining difficulty, maintenance costs. This is a long-term investment; don't expect quick returns.

### What are the main risks?

| Risk | Description |
|------|-------------|
| BTC volatility | BTC price affects USD value of mining rewards |
| Mining difficulty | Increases over time, reducing per-TH BTC rewards |
| Maintenance costs | Daily electricity fees reduce net profit |
| GMT token price | May decrease, affecting locked position value |
| Simple Earn APR | Variable, not guaranteed, can be zero |
| Regulatory | Products may become restricted in your region |
| MNPL obligation | Monthly payments regardless of mining performance |

### Is GoMining a guaranteed investment?

No. Like all crypto investments, GoMining carries risk. BTC mining rewards depend on Bitcoin's network difficulty and price. Simple Earn APRs are variable. Token values fluctuate. Never invest more than you can afford to lose.

---

## BTC Loans

### How do BTC Loans work?

You deposit BTC as collateral and borrow USDT or USDC. This gives you liquidity without selling your Bitcoin. Key uses for investors:
- Buy miners without selling BTC holdings
- Fund Simple Earn deposits while maintaining BTC exposure
- Cover MNPL down payments

### What's the liquidation risk?

If BTC price drops significantly, your loan's LTV (Loan-to-Value) ratio increases. If it exceeds the liquidation threshold, your BTC collateral may be partially or fully liquidated. Monitor your LTV ratio and add collateral if needed.

---

## Optimization

### How do I maximize my mining returns?

Stack all available discounts:
1. **Pay maintenance in GOMINING tokens** — up to 20% discount (based on token balance vs maintenance cost)
2. **VIP level discount** — increases with tier (up to 6% at Elite)
3. **Service Button** — click daily for 10 consecutive days for 3% discount
4. **Reinvestment bonus** — +5% at Silver I+ when reinvesting mining rewards into TH/s

### Should I reinvest mining rewards or withdraw?

- **Reinvest** if you're building hashrate toward a VIP tier (Silver, Gold) — the +5% reinvestment bonus at Silver I+ makes this more efficient than buying TH separately
- **Withdraw** if you need the BTC or want to take profits
- **Hybrid:** Reinvest a portion, deposit the rest in Simple Earn for additional yield
