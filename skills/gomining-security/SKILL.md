---
name: gomining-security
description: "GoMining security & compliance — identity verification, AML, the Travel Rule, taxes, and account safety. Covers KYC with a clear distinction between KYC Basic (identity only: passport, national ID, residence card, or driver's license) and KYC Advanced (additional compliance for the Visa card), including the former Level 1 / Level 2 names users still use, accepted documents, prohibited jurisdictions, AML transaction monitoring and blocked funds, the MiCA/TFR Travel Rule for EEA users on both deposits and withdrawals to/from external wallets, tax/reporting responsibilities, general account/wallet security, and Security Mode — a 12-hour hold on withdrawals and miner sales that starts automatically after an email / password / 2FA-disable change (everything else keeps working; support can lift early)."
license: Apache-2.0
compatibility: "Compatible with Claude Code, Codex, and all Agent Skills spec tools."
metadata:
  author: gomining
  version: "1.0"
  tags:
    - security
    - kyc
    - compliance
    - aml
    - taxes
    - identity-verification
    - security-mode
    - account-hold
  triggers:
    - "kyc"
    - "identity verification"
    - "verify my identity"
    - "what documents for kyc"
    - "kyc basic vs kyc advanced"
    - "kyc level 1 vs level 2"
    - "aml"
    - "funds blocked"
    - "travel rule"
    - "recipient details for withdrawal"
    - "withdrawal to external wallet"
    - "taxes"
    - "account security"
    - "security mode"
    - "your account is in security mode"
    - "why can't i withdraw"
    - "why can't i sell my miner"
    - "12 hour hold"
    - "12-hour hold"
    - "changed my password"
    - "changed my email"
    - "disabled 2fa"
    - "disabled two-factor"
---

# GoMining Security & Compliance

GoMining applies industry-standard security and compliance practices to protect user accounts, funds, and operations. This skill covers how the platform is secured, what identity verification is required and why, how transactions are monitored, and how taxes are handled.

---

## KYC: the most important rule

Identity verification has **two levels with different rules**. Before answering any question about identity verification, supported documents, eligibility, or country restrictions, **determine which level applies** — and never apply one level's restrictions to the other.

The two levels are **KYC Basic** and **KYC Advanced**. They were previously called **KYC Level 1** and **KYC Level 2**; users and older help articles still use the old names. Map "Level 1" to KYC Basic and "Level 2" to KYC Advanced, and reply using the new names.

| | **KYC Basic** | **KYC Advanced** |
|---|---|---|
| **Checks** | Identity only (document + selfie) | Identity **plus** email, phone, tax info, proof of address, financial questionnaire |
| **Accepted ID** | Passport, national ID, residence card, **driver's license** | Passport, national ID (varies by country); **no driver's license** |
| **Required for** | Withdraw tokens, unlock BTC withdrawals, mint/sell miners, access Launchpad | Issuing a GoMining Visa card |
| **Availability** | All countries except prohibited jurisdictions | Country-specific compliance |

**Quick answer to "Can I verify without a passport?"** → For **KYC Basic**, yes: a national ID, residence card, or driver's license all work. A passport is not mandatory.

**Russia & Belarus:** **KYC Basic** will **not be confirmed** for users in Russia or Belarus.

Full rules, document lists, prohibited jurisdictions, step-by-step flows, and answering do's/don'ts are in [references/KYC.md](references/KYC.md).

---

## Is GoMining licensed? (MiCA / regulated crypto services)

For questions about GoMining's MiCA licensing or who provides its regulated crypto services in the EU, give this documented answer. **Keep the entity names and licence numbers exact**:

> Regulated crypto services for EU users are provided through a licensed partner, **Noemon Finance Limited**, authorized by **CySEC (Cyprus) under MiCA, CIF licence No. 449/24**. The company is also on the **AMF (France) whitelist** and operates across EU member states, including France, via **MiCA passporting**. Additionally, **Noemon Tech Limited** is registered with **CySEC as a CASP, registration No. 014/24**. These details can be verified directly in the **CySEC and AMF registers**. Up-to-date information on the company's own licences and on its partners' licences and permissions is always available in the **Terms of Use** on the official website.

This is a documented factual answer — provide it directly rather than escalating. (Other legal/regulatory *interpretation* questions still go to a human — see the system prompt's legal-questions rule.)

---

## In this skill

| Topic | Reference | Covers |
|-------|-----------|--------|
| Identity Verification (KYC) | [references/KYC.md](references/KYC.md) | KYC Basic vs KYC Advanced, accepted documents, prohibited jurisdictions, verification steps |
| Anti-Money Laundering (AML) | [references/AML.md](references/AML.md) | Transaction monitoring, blocked/withheld funds, source-of-funds documents, refunds |
| Travel Rule | [references/TRAVEL-RULE.md](references/TRAVEL-RULE.md) | MiCA/TFR Travel Rule for EEA users on both deposits (identify sender, 24-hour window) and withdrawals (identify recipient) to/from external wallets - who it applies to, details required, custodial vs non-custodial, verification |
| Taxes & Reporting | [references/TAXES.md](references/TAXES.md) | Tax responsibility, what determines taxation, reporting to authorities |
| General Security | [references/GENERAL.md](references/GENERAL.md) | Equipment uptime, wallet/contract ownership, verifying miner authenticity |
| Security Mode | [references/SECURITY-MODE.md](references/SECURITY-MODE.md) | The 12-hour hold on withdrawals and miner sales after an email / password / 2FA-disable change — what pauses, what keeps working, how to lift it early |
| Security Overview | [references/OVERVIEW.md](references/OVERVIEW.md) | High-level summary of all security areas |

---

## Related skills

- **GoMining Card** — card-specific KYC Advanced details (regional eligibility, document tables, passport restrictions for Belarus/Russia): [gomining-card skill](../gomining-card/SKILL.md)
- **Payments** — KYC/AML in the context of buying crypto and miners: [gomining-payments skill](../gomining-payments/SKILL.md)
- **Platform Overview** — ecosystem basics: [gomining-overview skill](../gomining-overview/SKILL.md)
