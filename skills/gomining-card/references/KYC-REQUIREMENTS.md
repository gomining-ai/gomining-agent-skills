# KYC Requirements for GoMining Card

Issuing a **GoMining Card** requires **KYC Advanced** — the platform's full compliance verification.

To check whether a card is available for a given region, point the user to the eligibility section of the docs: https://docs.gomining.com/en/product/cards/about-the-gomining-card#am-i-eligible

> **USA / US card questions:** Do **not** confirm or deny whether cards are available in the USA — do not state, imply, or hint at either. Give a neutral response and direct the user to self-check eligibility at the link above, e.g. "Please check card availability for your region here: https://docs.gomining.com/en/product/cards/about-the-gomining-card#am-i-eligible".

> **Terminology:** "KYC Basic" and "KYC Advanced" below are the platform-wide KYC levels.
> They were previously called "KYC Level 1" and "KYC Level 2" - if a user says "Level 1" or
> "Level 2", they mean Basic and Advanced respectively.
> **KYC Basic** is the basic identity check (passport, national ID, residence card, or
> driver's license) used to withdraw tokens, mint/sell miners, and access Launchpad — it does
> **not** issue a card. The card requires **KYC Advanced**, which adds the compliance checks
> below. Full level definitions are in the [gomining-security skill](../../gomining-security/references/KYC.md).

## What KYC Advanced Covers (required for the card)

| Component | Description |
|-----------|-------------|
| Identity | Valid national passport or national ID card + selfie (liveness check) |
| Proof of address | Document dated within 3 months; address must match the ID document or be separately verified |
| Additional compliance | Email verification, phone verification, tax information, financial questionnaire |

A **driver's license is not accepted** for KYC Advanced identity verification.

> **US residents — KYC Advanced is passport-only.** When a US applicant selects **United States of America** in the KYC Advanced verification flow, the app offers **only Passport** — US state IDs and US driver's licenses are **not** accepted at KYC Advanced (they are accepted at KYC Basic, but KYC Basic does **not** issue a card). Do not tell US card applicants that state IDs are accepted; they are not. This is current policy, not a bug — if the user asks whether the app is broken because they only see passport, reassure them it is intentional. If they don't have a US passport, they cannot complete KYC Advanced today; offer to connect them with GoMining support if they want to raise a feedback request or ask about alternatives.

## Document Requirements

### Accepted Identity Documents

| Document | European Residents | Global Residents |
|----------|-------------------|------------------|
| National Passport | Yes | Yes (where supported) |
| National ID Card | Yes | Yes (where supported) |
| Driver's License | **No** | **No** |
| Residence Permit | No* | No* |

*Exception: Residence permits accepted for non-European citizens residing in Europe

### Proof of Address Documents

| Document Type | Accepted | Requirements |
|---------------|----------|--------------|
| Utility Bill | Yes | Dated within 3 months |
| Bank Statement | Yes | Dated within 3 months |
| Government Letter | Yes | Dated within 3 months |
| Tax Document | Yes | Current year |

## Regional Requirements

### European Residents (EEA+)
- Valid passport or ID card from EEA+ country
- Proof of address under 3 months old
- Both documents from same or different countries accepted

### Global Residents
- Valid passport or ID card (where supported)
- Proof of address from non-prohibited jurisdiction
- Identity and address documents can be from different countries

## Restrictions

### Passport Restrictions
- Certain nations' passports are not accepted
- Belarus passport holders: Must provide valid EEA+ residence permit
- Russian passport holders: Must provide valid EEA+ residence permit

### Prohibited Jurisdictions
60+ countries where card applications are not available. Check the [Supported Regions](SUPPORTED-REGIONS.md) reference for the complete list.

Users can self-check regional eligibility at https://docs.gomining.com/en/product/cards/about-the-gomining-card#am-i-eligible

## Will the accepted documents change? (roadmap / feedback questions)

If a user asks whether GoMining plans to relax KYC requirements — for example, to accept a **driver's license or US state ID** instead of a passport or national ID:

- State the **current** policy plainly: only a valid national passport or national ID card is accepted for KYC Advanced; a driver's license or state ID is **not** accepted.
- Do **not** promise or speculate about future changes. **No changes have been announced.**
- Close softly by inviting the user to share the request with the GoMining support team, who can pass feedback to the product team — e.g. "If you'd like to see this changed, you can share that feedback with our support team." Offer to connect them with GoMining support only if the user actually wants to submit the feedback; otherwise just offer it.
