# GoMining Agent Skills

This directory contains agent skills for the GoMining ecosystem. Each skill provides structured knowledge about a specific aspect of the platform.

## Available Skills

### Core Platform

| Skill | Description | Use When |
|-------|-------------|----------|
| [`gomining-overview`](gomining-overview/SKILL.md) | Platform introduction and ecosystem basics | User asks "What is GoMining?" or needs general orientation |
| [`gomining-miners`](gomining-miners/SKILL.md) | Digital Miners, mining modes, Miner Wars | User asks about miners, mining rewards, or Miner Wars |
| [`gomining-avatars`](gomining-avatars/SKILL.md) | Avatar collections, Luminars, marketplace, merch | User asks about avatars, Luminars, or merch |
| [`gomining-nft`](gomining-nft/SKILL.md) | NFT technical details, blockchains, rarity | User asks about NFT specs, blockchain networks, or rarity |
| [`gomining-vip`](gomining-vip/SKILL.md) | VIP tiers, thresholds, benefits | User asks about VIP levels, maintenance discounts, or perks |

### Token & Economics

| Skill | Description | Use When |
|-------|-------------|----------|
| [`gomining-token`](gomining-token/SKILL.md) | GOMINING token utility and use cases | User asks about token usage, discounts, or rewards |
| [`gomining-tokenomics`](gomining-tokenomics/SKILL.md) | Token economics, locking, voting, burn/mint | User asks about veGOMINING, epochs, supply, or voting |

### Financial Products

| Skill | Description | Use When |
|-------|-------------|----------|
| [`gomining-wallet`](gomining-wallet/SKILL.md) | Crypto wallet, assets, deposits, withdrawals | User asks about wallet, supported assets, or transfer limits |
| [`gomining-simple-earn`](gomining-simple-earn/SKILL.md) | Passive BTC yield on crypto balances | User asks about earning interest or Simple Earn |
| [`gomining-card`](gomining-card/SKILL.md) | GoMining Visa debit card | User asks about crypto card, payments, or card KYC |
| [`gomining-payments`](gomining-payments/SKILL.md) | Payment methods, Open Banking, MNPL, KYC | User asks about buying crypto, installments, or KYC/AML |

### Growth & Engagement

| Skill | Description | Use When |
|-------|-------------|----------|
| [`gomining-cashback`](gomining-cashback/SKILL.md) | TH/s cashback from Cards and Travel | User asks about cashback rates or mining power rewards |
| [`gomining-travel`](gomining-travel/SKILL.md) | Hotel booking with GM tokens, travel cashback | User asks about travel, hotel booking, or travel cashback |
| [`gomining-promos`](gomining-promos/SKILL.md) | Promo codes, GoBoxes, referrals, bonus system | User asks about promo codes, referrals, or GoBoxes |
| [`gomining-academy`](gomining-academy/SKILL.md) | Educational platform and courses | User wants to learn or asks about courses/articles |

### Guides

| Skill | Description | Use When |
|-------|-------------|----------|
| [`gomining-investment-guide`](gomining-investment-guide/SKILL.md) | Budget-tier recommendations, ROI, optimization | User asks "What can I do with $X?" or needs investment strategy |

## Skill Selection Guide

```
User Question                              Recommended Skill
─────────────────────────────────────────────────────────────
"What is GoMining?"                    →   gomining-overview
"How do Digital Miners work?"          →   gomining-miners
"How do I buy a miner?"               →   gomining-miners
"What are Miner Wars?"                →   gomining-miners
"What are avatar collections?"         →   gomining-avatars
"What are Luminars?"                   →   gomining-avatars
"What blockchains are supported?"      →   gomining-nft
"What are the VIP tiers?"             →   gomining-vip
"What discounts can I get?"            →   gomining-vip
"How do I use GOMINING tokens?"        →   gomining-token
"How does token burning work?"         →   gomining-tokenomics
"What is veGOMINING?"                  →   gomining-tokenomics
"How do I deposit crypto?"             →   gomining-wallet
"What assets are supported?"           →   gomining-wallet
"How do I get a crypto card?"          →   gomining-card
"How can I earn passive income?"       →   gomining-simple-earn
"What are the APR rates?"             →   gomining-simple-earn
"How do I buy crypto?"                →   gomining-payments
"Can I pay in installments?"           →   gomining-payments
"What are cashback rates?"             →   gomining-cashback
"Can I book hotels with crypto?"       →   gomining-travel
"How do promo codes work?"             →   gomining-promos
"What is a GoBox?"                     →   gomining-promos
"Where can I learn about mining?"      →   gomining-academy
"What can I do with $1000?"           →   gomining-investment-guide
"How do I maximize returns?"          →   gomining-investment-guide
"What's the best investment strategy?" →   gomining-investment-guide
```

## Skill Structure

Each skill follows the [Agent Skills specification](https://agentskills.io):

```
skill-name/
├── SKILL.md           # Main skill file with YAML frontmatter
├── skill.json         # Metadata, triggers, and type
└── references/        # Supporting documentation
    ├── FAQ-TOPIC.md   # Frequently asked questions
    ├── INSTRUCTION-X.md  # Step-by-step guides
    └── TOPIC.md       # Deep-dive references
```

## Quick Reference

### Official Resources

| Resource | URL |
|----------|-----|
| Main Website | https://gomining.com/ |
| Alternative | https://gmt.io/en |
| Academy | https://academy.gomining.com/ |
| Token FAQ | https://help.token.gomining.com/ |
| NFT FAQ | https://help.nft.gomining.com/ |
| Card FAQ | https://help.cards.gomining.com/ |

### Key Concepts

| Term | Definition |
|------|------------|
| GOMINING | Native utility token of the ecosystem |
| Digital Miners | NFTs representing Bitcoin mining power |
| BMINE | Issuer of Digital Miners NFT collections |
| veGOMINING | Vote-escrowed governance token (locked GOMINING) |
| Simple Earn | Yield-generating product for crypto holdings |
| Miner Wars | Competitive game mode for earning BTC |
| TH/s | Terahashes per second — unit of mining power |
| GoBox | Digital loot box with random prizes |
| MNPL | Mine Now, Pay Later — 0% installment plans for miners |
| Avatars | Cosmetic NFTs assignable to Digital Miners |
| Luminars | Avatar collection with VIP level boost properties |
