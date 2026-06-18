---
name: gomining-security
description: "GoMining security & compliance — identity verification, AML, taxes, and account safety. Covers KYC with a clear distinction between Level 1 (identity only: passport, national ID, residence card, or driver's license) and Level 2 (additional compliance for the Visa card), accepted documents, prohibited jurisdictions, AML transaction monitoring and blocked funds, tax/reporting responsibilities, and general account/wallet security."
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
  triggers:
    - "kyc"
    - "identity verification"
    - "verify my identity"
    - "what documents for kyc"
    - "kyc level 1 vs level 2"
    - "aml"
    - "funds blocked"
    - "taxes"
    - "account security"
---

# GoMining Security & Compliance

GoMining applies industry-standard security and compliance practices to protect user accounts, funds, and operations. This skill covers how the platform is secured, what identity verification is required and why, how transactions are monitored, and how taxes are handled.

---

## KYC: the most important rule

Identity verification has **two levels with different rules**. Before answering any question about identity verification, supported documents, eligibility, or country restrictions, **determine which level applies** — and never apply one level's restrictions to the other.

| | **KYC Level 1** | **KYC Level 2** |
|---|---|---|
| **Checks** | Identity only (document + selfie) | Identity **plus** email, phone, tax info, proof of address, financial questionnaire |
| **Accepted ID** | Passport, national ID, residence card, **driver's license** | Passport, national ID (varies by country); **no driver's license** |
| **Required for** | Withdraw tokens, unlock BTC withdrawals, mint/sell miners, access Launchpad | Issuing a GoMining Visa card |
| **Availability** | All countries except prohibited jurisdictions | Country-specific compliance |

**Quick answer to "Can I verify without a passport?"** → For **Level 1**, yes: a national ID, residence card, or driver's license all work. A passport is not mandatory.

Full rules, document lists, prohibited jurisdictions, step-by-step flows, and answering do's/don'ts are in [references/KYC.md](references/KYC.md).

---

## In this skill

| Topic | Reference | Covers |
|-------|-----------|--------|
| Identity Verification (KYC) | [references/KYC.md](references/KYC.md) | KYC Level 1 vs Level 2, accepted documents, prohibited jurisdictions, verification steps |
| Anti-Money Laundering (AML) | [references/AML.md](references/AML.md) | Transaction monitoring, blocked/withheld funds, source-of-funds documents, refunds |
| Taxes & Reporting | [references/TAXES.md](references/TAXES.md) | Tax responsibility, what determines taxation, reporting to authorities |
| General Security | [references/GENERAL.md](references/GENERAL.md) | Equipment uptime, wallet/contract ownership, verifying miner authenticity |
| Security Overview | [references/OVERVIEW.md](references/OVERVIEW.md) | High-level summary of all security areas |

---

## Related skills

- **GoMining Card** — card-specific KYC Level 2 details (regional eligibility, document tables, passport restrictions for Belarus/Russia): [gomining-card skill](../gomining-card/SKILL.md)
- **Payments** — KYC/AML in the context of buying crypto and miners: [gomining-payments skill](../gomining-payments/SKILL.md)
- **Platform Overview** — ecosystem basics: [gomining-overview skill](../gomining-overview/SKILL.md)
