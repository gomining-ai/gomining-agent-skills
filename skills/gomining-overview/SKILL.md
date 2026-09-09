---
name: gomining-overview
description: "GoMining platform overview — start here for ecosystem basics. Covers what GoMining is, the three main products (GOMINING Token, Digital Miners NFTs, GoMining Card), project objectives (democratizing Bitcoin mining), official resources and help sites, and how all products interconnect within the ecosystem."
license: Apache-2.0
compatibility: "Compatible with Claude Code, Codex, and all Agent Skills spec tools."
metadata:
  author: gomining
  version: "1.0"
  tags:
    - overview
    - introduction
    - ecosystem
    - bitcoin-mining
    - products
  triggers:
    - "what is gomining"
    - "gomining overview"
    - "ecosystem basics"
    - "platform introduction"
    - "how does gomining work"
    - "how gomining works"
    - "getting started"
    - "gomining products"
    - "about gomining"
    - "tell me about gomining"
    - "new to gomining"
    - "start with gomining"
    - "mining treasure"
    - "gobox"
    - "treasure reward"
    - "chest reward"
    - "special reward items"
    - "promo rewards"
    - "miner subscription"
    - "cancel miner subscription"
    - "cancel subscription"
    - "installment payment"
    - "installment plan"
    - "payment plan miner"
    - "cancel installment"
    - "cancel payment plan"
    - "subscription plan"
    - "hashrate subscription"
    - "monthly hashrate"
    - "pause subscription"
    - "adjust subscription"
    - "how much gmt for th"
    - "gmt needed for hashrate"
    - "how many gmt tokens to buy"
    - "gmt to th conversion"
    - "buy hashrate with gmt"
    - "gmt cost per th"
    - "how much gmt do i need"
    - "pay with gmt marketplace"
    - "gmt marketplace price"
---

# GoMining Platform Overview

## Introduction

GoMining is a blockchain-native platform that democratizes Bitcoin mining by removing barriers like expensive hardware and complex setup requirements. The platform enables users to participate in Bitcoin mining through a suite of interconnected products:

- **GOMINING Token** — The native utility token powering the ecosystem, used for marketplace purchases, maintenance discounts, rewards, and game boosts.
- **Digital Miners (NFTs)** — NFT collections representing ownership stakes in actual data center computing power actively engaged in Bitcoin mining.
- **GoMining Card** — A Visa debit card linked to your crypto wallet with instant crypto-to-fiat conversion.

All services are accessible through the GoMining platform with a unified user experience.

---

## Project Objectives

GoMining developed an easy mining method that does not require:
- Purchasing expensive equipment
- Hardware maintenance
- Technical connections or setup

The initiative aims to lower barriers to entry and reduce the threshold for participating in mining activities, making Bitcoin mining accessible to everyone.

---

## Products

### GOMINING Token

The native utility token functioning as both a crypto-asset management tool and authentication mechanism within the ecosystem.

| Use Case | Description |
|----------|-------------|
| Marketplace | Purchase miners, avatars, and merchandise |
| Maintenance | Pay for miner maintenance with up to 20% discount |
| Rewards | Earn royalties and rewards |
| Gaming | Activate boosts in Miner Wars game |

For detailed token information, see the [gomining-token skill](../gomining-token/SKILL.md).

### Digital Miners (NFTs)

NFT collections issued by BMINE representing ownership in data center computing power.

| Feature | Description |
|---------|-------------|
| Blockchains | Ethereum, BSC, Solana, TON |
| Rewards | Daily BTC from mining power allocation |
| Trading | Collectible artwork on public marketplaces |
| Modes | Mining mode or Miner Wars game mode |

For detailed NFT information, see the [gomining-miners skill](../gomining-miners/SKILL.md).

### GoMining Card

Virtual debit card with crypto payment support. Physical cards will be available in a future release.

| Feature | Description |
|---------|-------------|
| Currencies | GOMINING, BTC, USDT, USDC |
| Conversion | Instant crypto-to-fiat at current rates |
| Compatibility | Apple Pay, Google Wallet |
| Security | PIN + 3DS protection |

For detailed card information, see the [gomining-card skill](../gomining-card/SKILL.md).

---

## Buying Hashrate with GMT Tokens

### How Marketplace Pricing Works

