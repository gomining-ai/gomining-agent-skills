# Frequently Asked Questions

Common questions about GoMining products and services.

## General

**What is GoMining?**
GoMining is a platform that lets you mine Bitcoin by owning digital miners, digital representations of real mining hardware. You earn daily BTC rewards based on your miner's hashrate and energy efficiency without managing physical equipment.

**What guarantees that the equipment won't be disconnected?**
GoMining uses industrial power grids and its own substations with backup connections, guaranteeing uninterrupted operation of all equipment at our data centers.

**What happens if GoMining shuts down? / Is GoMining a long-term project?**
GoMining is not a short-term project or a simulation of mining. The platform is built on real mining infrastructure and operates in accordance with its publicly available Terms of Use and legal documentation. Users retain ownership of their digital assets and can manage them in line with the platform's rules and available features. GoMining continuously invests in the development and long-term operation of the ecosystem.

> This is the reassurance/continuity answer for general "what if GoMining shuts down / closes / is it here to stay" questions. A question about **legal proceedings, insolvency/bankruptcy specifics, or a user's creditor rights** ("if GoMining goes bankrupt, what's my legal claim?") is a legal-interpretation question — escalate that to a human instead.

**Who owns the main wallet and smart contract?**
The main wallet and smart contract belong to GoMining. All transactions are verifiable on-chain and our smart contracts are publicly auditable.

**How can I verify the authenticity of a digital miner?**
Purchase miners directly in your GoMining personal account. If buying on third-party marketplaces (e.g. GetGems), always verify the network and smart contract address matches GoMining's official contracts.

**Can I change the display or account currency (e.g. to GBP or EUR)?**
No. There is no setting to change the currency in which values are displayed in the GoMining app — it cannot be switched to GBP or another currency.

**How do I connect an AI assistant / MCP to my GoMining account?**
GoMining exposes an **MCP Server** so AI assistants can read your account data (balances, miners, earnings, etc.) in natural language. The connection is **read-only** — the assistant can view your data but cannot make changes. First sign in to your GoMining account at app.gomining.com, then add a custom connector in your AI tool:
- **Claude (web or desktop):** Customize → **Connectors** → **+** → add a custom connector named **GoMining** with URL **https://mcp.gomining.com/mcp** → Connect and authorize access.
- **Other MCP-compatible tools:** add **https://mcp.gomining.com/mcp** as a remote MCP server in the tool's settings.

Do **not** invent an in-app "generate MCP token / API key" flow under Profile Settings — connection is done through the AI tool's connector settings using the URL above.

## GoMining Card

**Why does the ATM show a €0 balance for my GoMining Card?**
ATMs always show **€0** because GoMining Cards do not support balance inquiries via ATM systems. Your actual balance is managed inside the GoMining ecosystem and depends on your allocated crypto and real-time conversion rates. To check your balance, open the **GoMining app**.

**Why was my card issuance declined?**
The card provider may decline your request if it does not pass their internal checks. If this happens, the card cannot be reissued for the same account. Please contact support for more information.

**My balance went negative after a purchase. Why?**
This happens due to exchange rate fluctuations between the time your payment is **authorized** (hold placed) and **settled** (charge finalized). If the rate moves unfavorably, the final charge may exceed the initial amount. Add funds to your account to restore a positive balance.

**What cryptocurrencies can I spend with my GoMining Card?**
You can choose which asset is used for payments: **GOMINING**, **BTC**, **USDT**, or **USDC**. Conversion to fiat happens instantly at the current exchange rate at the moment of each transaction.

**How many virtual GoMining Cards can I have?**
You can have up to **3 virtual GoMining Card** at a time. Physical cards will be available in a future release.

## Security & KYC

**What KYC level do I need to use GoMining Cards?**
Both **KYC Basic** and **KYC Advanced** are required to issue and use GoMining Cards. Identity verification is mandatory for regulatory compliance.

**How do I verify a GoMining representative?**
GoMining representatives will never ask for your password. To verify someone claiming to be from GoMining, check the official support channels listed on gomining.com and never share sensitive credentials.

**What is GoMining's AML policy?**
GoMining follows strict Anti-Money Laundering procedures in compliance with international standards. All users must complete identity verification before accessing financial features. Prohibited jurisdictions include countries under international sanctions.

## GOMINING Token

**What is the GOMINING token used for?**
The GOMINING token powers the GoMining ecosystem: it can be locked to receive **veGOMINING** votes (which grant governance rights and weekly rewards), used to pay for miner maintenance with up to a 20% discount, and traded on supported exchanges.

**How does veGOMINING voting work?**
Lock your GOMINING tokens to receive **veGOMINING** (vote-escrow GOMINING). The longer you lock, the more voting power you receive. Use veGOMINING to vote on protocol proposals and ecosystem decisions.

**What are tokenomics epochs and burn mechanics?**
GOMINING uses a periodic epoch system where token emissions are adjusted based on ecosystem activity. A portion of platform fees is used to buy back and burn GOMINING tokens, creating deflationary pressure over time.
