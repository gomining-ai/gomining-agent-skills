# Rewards

## Mining Mode

### Where do I find Reward settings?

Reward settings open the same **Settings** panel. Where to find it:

- **Rewards** tab → **Reward settings** button (top-right), or
- **Mining farm** tab → **Settings** (gear icon, top-right of the Mining farm card), or
- on **mobile**: **My Miners → Settings**.

The section **is available on mobile too** — do not tell users it's missing on iOS, and don't send them to "Profile Settings" (that is not where it lives).

The panel contains:

- **Maintenance in GOMINING** — toggle on to pay maintenance with GOMINING tokens for up to a 20% discount; **Increase discount ›** opens the Maintenance discounts page.
- **Reward protection** — protects from negative payouts when the maintenance fee is higher than the reward (in Mining mode it applies per miner; in Miner Wars, to the whole mining farm).
- **Reinvestment** — automatically convert BTC rewards into GOMINING tokens or into TH for one of your miners.
- **Pool** — choose the mining pool (e.g. VIA BTC).

> "Reward settings" is a mining/rewards feature — it is **not** related to the GoMining Card.

### What time of day are rewards added?

This applies to **Mining mode** rewards only. In Mining mode, BTC rewards are credited **once per day**, but there is **no fixed or guaranteed time** — they are added at some point during the day rather than at a set hour. There is no published exact crediting time. If a reward seems to be missing well beyond the usual daily cycle, ask the user for details and escalate rather than quoting a specific time.

