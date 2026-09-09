# Travel Rule

## What the Travel Rule is

The **Travel Rule** is an international regulatory requirement applied under the **Markets in Crypto-Assets Regulation (MiCA)** and the **Transfer of Funds Regulation (TFR)**. It obliges crypto platforms (VASPs) to collect and share information about the sender and recipient when crypto is transferred to or from an external address, to increase transparency and help prevent money laundering and fraud.

---

## Who it applies to

The Travel Rule is **no longer EEA-only**. It applies to:

- **EEA users** — on external transfers in **both directions** (deposits and withdrawals), regardless of amount.
- **US users** — on **deposits above $3,000** (this threshold applies to US users specifically; it is shown as an embedded verification step).

Do **not** tell a non-EEA user that a Travel Rule / verification form "shouldn't happen" or is an error — a **US user** can legitimately receive it on a deposit over **$3,000**. Users in other regions are generally not asked for Travel Rule details.

For EEA users it applies in **both directions**:

- **Deposits** - you may be asked to identify the **sender** of an incoming transfer.
- **Withdrawals** - you may be asked to identify the **recipient** before the withdrawal can be sent.

**Deposits - 24-hour window:** when the sender needs to be identified for an incoming transfer, you have **24 hours** to verify the sender. If the sender is not verified within that time, the deposit is **not credited** - contact support to arrange a return of the funds.

---

## Information requested

| Step | Field | Details |
|------|-------|---------|
| 1 | **Who owns the wallet** | **Me (self-transfer)** — your own wallet; or **Other person or company** — a third party |
| 2 | **Recipient** (only if *Other person or company*) | **Individual:** full name, country, city, address line 1, address line 2 (optional). **Company:** company name, registration number (optional), country (optional) |
| 3 | **Wallet type** | **Custodial** (exchange/VASP, e.g., Binance) or **Non-custodial** (self-hosted, e.g., MetaMask) |
| 4 | **Provider / self-confirmation** | *Custodial:* select the provider (exchange) from the list. *Non-custodial to your own wallet:* self-confirm ownership. *Non-custodial to someone else:* no provider — recipient is identified via step 2 details |
| 5 | **Consent** | Agree to share recipient details to meet MiCA / TFR requirements before sending |

> **Why the recipient's address is requested:** the Travel Rule requires the recipient of a transfer to be identified, so the address used during their KYC may be requested. This identifies the recipient — it is not the wallet address itself (the wallet address is captured separately).

---

## After submitting

The details are submitted for compliance verification. While this runs, the withdrawal amount is **temporarily locked** on the balance.

- If verification **passes**, the withdrawal is executed.
- If it does **not** pass, the withdrawal is cancelled and the funds are returned to the balance.

Verification usually takes a few seconds, but may take up to a few minutes in some cases.

---

## One withdrawal at a time

Only one withdrawal can be processed at a time. After submitting a withdrawal, the user must wait until it is fully processed (successfully or cancelled) before starting a new one.

---

## Hosted vs unhosted (quick guidance)

- **Hosted (custodial)** — a wallet on a centralized exchange or service that holds funds for the user. Examples: Binance, Coinbase, Kraken, Bitstamp, Bybit.
- **Unhosted (non-custodial)** — a wallet where the user (or recipient) personally holds the private keys. Examples: MetaMask, Trust Wallet, Ledger, Trezor, paper wallet.
- If unsure: logging in to a website to access the wallet usually means hosted; using a browser extension / mobile app with a seed phrase usually means unhosted.

**Choosing the VASP:** search the provider by exact name. If multiple similar names appear (e.g., regional variants), choose the one matching the service actually used. If the VASP is not in the list, contact support — it may be possible to add it, or the destination may not be supported.

---

## Common scenarios

| Scenario | Who owns | Wallet type | Provider / detail |
|----------|----------|-------------|-------------------|
| Own Binance / Bybit / Coinbase / Kraken account | Me | Custodial | Select the exchange |
| Own MetaMask / Trust Wallet / Ledger / Trezor | Me | Non-custodial | Confirm ownership; no provider |
| Another person's exchange account | Other person | Custodial | Recipient details (Individual) + select exchange |
| Another person's personal wallet | Other person | Non-custodial | Recipient details (Individual); no provider |
| A company (e.g., paying an invoice) | Other person/company | Custodial or Non-custodial | Company details; if custodial, select provider |

---

## Common questions

**Whose name should I enter?** Only when sending to another person or company. Enter the recipient's full name exactly as it appears on the receiving wallet or account — it does not need to match your GoMining name. No name is requested for self-transfers.

**What address should I enter?** Only when sending to another person or company. Enter the recipient's residential address, typically the one used during their KYC on the receiving service. No address is requested for self-transfers.

**What if I make a mistake?** If verification doesn't pass, the withdrawal is cancelled and funds are returned. Double-check the recipient's name and details before submitting.
