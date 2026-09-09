---
name: gomining-miners
description: "GoMining Digital Miners collections — NFTs representing ownership in Bitcoin mining infrastructure. Covers NFT definition and blockchain distribution (Ethereum, BSC, Solana, TON), BMINE issuer, daily BTC rewards mechanism, 12 rarity attributes, Mining mode vs Miner Wars mode, accessing miners via GoMining account or external wallets (MetaMask, Trust Wallet), marketplace trading, GoMiner Avatars product, miner creation calculator location, per-miner reward history navigation, energy efficiency limits, and BTC reward calculation examples."
license: Apache-2.0
compatibility: "Compatible with Claude Code, Codex, and all Agent Skills spec tools."
metadata:
  author: gomining
  version: "1.1"
  tags:
    - nft
    - digital-miners
    - mining
    - blockchain
    - ethereum
    - solana
    - bsc
    - ton
    - rewards
    - avatars
  triggers:
    - "digital miners"
    - "nft mining"
    - "mining rewards"
    - "blockchain networks"
    - "rarity attributes"
    - "miner wars"
    - "btc rewards"
    - "mining mode"
    - "game mode"
    - "modes"
    - "gominer avatars"
    - "gominers"
    - "avatar benefits"
    - "luminar"
    - "sentinel avatar"
    - "human avatar"
    - "cryptile"
    - "goclub"
    - "avatar series"
    - "miner wars profile"
    - "change name miner wars"
    - "username miner wars"
    - "display name"
    - "reward history"
    - "per miner rewards"
    - "miner reward breakdown"
    - "past upgrade data"
    - "upgrade history"
    - "where is calculator"
    - "create miner calculator"
    - "12 w/th"
    - "15 w/th"
    - "best energy efficiency"
    - "minimum w/th"
    - "btc calculation example"
    - "daily reward calculation"
    - "how much will i make"
---

# Digital Miners (NFTs)

## Overview

Digital Miners are NFT collections representing ownership stakes in actual data center computing power actively engaged in Bitcoin mining. The collections are issued and distributed by **BMINE** across multiple blockchain networks.

Holders receive daily BTC rewards calculated from their mining power allocation and energy efficiency metrics. Additionally, these assets function as collectible artwork tradeable on public marketplaces.

---

## Supported Blockchains

Digital Miners are available on four blockchain networks:

| Blockchain | Network Type | Marketplace |
|------------|--------------|-------------|
| **Ethereum** | EVM Layer 1 | OpenSea |
| **BSC** | Binance Smart Chain | OpenSea |
| **Solana** | Solana Network | Magic Eden |
| **TON** | The Open Network | Getgems |

---

## Key Features

### Daily BTC Rewards

Each Digital Miner generates Bitcoin rewards based on:

| Factor | Description |
|--------|-------------|
| Mining Power | Hash rate allocation represented by the NFT |
| Energy Efficiency | Power consumption efficiency metrics |
| Network Difficulty | Current Bitcoin network mining difficulty |
| Pool Performance | Data center mining pool statistics |

Rewards accumulate daily and can be withdrawn to your wallet.

### Collectible Artwork

Digital Miners are unique digital art pieces with:
- Custom visual designs
- Rarity-based attributes
- Tradeable on NFT marketplaces
- Collectible value beyond mining utility

---

## Rarity Attributes

Miners possess **12 customizable attributes** affecting rarity:

| Attribute | Category |
|-----------|----------|
| Basement | Base structure |
| Body | Main chassis |
| Buttons | Control interface |
| Bottom fan | Lower cooling |
| Top fan | Upper cooling |
| Items | Accessories |
| Screen | Display unit |
| Stickers | Decorations |
| UI | Interface design |
| Upgrades | Enhancement modules |
| Walls | Housing panels |
| Down Fan | Double fan option |

> **Note:** There is no strict mathematical ratio to the rarity values. OpenSea hosts rarity information for Ethereum and BSC collections.

---

## Current Pricing & Costs (March 2026 Snapshot)

**Important:** These values change frequently. Always check the GoMining app or calculator for current rates.