**Miner Wars rewards are different — they are weekly, not daily.** They are distributed at the end of each Cycle (Tuesday 00:00 UTC), not during the day. See [Miner Wars Rewards](#miner-wars-rewards) below.

### What time is the daily BTC price taken for the reward calculation?

The BTC price used to value the daily reward is captured **once a day, sometime between 00:00 and 03:00 UTC** (the exact minute within that window isn't fixed). The price source is the **Binance Pool**. So the USD value of a day's reward reflects the BTC price from that early-UTC window, not the price at the moment you view it.

### What do the reward statuses mean (Calculated, Sent, Reinvested, Inactive)?

- **Calculated** — the reward amount has been **confirmed by the system but not yet credited** to your wallet. It's the intermediate state; once credited, the status changes to **Sent**. Do **not** tell a user "Calculated" means the reward is already in their wallet — it isn't yet.
- **Sent** — the reward has been **credited** to your virtual wallet.
- **Reinvested** — instead of being kept as BTC, the reward was automatically converted into **TH (mining power)** or **GOMINING tokens**, per your reinvestment setting; the BTC value was used for that conversion rather than showing as a BTC payout.
- **Inactive / 0 reward** — your maintenance fees equalled or exceeded the pool reward for that day; with Reward Protection you're not charged the difference and both the reward and fee show as 0.

You can see the full per-day breakdown (PR, electricity C1, service C2, discount, net) under **My Miners → Rewards** — tap a payment record, then a specific miner.

---

### What is the "GoBTC Pay reward" line in my Mining Rewards?

The **GoBTC Pay reward** is a **share of the GoBTC Pay payment network's daily volume** paid to miners: **0.1% of the network's daily BTC volume is distributed among all GoMining miners in proportion to their mining power (TH)**. So your amount is proportional to your whole farm's power. It's credited **once a day together with your normal mining reward** and shown as a separate **GoBTC Pay reward** column/line in the Mining Rewards (Reward Digest). Amounts are **small right now and will grow as the payment network's volume grows**.

Key points to avoid confusion:
- This is a **reward for owning miners** (by TH) — it is **not** a fee, and it's separate from your pool reward, electricity (C1), and service (C2) lines.
- You do **not** earn it for *spending/paying* with GoBTC or just for holding a wallet — it's tied to your **mining power**. (The separate wallet-provider revenue share is for platforms that integrate the GoBTC SDK, not individual users — see the GoBTC Pay skill.)

### How do I withdraw my BTC rewards?

All earned BTC rewards are accumulated in your GoMining virtual wallet. You can withdraw them to your external Bitcoin wallet manually at any time.

To enable BTC withdrawals, please ensure you have created at least one miner directly on the GoMining platform. If you only own miners bought on the secondary market or imported from elsewhere, BTC withdrawals will stay unavailable until you create a primary miner through GoMining.

BTC is withdrawn via **Fast withdrawal** — your BTC is transferred within **1 hour**; a **network fee** applies (variable, shown at confirmation) and **KYC verification is required**.

> The fee-free **Standard withdrawal** (within 24 hours, no fee) was **discontinued on July 6, 2026**. BTC withdrawals now use Fast withdrawal only (within 1 hour, variable network fee).

#### What steps should I follow to complete a withdrawal?

1. Go to your virtual wallet and click **Withdraw**.
2. Choose **BTC** and select the **Bitcoin network**.
3. Enter the amount and the recipient wallet address. You can save this address as your default (pre-filled in future withdrawals); you can edit it or set a new default at any time during the withdrawal.
4. Complete two-factor authentication to confirm the withdrawal.

You can view your full withdrawal history and transaction statuses in the virtual wallet.

---

### How to withdraw GOMINING token rewards?

If you choose to withdraw GOMINING tokens from your virtual wallet, you can do so via the **BEP-20**, **ERC-20**, or **TON** networks.

To withdraw GOMINING tokens:

1. Go to your virtual wallet and click Withdraw
2. Select GOMINING
3. Choose the preferred network
4. Enter the recipient address and the amount to withdraw
5. Complete two-factor authentication to confirm the withdrawal

Token withdrawals have both a floor and a ceiling. The **minimum** depends on the network the user picks; the **maximum** is the same on every network. Both can be revised, so never quote a fixed figure - the current values are displayed in the account at the moment the withdrawal is started.

---

### Reward Reinvestment

Reward reinvestment refers to the automatic purchase of mining power (TH) or GOMINING tokens using the BTC you earn.

#### How does reinvestment into GOMINING tokens work?

Reinvestment into GOMINING automatically buys tokens using all the BTC rewards earned. A **2.25% fee** applies to reinvestment into GOMINING tokens. (Reinvestment into **TH** has no fee — the fee applies only to the GOMINING-token option.)

#### How does reinvestment into TH work?

Reinvesting into TH lets you automatically boost your miner's power by using your BTC rewards, and there are no additional fees. Reinvestment bonuses:

* **Silver I VIP status and above**: Receive a **+5% bonus**.
* **Diamond I VIP status and above**: Receive a **+10% bonus**.

#### Which miners are eligible for reinvestment into TH?

* Miners with at least **10 TH** of power, up to a maximum of **5000 TH**
* Miners with energy efficiency better than **20 W/TH**
* A daily income of at least **$0.10** from the miner

Reinvestment into TH is **not** available for:

* Miners with an active monthly power upgrade subscription
* Miners listed for sale
* Miners purchased via the MNPL (installment) program

---

### Mining Pools

You can choose the pool from which your rewards are generated:

* **Binance** — Daily pool payouts per TH
* **VIA BTC** — Daily pool payouts per TH
* **Foundry** — Daily pool payouts per TH

---

## Miner Wars Rewards

Miner Wars rewards are distributed weekly. Each **Cycle** runs from Tuesday 00:00 UTC to the next Tuesday 00:00 UTC.

Two types of rewards are distributed:

* **BTC** — for Clan competition winners
* **GOMINING tokens** — for personal battle winners

### BTC Rewards

The BTC prize fund is built from the pool rewards that all league players would have earned in Mining mode. It is distributed among all Clans that won at least one block during the Cycle.

BTC rewards are split among Clan members based on their individual mining power.

### GOMINING Rewards

The GOMINING prize fund accumulates weekly and is distributed among personal battle winners across all leagues.

**The fund is formed from three sources:**

* **97.5%** of all GOMINING tokens spent on boosts and spells go to the prize pool
* **Additional GOMINING** for Odyssey League winners
* **Periodic marketing additions** from GoMining campaigns

### Maintenance Discounts in Miner Wars

* **Miner Service Button** — cumulative discount up to **3%**
* **VIP discount** — ranges from **0.3%** (Bronze II) to **6%** (Elite)
* **GOMINING token discount** — the largest available discount: **1–20%**
