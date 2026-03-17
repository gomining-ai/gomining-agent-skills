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

### 3. Reinvestment Setting Changes How Rewards Are Displayed

- **With reinvestment active:** rewards are shown post-deduction of service fees (net amount)
- **Without reinvestment:** gross (pre-fee) rewards may be displayed

Switching between these modes can make rewards appear to change even if the underlying mining output is the same.

### 4. Hashrate Upgrade — Next Cycle Delay

If you recently upgraded your miner's TH, the upgraded capacity only starts earning from the **next full daily cycle (00:00–00:00 UTC)**. The first reward after an upgrade may appear lower than expected.

### 5. Miner Switched to Miner Wars Mode

Miners in **Miner Wars** mode do not earn daily BTC rewards in the same way — rewards are distributed weekly based on clan block wins. A miner switched to this mode will show no daily BTC output.

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