| Metric | Approximate Value | Notes |
|--------|-------------------|-------|
| **TH Price** | ~$20-30 per TH | Varies by efficiency (W/TH) |
| **Hash Price** | ~$0.065-0.07/TH/day | Revenue per TH |
| **Maintenance Cost** | ~$0.04-0.07/TH/day | Before discounts |
| **Net Profit** | ~$0.01-0.03/TH/day | After maintenance |

### Maintenance Discounts

| Discount Type | Maximum | How to Obtain |
|--------------|---------|---------------|
| GOMINING Token Payment | 20% | Hold 360+ days maintenance in tokens |
| VIP Level | 6% | Reach Elite tier |
| Service Button | 3% | Click daily for 10 days |
| Mining Mode | Variable | Based on Burn & Mint cycles |

For real-time pricing and live sources, see [Live Market Data](../gomining-overview/references/LIVE-MARKET-DATA.md).

---

## Energy Efficiency — Current Limits

Energy efficiency is measured in W/TH (watts per terahash). **Lower is better** — a lower W/TH means lower electricity fees and higher net rewards.

- There is **no single platform-wide W/TH floor, and 15 W/TH is not the best available.** The lowest efficiency you can reach depends on the specific miner and is shown in that miner's **Create Miner** / **Upgrade** flow; the best available keeps improving as new miners and collections launch.
- Efficiencies **below 15 W/TH exist** — **12 W/TH miners are available**, and some miners reach single-digit W/TH. Never tell a user a given efficiency (e.g. 12 W/TH) is "not available," and never call 15 W/TH the floor.
- If a user says they own a miner at a specific W/TH, treat that first-hand information as **accurate** — do not contradict it or double down on a general claim. For the exact lowest value available to them, point to their miner's create/upgrade flow.
- Exception: GoMiner Avatars of the **Cryptile** series improve a miner farm's effective efficiency by 1 W/TH, but not below 20 W/TH.

### Electricity Cost Example

If electricity costs $0.05/kWh and your miner has 8 TH:

| Efficiency | Daily Electricity Cost |
|------------|------------------------|
| 28 W/TH | (28 × 8) × $0.05 × 24 / 1000 = **$0.2688** |
| 20 W/TH | (20 × 8) × $0.05 × 24 / 1000 = **$0.192** |
| 15 W/TH | (15 × 8) × $0.05 × 24 / 1000 = **$0.144** |

---

## BTC Reward Calculation

### Formula

```
Net Daily Reward (BTC) = Pool Reward per TH × TH − [(C1 + C2) × (1 − Total Discount)]
```

Where:
- **Pool Reward per TH** = hash price in BTC (e.g., $0.065/TH/day ÷ BTC price)
- **C1** = electricity cost per TH per day (depends on W/TH and electricity rate)
- **C2** = service/maintenance cost per TH per day
- **Total Discount** = sum of all active discounts (token, VIP, service button, etc.)

### Worked Example

> **Scenario:** 625 TH at 15 W/TH, 17% total maintenance discount, BTC price = $90,000

**Step 1 — Gross revenue:**
- Hash price ≈ $0.065/TH/day (approximate; check live data for current rate)
- Gross revenue = 625 TH × $0.065 = **$40.625/day**

**Step 2 — Electricity cost (C1):**
- Electricity rate ≈ $0.05–$0.07/kWh (use $0.06 as midpoint)
- C1 = (15 W/TH × 625 TH) × $0.06 × 24 / 1000 = 9,375 W × $0.06 × 24 / 1000 = **$13.50/day**

**Step 3 — Service cost (C2):**
- Service cost is variable; combined with electricity it typically totals ~$0.04–$0.07/TH/day before discounts
- Using ~$0.065/TH/day total (C1+C2): total fees before discount = 625 × $0.065 = **$40.625/day**

**Step 4 — Apply 17% discount:**
- Fees after discount = $40.625 × (1 − 0.17) = **$33.72/day**

**Step 5 — Net USD profit:**
- Net = $40.625 − $33.72 = **~$6.90/day**

