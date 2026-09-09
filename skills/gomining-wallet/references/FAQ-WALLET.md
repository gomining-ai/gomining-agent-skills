# Wallet FAQ

### What is a GoMining wallet?

The GoMining wallet is your all-in-one crypto wallet for interacting with the GoMining ecosystem. It allows you to store assets, receive rewards, pay for features, manage digital miners, and more.

### How do deposits and withdrawals work?

Each asset has fixed deposit addresses for each supported blockchain network. You can use these addresses at any time to top up your wallet.

Currently supported assets and networks:

| Asset          | Networks                                                     |
| -------------- | ------------------------------------------------------------ |
| GOMINING token | Ethereum, BNB Smart Chain (BSC), TON, Solana                 |
| BTC            | Bitcoin network                                              |
| USDT           | Ethereum, BNB Smart Chain (BSC), Tron, Solana, TON, Arbitrum |
| USDC           | Ethereum, BNB Smart Chain (BSC), Base, Arbitrum              |
| BNB            | BNB Smart Chain (BSC)                                        |
| ETH            | Ethereum, Base                                               |
| SOL            | Solana                                                       |
| TON            | TON                                                          |

After deposit, your balance is available for withdrawal through any of the supported networks for that asset. This lets you deposit through one network and withdraw through another. For example, deposit GOMINING on BSC, withdraw on Ethereum.

> **Minimum Deposit Amounts**
>
> If you send less than the minimum amount **in a single transaction**, your funds will be lost and cannot be recovered. Make sure your deposit meets the following minimums per transaction:
>
> * GOMINING — 1
> * USDC — 1
> * USDT — 1
> * BTC — 0.00001
> * BNB — 0.001
> * ETH — 0.0005
> * SOL — 0.01
> * TON — 0.1

Deposits are credited after the required number of network confirmations is reached:

| Asset    | Network   | Confirmations |
| -------- | --------- | ------------- |
| GOMINING | BNB Chain | 30            |
| GOMINING | Ethereum  | 34            |
| GOMINING | TON       | 1             |
| GOMINING | Solana    | 1             |
| BTC      | Bitcoin   | 2             |
| USDT     | BNB Chain | 30            |
| USDT     | Ethereum  | 34            |
| USDT     | Tron      | 20            |
| USDT     | Solana    | 1             |
| USDT     | TON       | 1             |
| USDT     | Arbitrum  | 30            |
| USDC     | BNB Chain | 30            |
| USDC     | Ethereum  | 34            |
| USDC     | Arbitrum  | 30            |
| USDC     | Base      | 30            |
| BNB      | BNB Chain | 30            |
| ETH      | Ethereum  | 34            |
| ETH      | Base      | 30            |
| SOL      | Solana    | 1             |
| TON      | TON       | 1             |

Withdrawals also require network confirmations. The required number depends on the receiving wallet. For more information, check the info in your external wallet.

---

### Are my deposit addresses fixed?

Yes. You get a unique, permanent deposit address for each asset on each supported network.

For example:

* Your BTC deposit address will always stay the same
* Your GOMINING deposit address in Ethereum, BSC, TON, or Solana won't change

You can safely reuse them any time you want to top up your wallet. However, there are a couple of exceptions when your address may change:

> **After completing KYC**
>
> If you're an EEA resident, your deposit addresses may change after completing KYC due to legal requirements. You'll need to generate new deposit addresses — you'll see a prompt in your GoMining wallet when it's required.
>
> **After sending a high-risk deposit**
>
> If you send a deposit to your GoMining wallet and our AML system classifies this transaction as high-risk, your deposit addresses in that network will become invalid. You'll need to confirm the source of funds for all your blocked transactions. Once completed, you'll be able to generate new deposit addresses in your GoMining wallet.

---

### What can I do with my GoMining wallet?

The wallet is designed for everyday use in the GoMining ecosystem. With it, you can:

* Store and manage GOMINING tokens, BTC, USDT, USDC, and other assets
* Buy and store digital miners
* Receive BTC rewards from your miners
* Receive rewards in GOMINING tokens
* Pay for purchases or upgrades in the app
* Get veGOMINING votes and participate in governance
* And more — as the platform grows

---

### Are there any fees?

* GoMining does not charge fees for deposits
* Withdrawals may include a network fee, which is shown at the time of the transaction

---

### How can I convert assets? Where is the Convert button?

The **Convert** option lets you exchange one cryptocurrency for another directly inside your GoMining wallet. Conversions are processed in real time, so you receive the new asset instantly without leaving the app.

