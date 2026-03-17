# GoMining Agent Skills

[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE)
[![Agent Skills](https://img.shields.io/badge/Agent%20Skills-v1.0-green.svg)](https://agentskills.io)

Agent skills for **GoMining** — a blockchain platform democratizing Bitcoin mining through Digital Miners NFTs, the GOMINING utility token, crypto-powered Visa cards, DeFi products, and travel integrations.

## Skills

### Core Platform

| Skill | Description | Use When |
|-------|-------------|----------|
| [`gomining-overview`](skills/gomining-overview/SKILL.md) | Platform introduction, ecosystem basics | "What is GoMining?" |
| [`gomining-miners`](skills/gomining-miners/SKILL.md) | Digital Miners, mining modes, Miner Wars | "How do miners work?" |
| [`gomining-avatars`](skills/gomining-avatars/SKILL.md) | Avatar collections, Luminars, merch, marketplace | "What are avatar races?" |
| [`gomining-nft`](skills/gomining-nft/SKILL.md) | NFT technical details, blockchains, rarity | "What blockchains are supported?" |
| [`gomining-vip`](skills/gomining-vip/SKILL.md) | VIP tiers, thresholds, benefits | "What are VIP levels?" |

### Token & Economics

| Skill | Description | Use When |
|-------|-------------|----------|
| [`gomining-token`](skills/gomining-token/SKILL.md) | GOMINING token utility, discounts, rewards | "How do I use tokens?" |
| [`gomining-tokenomics`](skills/gomining-tokenomics/SKILL.md) | Token economics, locking, voting, burn/mint | "What is veGOMINING?" |

### Financial Products

| Skill | Description | Use When |
|-------|-------------|----------|
| [`gomining-wallet`](skills/gomining-wallet/SKILL.md) | Crypto wallet, deposits, withdrawals | "How do I deposit crypto?" |
| [`gomining-simple-earn`](skills/gomining-simple-earn/SKILL.md) | Passive BTC yield on crypto balances | "How can I earn interest?" |
| [`gomining-card`](skills/gomining-card/SKILL.md) | GoMining Visa debit card, KYC | "How do I get a crypto card?" |
| [`gomining-payments`](skills/gomining-payments/SKILL.md) | Payment methods, Open Banking, MNPL, KYC | "How do I buy crypto?" |

### Growth & Engagement

| Skill | Description | Use When |
|-------|-------------|----------|
| [`gomining-cashback`](skills/gomining-cashback/SKILL.md) | TH/s cashback from Cards and Travel | "What are cashback rates?" |
| [`gomining-travel`](skills/gomining-travel/SKILL.md) | Hotel booking with GM tokens, travel cashback | "Can I book hotels with crypto?" |
| [`gomining-promos`](skills/gomining-promos/SKILL.md) | Promo codes, GoBoxes, referrals, bonus system | "How do promo codes work?" |
| [`gomining-academy`](skills/gomining-academy/SKILL.md) | Courses, articles, product guides | "Where can I learn more?" |

### Guides

| Skill | Description | Use When |
|-------|-------------|----------|
| [`gomining-investment-guide`](skills/gomining-investment-guide/SKILL.md) | Budget-tier recommendations, ROI examples, optimization | "What can I do with $100?" |

## Installation

### Claude Code

Load directly from a local clone:

```bash
git clone https://github.com/gomining-ai/gomining-agent-skills.git
cd gomining-agent-skills
claude --plugin-dir ./skills
```

### Any Agent (npx skills)

Install into any supported agent using the [skills CLI](https://github.com/vercel-labs/skills):

```bash
# Install all skills
npx skills add gomining-ai/gomining-agent-skills --all

# Install a specific skill
npx skills add gomining-ai/gomining-agent-skills --skill gomining-token

# Install to a specific agent
npx skills add gomining-ai/gomining-agent-skills -a claude-code --all
```

### Generic Agents (agentskills.io)

Each skill follows the [Agent Skills specification](https://agentskills.io). Skills are in `skills/`, each containing a `SKILL.md` with YAML frontmatter and a `references/` directory with detailed documentation.

### Programmatic Access

The [`skills.json`](skills.json) manifest provides programmatic access to all skills:

```javascript
const manifest = require('./skills.json');
console.log(manifest.skills); // Array of all skills with metadata
```

## Project Structure

```
.
├── LICENSE
├── CONTRIBUTING.md
├── README.md
├── skills.json                    # Skills manifest for programmatic access
├── agents/
│   └── AGENTS.md                  # Agent skills description for LLM agents
└── skills/
    ├── README.md                  # Skills overview and selection guide
    ├── gomining-overview/         # 16 skill directories, each containing:
    ├── gomining-miners/           #   ├── SKILL.md        (main skill file)
    ├── gomining-avatars/          #   ├── skill.json      (metadata & triggers)
    ├── gomining-nft/              #   └── references/     (supporting docs)
    ├── gomining-vip/
    ├── gomining-token/
    ├── gomining-tokenomics/
    ├── gomining-wallet/
    ├── gomining-simple-earn/
    ├── gomining-card/
    ├── gomining-payments/
    ├── gomining-cashback/
    ├── gomining-travel/
    ├── gomining-promos/
    ├── gomining-academy/
    └── gomining-investment-guide/
```

## GoMining Ecosystem Overview

```
┌────────────────────────────────────────────────────────────────────┐
│                        GoMining Ecosystem                          │
├────────────────────────────────────────────────────────────────────┤
│                                                                    │
│  ┌───────────┐  ┌───────────┐  ┌───────────┐  ┌────────────────┐  │
│  │ GOMINING  │  │  Digital  │  │ GoMining  │  │  Wallet &      │  │
│  │  Token    │◄─┤  Miners   ├─►│   Card    │◄─┤  Simple Earn   │  │
│  │           │  │  (NFTs)   │  │  (Visa)   │  │                │  │
│  └─────┬─────┘  └─────┬─────┘  └─────┬─────┘  └───────┬────────┘  │
│        │              │              │                 │            │
│        └──────────────┼──────────────┼─────────────────┘            │
│                       ▼              ▼                              │
│  ┌──────────────────────────────────────────────────────────────┐  │
│  │  VIP • Cashback • Travel • Promos • Academy • Payments      │  │
│  │  Tokenomics (Burn & Mint) • Avatars • Investment Guide      │  │
│  └──────────────────────────────────────────────────────────────┘  │
│                                                                    │
└────────────────────────────────────────────────────────────────────┘
```

## Documentation

| Resource | URL |
|----------|-----|
| Main Website | https://gomining.com/ |
| Academy | https://academy.gomining.com/ |
| Token FAQ | https://help.token.gomining.com/ |
| NFT FAQ | https://help.nft.gomining.com/ |
| Cards FAQ | https://help.cards.gomining.com/ |
| CoinMarketCap | https://coinmarketcap.com/currencies/gomining-token/ |

## Contributing

Contributions are welcome! Please read [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

## License

Apache-2.0 — see [LICENSE](LICENSE) for details.