**Step 6 — Convert to BTC:**
- Net BTC = $6.90 / $90,000 ≈ **0.0000767 BTC/day**

> **Important:** Hash price and maintenance costs fluctuate daily. Use the **Create Miner calculator** in the app for a real-time estimate with current rates. The example above uses approximate values.

---

## Earning Modes

Digital Miners support two distinct earning modes:

### Mining Mode

| Aspect | Description |
|--------|-------------|
| Activation | Automatically active upon purchase |
| Rewards | Accumulated BTC from mining operations |
| Withdrawal | Available for withdrawal to external wallet |
| Passive | No active participation required |

### Miner Wars Mode

| Aspect | Description |
|--------|-------------|
| Activation | Switch from Mining mode in settings |
| Rewards | Game-based rewards through gameplay |
| Boosts | GOMINING tokens can activate boosts |
| Active | Requires player participation |

---

## Accessing Your Miners

Users can locate and manage their Digital Miners through two methods:

### GoMining Personal Account

1. Log in to your GoMining account
2. Navigate to the **Mining Farm** section
3. View all owned miners with stats and rewards

### External Wallets

Supported wallets for viewing and managing NFTs:

| Wallet | Chains Supported |
|--------|------------------|
| MetaMask | Ethereum, BSC |
| Trust Wallet | Ethereum, BSC, Solana |
| Phantom | Solana |
| Tonkeeper | TON |

---

## Where to Find Reward History & Per-Miner Stats

### Overall Rewards Section

To see your reward history:
1. Go to **My Miners → Rewards** in the GoMining app
2. Tap any payment record to see the full breakdown
3. Tap a specific miner within that record to see its individual pool reward and all deductions

### Per-Miner Reward Breakdown

To see how much a specific miner has mined:
- Open the miner card in **Mining Farm**
- Tap the payment record in the Rewards section, then tap the individual miner to see its pool reward, electricity cost, service cost, and net reward for that day

### Past Upgrade Data

Upgrade history (past TH and energy efficiency upgrades) can be reviewed in the **Rewards** section — each reward entry reflects the miner's specs at the time. TH reinvestment upgrades are also confirmed via email.

---

## Where Is the Miner Creation Calculator?

The built-in calculator is located inside the **Create Miner** flow:

1. Log in to your GoMining account
2. Go to **My Miners** (or tap **Create Miner** on the Home screen)
3. Click/tap **Create Miner**
4. Select your desired **Power (TH/s)** and **Energy Efficiency (W/TH)**
5. The calculator automatically shows estimated **daily, monthly, and yearly BTC rewards** plus projected annual ROI based on current network conditions

The calculator updates in real time as you adjust power and efficiency sliders.

> **No pre-filled / parameterized calculator link.** The calculator URL does **not** support query parameters (e.g. `?efficiency=15`), so you **cannot** generate a link that opens it with settings already applied. If a user asks for "a calculator link set to 15 W/TH" (or any pre-set value), don't invent such a URL — explain there's no pre-filled link and give the manual steps: open the **Create Miner** calculator and set the efficiency/power yourself.

### What exactly does the calculator show? (inputs and outputs)

**Inputs you can adjust (left side):**

- **Digital Miner Price** — a slider (spans roughly $13 up to ~$4,000+). Price and Computing Power move together — setting one adjusts the other.
- **Computing Power** — a slider in **TH** (from 1 TH up the scale — 2, 4, 8, 16, 32, 48, 64, 96, 128, 192, 256 …).
- **Energy Efficiency** — the **W/TH** for the miner (e.g. 12 W/TH); lower is better.
- **Expected BTC price** — a slider to model earnings at a chosen BTC price (roughly **$60K–$130K**). This is a "what-if" input, not a live price.
- **VIP discount** — shows your VIP-based maintenance discount %.
- Two discount toggles: **−20% with GOMINING token** and **−3% with the Service button** — turning them on applies those maintenance discounts to the payback figure.

**Outputs (right side — "Average BTC rewards"):**