You can convert any combination of **BTC, ETH, USDT, USDC, BNB, SOL, TON, and GOMINING tokens**. Conversions **from the GOMINING token** to other assets are limited to **30,000 GOMINING per day**.

**How to convert (step by step):**

1. Go to the **Wallet** section.
2. Click **More (three dots) → Convert**. In the **mobile app**, **Convert** is one of the four buttons right on the Wallet screen (**Top up**, **Convert**, **Instant Funds**, **Withdraw**) — no "more" menu needed.
3. Choose the cryptocurrency you want to give and the one you want to receive.
4. Enter the amount you want to swap.
5. Check the exchange rate, conversion fee, and the final amount you'll receive. If the price changes before you confirm, you'll see a slippage warning.
6. Click **Confirm** — when the progress finishes, your balances update right away.

---

### Is there a fee for converting assets in my wallet?

Yes. In-wallet conversions carry a **2% fee**, and it is **already included in the quote** — the "You receive" amount shown on the Convert screen is the net amount after the fee (the screen labels it "2% fee (Incl.)"). There is no separate charge added on top, and this is distinct from network/withdrawal fees. The exact fee and final amount are always shown on the Convert screen before you confirm, so you can review them there.

---

### Can I export my Wallet transaction history (for taxes, accounting, records)?

**There is no built-in export for Wallet transaction history in the GoMining app.** Deposits, withdrawals, conversions, and other Virtual Wallet movements are visible in-app via **Wallet → Recent transactions → "All transactions"** (with filters), but there is **no CSV / PDF / XLSX export button** on that view. Do not tell users to look for one — it doesn't exist.

This is a hard gap between products: **mining rewards** have a documented CSV export (**Rewards → Export CSV**, emailed to the profile address, max 365 days per report). **Wallet transactions do not.** If a user asks for a Wallet export for taxes / accounting / records, contact GoMining support so support can arrange the data or advise a workaround — do not send them to look for an export button that isn't there, and don't invent a path.

For the user's own visibility, in the meantime, they can view (but not export) each transaction row inside the app: Wallet → All transactions, apply the Type / Direction / Asset / Date filters they need. If tax reporting is the goal, the assistant should proactively escalate on the export gap rather than only pointing to the in-app viewer.

---

### Can I set up automatic conversion — e.g. auto-convert BTC to USDC on receipt?

**In-wallet Convert is manual only.** There is no scheduled, recurring, or on-receipt auto-conversion in the wallet — every Convert has to be confirmed on the Convert screen each time. So a rule like "any BTC that arrives → convert to USDC" doesn't exist as a wallet setting.

The **one auto-conversion path GoMining does have** is **Reinvestment** (in **Mining Farm → Settings → Reinvestment**): it automatically converts your **BTC mining rewards** into either **GOMINING tokens (GMT)** or **TH (mining power)** on receipt. It is limited to those two destinations — Reinvestment cannot auto-convert to USDC, USDT, or any other asset. So if the user's underlying goal is "turn mining rewards into a stablecoin automatically", the honest answer is that this isn't supported today; the closest available option is either (a) Reinvestment → GMT, then manual Convert to USDC when they want to, or (b) manual Convert on the Wallet screen each time a reward arrives.

Do **not** invent a scheduled-convert setting, do **not** point users to third-party bots for it, and do **not** claim it is "on the roadmap" — no such feature or timeline is documented. State the situation and the closest available option, and if the user wants to raise a feature request, offer to connect them with GoMining support.

---

### USDT in the EEA

For users in the **EEA**, **USDT is being removed** — **USDC remains fully available**. If you're in the EEA:

- You can **no longer deposit or buy USDT**.
- If you still hold a USDT balance, you can **withdraw it**, and you can **convert it to other assets** — including a **1:1 Convert to USDC**. You **cannot convert *into* USDT** (conversions work only *from* USDT).
- **USDC** works as normal for deposits, purchases, and conversions.

This applies to EEA users only; outside the EEA, USDT is unchanged.

---

### Can I use my GoMining deposit address to receive NFTs (digital miners)?

No. Standard GoMining deposit addresses (used for BTC, USDT, and other tokens) do not support NFT transfers. Attempting to send digital miners to a deposit address will result in loss of the asset.

---

### I log in with Google/Apple/Facebook but want to set a password. Can I do that?

Yes. Go to **Profile → Change password**. If you do not have a password yet, the system will prompt you to create one.
