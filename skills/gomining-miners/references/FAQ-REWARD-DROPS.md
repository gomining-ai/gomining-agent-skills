# Why Did My Mining Reward Drop?

## Common Reasons for a Reward Decrease

### 1. Bitcoin Network Difficulty Increased

Mining rewards are calculated using the **FPPS (Full Pay Per Share)** method. Bitcoin network difficulty adjusts approximately every 2 weeks as more miners join the network. When difficulty rises, the BTC earned per TH decreases for everyone — this is automatic and affects all miners globally.

### 2. Maintenance Fees Took More from BTC Rewards

Each miner has a daily fee for electricity and service. The system deducts from GOMINING tokens first. If your GMT balance is insufficient to cover the full fee, the remaining amount is taken directly from your BTC reward — making the payout look much smaller than usual.

Causes:
- GMT balance dropped below the threshold
- VIP discount level changed (lower discount = higher deduction)
- BTC price dropped (USD-denominated fees = more BTC deducted at lower BTC price)

### Reconciling a lower-than-expected wallet balance vs a credited reward

When the user says *"my Rewards line shows +0.00001602 BTC but my wallet only went up by 0.00000521 BTC — where did the rest go?"*, walk them through the deduction, don't just hypothesise. Structure:

1. **Confirm both figures** — quote the credited reward from the reward-history tool AND the wallet change (or reward-history net) exactly as returned.
2. **Explain the deduction order plainly.** *"The daily electricity + service fee comes out of GOMINING tokens first; if your GMT balance can't cover it, the shortfall is taken out of the BTC reward before it reaches your wallet."* So a gross reward of `X BTC` can arrive as `X - (shortfall / BTC-price)` in the wallet if GMT was short.
3. **Worked example** (label as illustrative): gross reward 0.00001602 BTC, wallet increase 0.00000521 BTC ⇒ the BTC leg of the fee absorbed ~0.00001081 BTC of the reward. That's the fee shortfall in BTC-equivalent for that day; the rest of the day's electricity + service went out of any GMT balance the user had.
4. **Where the user can verify the breakdown themselves.** Point them to the **Rewards** tab (each row shows the per-day electricity (C1) / service (C2) split and applied discount) or the **CSV rewards report** (Rewards → Export CSV → date range) — those give the exact fee columns and the total discount for that date. Do **not** invent a specific per-day fee amount if the tool didn't return it.
5. **Do not present this reconciliation as a certainty** if you don't have C1/C2 figures for that day — frame it as *"the shape of the gap is consistent with fee deduction; the exact split lives in the Rewards tab / CSV"*, and escalate if the user needs an authoritative accounting.

### 3. Reinvestment Is Converting Your BTC Into GMT or TH

If you turned on **Reinvestment** (Mining farm → Settings), your BTC rewards are no longer kept as BTC — they are **automatically converted** into either **GOMINING tokens** (credited to your virtual wallet) or **TH** (added to a selected miner), depending on the option you chose. Your BTC reward history then looks like it "dropped" or stopped growing, but you have **not** lost money — the value moved into GMT or TH instead. (There is no separate "GMT mining mode"; this is the Reinvestment setting — see [Reinvestment Options](FAQ-REINVEST-OPTIONS.md).)

- **GMT reinvestment:** check your **virtual wallet** GMT balance to see the converted value.
- **TH reinvestment:** check the selected miner's added power (and the email confirmation).
- To resume receiving BTC, set the Reinvestment option back to **Receive rewards in BTC**.

Separately, the **display** can also differ between modes: with reinvestment active, rewards may be shown net of service fees; without it, gross (pre-fee) rewards may be shown — so the figure can look different even when the underlying mining output is the same.

### 4. Hashrate Upgrade — Next Cycle Delay

If you recently upgraded your miner's TH, the upgraded capacity only starts earning from the **next full daily cycle (00:00–00:00 UTC)**. The first reward after an upgrade may appear lower than expected.

### 5. Miner Switched to Miner Wars Mode

Miners in **Miner Wars** mode do not earn daily BTC rewards in the same way — rewards are distributed weekly based on clan block wins. A miner switched to this mode will show no daily BTC output.

---

## Why was my income 0 for the day/week (zero rewards)?

> **First, if a reward-history lookup comes back empty / shows nothing at all** (not just a small number), the most likely reason is that the account is in **Miner Wars mode** (rewards are weekly, not daily — the daily view can show nothing) or has **reinvestment enabled** (BTC is converted to TH/GMT, not accumulated). Check mode and reinvestment **first** and surface that proactively, before concluding the user "isn't earning" — don't make the user ask twice.

If your net reward is **0** even though your miners show as active, the usual cause is that your **maintenance fees were equal to or higher than the BTC your miners earned**. When that happens, **Reward Protection** keeps you from going negative: instead of charging you the difference, the miner is marked inactive for that period and both the reward and the maintenance show as 0. So you don't lose money — but you also don't earn any.

This is not a bug and not "missing" rewards. It means the cost to run your miners reached or exceeded what they produced. The most common underlying reasons are:

- **Poor energy efficiency (high W/TH) — the most common cause.** A higher W/TH means a higher electricity fee per TH, which eats up more (or all) of the reward.
- **A low maintenance discount on the account.** With little or no discount, the full electricity and service fees are deducted, leaving nothing.
- **A weak BTC market (low BTC price).** Fees are set in USD but deducted in BTC, so when BTC is low, the fees consume a larger share of the BTC reward.

### What to do about it

The goal is to push fees back below your rewards. Two levers help most:

1. **Increase your maintenance discount.**
   - **Service button (free):** click it once per UTC day — each day adds +0.3% to your discount, up to a maximum of 3% after 10 days in a row. Missing a day resets the progress.
   - **Hold more GOMINING tokens:** keeping enough unlocked GOMINING in your wallet to cover maintenance unlocks a discount of up to 20% (the more days of fees your balance covers, the higher the discount).
2. **Upgrade your miners' energy efficiency (lower W/TH).** A more efficient miner has a lower electricity fee, so more of the mined BTC stays with you. This is usually the highest-impact fix when efficiency is poor.

A higher VIP tier also adds a maintenance discount. To see the exact breakdown for any day, go to **My Miners → Rewards**, tap the payment record, then tap a miner.

---

## Formula

```
Net Reward = Pool Reward − ([Electricity + Maintenance] × [1 − Discount])
```

If total fees exceed the pool reward on a given day, net reward = 0 (if Reward Protection is off) or the miner is marked inactive with 0 maintenance charged (if Reward Protection is on).

---

## How to Check the Full Breakdown

Go to **My miners → Rewards**, tap the payment record, then tap a specific miner to see the full breakdown of pool reward and all deductions.

---

## What Is NOT a Cause of Reward Drops

- The **90-day selling restriction** has no effect on reward calculation — it only affects the ability to sell or withdraw a miner, not its earnings.
- Reward Protection being enabled means fees are not charged when they exceed rewards — it does not reduce rewards.

---

## When you can't explain a large, sudden drop

If none of the causes above fits a big sudden drop (e.g. ~90% lower than usual), be honest about the limits: you do **not** have access to **network-difficulty history** or a **per-miner reward breakdown over time**, which are what's needed to pinpoint it. Do **not** present an unverified guess (e.g. "Bitcoin network difficulty rose") as the confirmed cause, and don't keep floating new hypotheses turn after turn. Walk through the documented causes, and if they don't explain it, **collect the details (which miners, the dates, the before/after figures) and contact GoMining support** for a definitive answer rather than leaving the user with a hypothesis.