- **Daily** — estimated daily reward, shown in **USD and BTC**.
- **Per month** — estimated monthly reward, in **USD and BTC**.
- **Annual payback in BTC** — the projected yearly ROI %, shown with vs without your discounts (see below).
- Footnote: *BTC rewards are shown **before** maintenance fees, while payback is **after** fees; values are approximate and depend on network difficulty, BTC price, and other factors.*
- A **Create miner** button confirms the configuration.

When a user asks "what does the calculator show / how much will I make", walk them through these inputs and outputs. Do **not** quote a specific daily/monthly figure yourself (it depends on live network difficulty and BTC price) — have them read it from the calculator with their own settings.

### "Annual payback in BTC" — is it calculated with the maintenance discount?

**Yes.** In the calculator, the **BTC rewards** (daily/monthly) are shown **before** maintenance fees, but the **Annual payback in BTC** is calculated **after** fees **and reflects the discounts you have enabled** (VIP discount, −20% for paying with the GOMINING token, −3% Service button). Toggling discounts on **raises** the payback %: the calculator shows the lower figure struck through (without discounts) next to the higher active figure (with your discounts) — e.g. ~~52.67%~~ → **64.71%**. All values are approximate and depend on network difficulty, BTC price, and other factors.

---

## Miner Wars — Profile & Display Name

In Miner Wars, your profile is visible to other players across leaderboards, GoClub, and the ecosystem. To change your display name or profile picture:

- Go to your **Profile** settings in the GoMining app
- Update your **username/display name** from the profile section
- To activate a GoMiner Avatar as your profile picture (and unlock its unique ability), go to **My GoMiners**, tap the avatar, and tap **Activate ability** — this sets it as your profile picture

> **Note:** These skills do not document a dedicated "Miner Wars username" field separate from the main GoMining account profile. Your GoMining account display name is what appears in Miner Wars. If you cannot find the option, contact GoMining support.

---

## GoMiner Avatars

GoMiners are limited-edition digital avatars that unlock exclusive benefits in the GoMining ecosystem. They are a separate product from Digital Miners.

### Core Benefits (All Avatar Holders)

| Benefit | Details |
|---------|--------|
| **GoClub access** | Private club with online & offline meetups, member-only content, and special privileges |
| **5% discount** | Permanent discount on miner creation and power upgrades |
| **Pre-sale access** | Buy new limited miner collections before general availability |
| **Welcome pack** | Official GoMining merch shipped worldwide (first claimed avatar only; one-time per avatar) |

### Avatar Series & Unique Abilities

Each series has its own unique ability **in addition** to the core benefits above:

| Series | Unique Ability |
|--------|---------------|
| **Luminars** | +1 VIP level instantly. You receive a GoBox for any VIP level reached with a Luminar (first time only; GoBox Bronze not issued if reached via avatar). |
| **Sentinels** | 20% discount on Miner Wars spells and boosts |
| **Humans** | Automatic 3% maintenance discount — no need to click the Service button daily |
| **Cryptiles** | Upgrades mining farm efficiency by 1 W/TH (but not below 20 W/TH) |

### How to Get a GoMiner Avatar

**Option 1 — Claim with a Key:**
- Keys are found inside **GoBoxes** (earned via VIP level-ups, raffles, and promotions)
- Keys appear automatically in the **My GoMiners** section of your profile
- To use: go to **Marketplace → GoMiners**, choose an available avatar, tap **Claim**
- Choose storage: GoMining wallet or any linked Ethereum wallet

**Option 2 — Buy on the Marketplace:**
- Purchase directly from other users on the GoMining Marketplace
- All benefits transfer to the new owner upon purchase
- Note: the Welcome pack is only awarded once — if the previous owner claimed it, it cannot be claimed again

### Using Your GoMiner Avatar

- All avatars are stored in **My GoMiners** (in your profile)
- Most core perks activate automatically upon claiming
- **Welcome pack:** not automatic — tap the button on the avatar's page to order it
- **Unique ability:** requires setting the avatar as your profile picture — tap **Activate ability** on the avatar card and save changes
- Once activated, the unique ability works immediately and your avatar is visible to other users