GoMining marketplace prices for miners and hashrate (TH/s) are **denominated in USD**. However, you can pay using GOMINING (GMT) tokens. When you pay with GMT, the checkout converts the USD price into the equivalent GMT amount based on the **current GMT market price** at the time of purchase.

### Calculating How Much GMT You Need

To estimate the number of GMT tokens required to purchase a given amount of hashrate:

```
GMT needed = (TH/s amount × USD price per TH) ÷ current GMT token price (USD)
```

**Example:**
- You want to buy **1,000 TH/s**
- Current marketplace price: **$25 per TH** (varies by miner efficiency and purchase size)
- Current GMT token price: **$0.30**

```
GMT needed = (1,000 × $25) ÷ $0.30 = $25,000 ÷ $0.30 ≈ 83,333 GMT
```

> **Important:** Both the TH price and the GMT token price change frequently. The example above uses approximate values for illustration only. Always check current values before purchasing.

### Where to Find the Live GMT/TH Conversion

You do not need to calculate this manually at checkout. The GoMining marketplace shows the **GMT equivalent** of any purchase automatically:

1. Open the GoMining app and go to **Marketplace → Miners**.
2. Select the miner or hashrate amount you want to purchase.
3. At checkout, choose **GOMINING (GMT)** as your payment method.
4. The checkout screen will display the exact GMT amount required at the current exchange rate.

### Where to Find Current Prices