### Multiple Avatars

- Benefits **do not stack** (e.g., two Sentinels do not give 40% spell discount)
- You can own multiple avatars from different series and **switch** which one is active by changing your profile picture
- Example: activate a Human to reduce maintenance costs, then switch to a Sentinel when playing Miner Wars

### Selling an Avatar

- Tap **Sell** on the avatar card to list it on the Marketplace
- You keep all perks until the avatar is purchased by another user

---

## Purchasing Digital Miners

Digital Miners can be acquired through:

| Method | Description |
|--------|-------------|
| GoMining Marketplace | Primary sales and official drops |
| OpenSea | Secondary market for ETH/BSC miners |
| Magic Eden | Secondary market for Solana miners |
| Getgems | Secondary market for TON miners |

> **Tip:** Use GOMINING tokens for purchases in the official marketplace to access potential discounts.

---

## Frequently Asked Questions

### What are Digital Miners?

Digital miners represent ownership stakes in actual data center computing power actively engaged in Bitcoin mining. Holders receive daily BTC rewards calculated from their mining power allocation and energy efficiency metrics.

### On which blockchains are Digital Miners available?

The collections are issued and distributed by BMINE on the Ethereum, BSC, Solana, and TON blockchains.

### What rarity attributes do Digital Miners have?

Miners possess 12 customizable attributes affecting rarity: Basement, Body, Buttons, Bottom fan, Top fan, Items, Screen, Stickers, UI, Upgrades, Walls, and Down Fan (double fan option). There is no strict mathematical ratio to the rarity values.

### How do I access my Digital Miners?

Users can locate miners through the GoMining personal account Mining farm section or through external wallets like MetaMask, Trust Wallet, and others.

### How do I earn rewards with Digital Miners?

Purchasing activates Mining mode, generating accumulated BTC rewards for withdrawal. Alternatively, players can switch to Miner Wars mode for game-based rewards.

### Where do I see how much each miner mines?

Go to **My Miners → Rewards** in the app. Tap any payment record, then tap a specific miner to see its individual pool reward, electricity cost, service cost, and net reward for that day.

### Where is the miner creation calculator?

The calculator is built into the **Create Miner** flow. Go to **My Miners → Create Miner**, then select your desired power (TH/s) and energy efficiency (W/TH). The calculator shows estimated daily, monthly, and yearly BTC rewards in real time.

### Is 12 W/TH energy efficiency available?

Yes — **12 W/TH miners exist**, and there is no fixed platform-wide floor at 15 W/TH. The best efficiency available depends on the specific miner and is shown in its **Create Miner** / **Upgrade** flow, and it improves over time as new miners launch. Don't tell users 12 W/TH (or any specific value) is unavailable, and if a user reports owning one, take that as accurate.

### Can I change my display name in Miner Wars?

Your Miner Wars display name is your GoMining account profile name. You can update it in your **Profile** settings in the GoMining app. To set a GoMiner Avatar as your profile picture (which also activates its unique ability), go to **My GoMiners**, tap the avatar, and tap **Activate ability**.

### What are GoMiner Avatars?

GoMiners are limited-edition digital avatars that unlock exclusive benefits: GoClub access, a 5% discount on miner creation and upgrades, pre-sale access to new collections, and a welcome merch pack. Each avatar series also has a unique ability (e.g., Sentinels get 20% off Miner Wars spells; Humans get automatic 3% maintenance discount). See the [GoMiner Avatars](#gominer-avatars) section above for full details.

---

## Official Resources

| Resource | URL |
|----------|-----|
| Digital Miners FAQ | https://help.nft.gomining.com/ |
| Main Website | https://gomining.com/ |
| GoMiners Avatars | https://gomining.com/gominers |

---

## References

- [Mining Farm Screen Layout](references/MINING-FARM-SCREEN.md) — What the My miners → Mining farm screen contains: tabs, metric tiles, Service/Settings, list sorting
- [Leaderboards](references/LEADERBOARDS.md) — The four leaderboard tabs (Miner rewards, Miner uniqueness, Farms, Liquidity) and the Liquidity Pools program wind-down
- [Blockchain Networks](references/BLOCKCHAIN-NETWORKS.md) — Detailed chain specifications
- [Rarity System](references/RARITY-SYSTEM.md) — How rarity affects value and rewards
- [Mining Rewards](references/MINING-REWARDS.md) — BTC reward calculation methodology
- [FAQ: Miners Overview](references/FAQ-OVERVIEW.md) — General overview of digital miners product section
- [FAQ: About Miners](references/FAQ-ABOUT.md) — What digital miners are and how they work
- [FAQ: Buying and Selling](references/FAQ-BUYING-SELLING.md) — How to buy, sell, and trade digital miners
- [FAQ: Computing Power](references/FAQ-COMPUTING-POWER.md) — Mining power, TH, and power upgrade mechanics
- [FAQ: Energy Efficiency](references/FAQ-ENERGY-EFFICIENCY.md) — Energy efficiency ratings and upgrades
- [FAQ: Maintenance Fees and Discounts](references/FAQ-MAINTENANCE.md) — Maintenance costs, fee structure, and discount types
- [FAQ: Mining Mode](references/FAQ-MINING-MODE.md) — Mining mode explained, rewards, and settings
- [FAQ: Miner Subscriptions](references/FAQ-SUBSCRIPTIONS.md) — Subscription-based miner options
- [FAQ: Rarity and Achievements](references/FAQ-RARITY.md) — Miner rarity attributes and achievement system
- [FAQ: Rewards](references/FAQ-REWARDS.md) — How mining rewards are calculated and distributed
- [FAQ: Miner Wars Overview](references/MINER-WARS.md) — Introduction to the Miner Wars game mode
- [FAQ: Miner Wars Clans](references/MINER-WARS-CLANS.md) — Clan system, creation, and royalties
- [FAQ: Miner Wars Game Mechanics](references/MINER-WARS-MECHANICS.md) — Game rules, cycles, and scoring
- [FAQ: Miner Wars Spells and Power-ups](references/MINER-WARS-SPELLS.md) — Boosts, spells, and power-up mechanics
- [How-to: Miner Instructions Overview](references/INSTRUCTION-OVERVIEW.md) — Overview of miner how-to guides
- [How-to: Activate a Miner from Getgems](references/INSTRUCTION-ACTIVATE-GETGEMS.md) — Step-by-step guide to activating a TON miner from Getgems
- [FAQ: Subscriptions Overview](references/FAQ-SUBSCRIPTIONS-OVERVIEW.md) — Overview of GoMining subscription products
- [FAQ: Miner Subscription](references/FAQ-MINER-SUBSCRIPTION.md) — Details on the miner subscription plan
- [How-to: Mint a Miner](references/INSTRUCTION-MINT.md) — What minting is (vs creating/selling), wallet setup, network fees, and minting steps
- [How-to: Sell Your Miner](references/INSTRUCTION-SELL.md) — Full guide to listing, 90-day restriction, and marketplace
- [FAQ: Upgrade Rewards & Mode Switching](references/FAQ-UPGRADE-REWARDS.md) — Reward processing timeline after upgrades, mode switching effects
- [FAQ: Reinvestment Options](references/FAQ-REINVEST-OPTIONS.md) — Reinvest settings, all-miner mode, where to see reinvestments
- [FAQ: Maintenance — Advanced](references/FAQ-MAINTENANCE-ADVANCED.md) — PR/MR formula, token payment priority, bonus miners, reward protection
- [FAQ: Raffle Eligibility](references/FAQ-RAFFLE-ELIGIBILITY.md) — Raffle ticket rules, qualifying actions, GoBox raffle
- [FAQ: Why Did My Reward Drop?](references/FAQ-REWARD-DROPS.md) — Network difficulty, maintenance deductions, reinvestment display, common causes and what is NOT a cause
- [Miner Collections](references/MINER-COLLECTIONS.md) — Bonus Miner limitations and tasks, Limited-edition collections (incl. Greedy Machines), Minebox customization and random design