| Value | Where to Check |
|-------|----------------|
| **TH price (USD)** | GoMining app marketplace or [GoMining Calculator](https://gomining.com/calculator) |
| **GMT token price** | [CoinMarketCap](https://coinmarketcap.com/currencies/gomining-token/) or [CoinGecko](https://www.coingecko.com/en/coins/gomining-token) |
| **GMT amount at checkout** | GoMining app marketplace checkout (shown automatically) |

> **Note:** The TH price decreases with larger purchases on the primary marketplace — buying more TH at once lowers your cost per TH. On the secondary marketplace, prices are set by individual sellers and may differ.

---

## Miner Subscription

A **Miner Subscription** is a feature that automatically adds a fixed amount of TH/s (hashrate) to your miner every month, allowing your mining power to grow on autopilot without requiring manual marketplace purchases each time.

### How It Works

- You set up the subscription once, specifying the amount of hashrate to be added monthly.
- Each month, the agreed hashrate increment is applied to your miner automatically.
- Your total hashrate compounds over time with no additional action required.

### Managing Your Subscription

According to GoMining's documentation, subscriptions can be **paused, adjusted, or cancelled at any time**.

To manage or cancel your Miner Subscription:
1. Open the GoMining app.
2. Navigate to **My miners → Mining Farm**.
3. Locate the miner associated with your subscription.
4. Use the available management options to pause, adjust, or cancel the subscription.

> **Note:** The GoMining reference documentation states that subscriptions can be cancelled at any time, but does not specify additional terms such as refund policies for partially completed payment periods or fees for early cancellation. For precise cancellation terms or if you cannot find the option in the app, contact GoMining support at **support@gomining.com**.

### Who It's For

Miner Subscriptions are suited for users who want consistent hashrate growth without manually monitoring the marketplace every month.

---

## Promos and Bonus Rewards

GoMining offers several ways to earn rewards beyond standard daily mining income. These are accessible via the **Promos** section of the app.

| Reward Type | Description |
|-------------|-------------|
| **GoBoxes** | Reward boxes (sometimes called treasure chests or mining treasure) that can contain miners, hashrate, tokens, or other prizes |
| **Referral Bonuses** | Earn rewards for inviting new users to the platform |
| **VIP Program** | Tiered membership with enhanced discounts and perks |
| **Raffles** | Prize draws for platform participants |
| **Bounty Initiative** | Task-based reward campaigns |

### GoBoxes (Treasure / Chest Rewards)

GoBoxes are reward boxes distributed through promotions, events, and campaigns on the GoMining platform. They may contain:
- Digital miners or additional hashrate (TH/s)
- GOMINING tokens
- Other ecosystem rewards

**Important notes on GoBox value and selling:**
- The value of a GoBox reward depends entirely on its contents once opened.
- If a GoBox contains a **digital miner**, that miner can be listed for sale on the GoMining internal marketplace (**My miners → Selling**) or traded on supported external NFT marketplaces (OpenSea, Magic Eden, Getgems — depending on the blockchain).
- If a GoBox contains **GOMINING tokens**, those can be traded on supported exchanges or used within the ecosystem.
- GoMining does not publish a fixed price for GoBox contents in advance. The market value of any reward item is determined by current marketplace conditions at the time you choose to sell.
- To check the current market value of a miner received from a GoBox, compare it against similar listings in the GoMining marketplace or the relevant external NFT marketplace for its blockchain.

> **Note:** GoMining's reference documentation does not provide specific pricing for GoBox contents or guarantee any particular reward. For the most accurate and current valuation, check live marketplace listings at the time of sale.

---

## Official Resources

| Resource | URL | Description |
|----------|-----|-------------|
| Main Website | https://gomining.com/ | Official platform |
| Alternative | https://gmt.io/en | Alternative domain |
| Token FAQ | https://help.token.gomining.com/ | Token documentation |
| Miners FAQ | https://help.nft.gomining.com/ | Digital Miners documentation |
| Cards FAQ | https://help.cards.gomining.com/ | Card documentation |
| CoinMarketCap (price, ATH, market cap) | https://coinmarketcap.com/currencies/gomining-token/ | Price and market data |
| CoinMarketCap (holders) | https://coinmarketcap.com/currencies/gomining-token/holders/ | Holder counts |

---

## Ecosystem Integration

All GoMining products work together in a unified ecosystem:

```
┌─────────────────────────────────────────────────────────────┐
│                    GoMining Ecosystem                        │
├─────────────────────────────────────────────────────────────┤
│                                                              │
│   ┌──────────────┐    ┌──────────────┐    ┌──────────────┐  │
│   │   GOMINING   │    │   Digital    │    │   GoMining   │  │
│   │    Token     │◄──►│   Miners     │◄──►│    Card      │  │
│   │              │    │   (NFTs)     │    │              │  │
│   └──────────────┘    └──────────────┘    └──────────────┘  │
│          │                   │                    │          │
│          ▼                   ▼                    ▼          │
│   ┌──────────────────────────────────────────────────────┐  │
│   │              GoMining Marketplace                     │  │
│   │    Purchase miners, avatars, merchandise              │  │
│   └──────────────────────────────────────────────────────┘  │
│          │                   │                    │          │
│          ▼                   ▼                    ▼          │
│   ┌──────────────────────────────────────────────────────┐  │
│   │                  Miner Wars Game                      │  │
│   │         Game rewards and token boosts                 │  │
│   └──────────────────────────────────────────────────────┘  │
│          │                   │                    │          │
│          ▼                   ▼                    ▼          │
│   ┌──────────────────────────────────────────────────────┐  │
│   │              Promos & Bonus Rewards                   │  │
│   │    GoBoxes, referrals, VIP, raffles, bounties         │  │
│   └──────────────────────────────────────────────────────┘  │
│                                                              │
└─────────────────────────────────────────────────────────────┘
```

---

## References

- [Live Market Data](references/LIVE-MARKET-DATA.md) — Current prices, rates, and where to find real-time values
- [Token Use Cases](references/TOKEN-USE-CASES.md) — Detailed token utility breakdown
- [Supported Blockchains](references/SUPPORTED-BLOCKCHAINS.md) — Blockchain networks and compatibility
- [Help Resources](references/HELP-RESOURCES.md) — FAQ sites and support channels
- [FAQ: About GoMining](references/ABOUT.md) — What GoMining is, its mission, and core products
- [FAQ: Getting Started](references/GETTING-STARTED.md) — How to begin using the GoMining platform
- [FAQ: Use Cases](references/USE-CASES.md) — Practical use cases for digital miners and the ecosystem
- [FAQ: General FAQ](references/FAQ.md) — General frequently asked questions about GoMining
- [FAQ: Infrastructure Overview](references/INFRASTRUCTURE.md) — Overview of GoMining's data center and mining infrastructure
- [FAQ: Environmental Friendliness](references/INFRASTRUCTURE-ENVIRONMENT.md) — GoMining's approach to energy and the environment
- [FAQ: Technical Equipment](references/INFRASTRUCTURE-EQUIPMENT.md) — Hardware and technical infrastructure details
- [App Navigation](references/APP-NAVIGATION.md) — Section names and paths for all main app areas

For security and compliance topics — identity verification (KYC Basic vs KYC Advanced), AML, taxes, and account security — see the [gomining-security skill](../gomining-security/SKILL.md).
