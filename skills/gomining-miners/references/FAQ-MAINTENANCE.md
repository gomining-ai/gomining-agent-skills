# Maintenance Fees and Discounts

### Why are there maintenance fees?

Each miner in our collections is powered by a real fleet of devices — this is what allows them to mine Bitcoin for you.

When buying a miner, you are purchasing a portion of existing ASICs, each one of which requires maintenance. Our service center handles it 24/7 on its own, and you only pay a daily fee.

---

### How do maintenance fees affect my rewards?

To calculate your daily net reward, we deduct the maintenance fees (electricity and equipment service) from your pool reward, applying all your maintenance discounts.

Net Reward = Pool Reward − (Electricity + Service) × (1 − Discounts)

---

## Maintenance Discounts

### Where do I find the maintenance / discounts page?

1. Open the **Mining farm** tab.
2. Tap **Settings** (gear icon, top-right of the Mining farm card).
3. In **Settings** you'll see **Maintenance in GOMINING** (toggle on to pay maintenance with GOMINING tokens for up to 20% discount), along with **Reward protection**, **Reinvestment**, and **Pool** selection.
4. Under **Maintenance in GOMINING**, click **Increase discount ›** to open the **Maintenance discounts** page.

The **Maintenance discounts** page shows your **Total discount** (e.g. "2.08% of 29.88%" — current of maximum) and each component you can work on:

- **Token discount** — up to 20%, based on how many days of maintenance your balance + locked tokens cover (slider 0–20%).
- **Service discount** — up to 3%, via the daily **Service** button (10-day streak).
- **VIP discount** — based on your VIP status (shows current and next tier).
- **Mining mode discount** — depends on reward-distribution voting results.

It also has a **"What is miner maintenance?"** link for an explainer.

### Where do I see my total maintenance discount and where it comes from?

This exact **Maintenance discounts** page is the single place that shows it: your **Total discount** and the **breakdown by source** — Token, Service, VIP, and Mining-mode — all in one view. Reach it via **Mining farm → Settings (gear) → Maintenance in GOMINING → Increase discount ›**. Do **not** send users to "Rewards → individual miner" for the discount breakdown — it's the Maintenance discounts page. Note the **Service discount is streak-based** (a daily click on the Service button, up to 3% over 10 days) — it is **not** based on your wallet balance; the wallet-balance-driven part is the separate **Token discount**.

### What is my total daily maintenance cost (in BTC / USD)?

The **exact** daily maintenance figure is shown **in-app** — on the Maintenance page and per-day in **Rewards** (tap a reward record to see that day's electricity **C1** and service **C2**). Maintenance = **electricity (C1) + service (C2)**, minus your discounts. Do **not** just answer with wattage — explain the composition and point to the in-app figure. You may give an **approximate electricity** portion from documented rates (electricity ≈ **$0.05–$0.07/kWh**, so daily electricity ≈ total watts × 24 ÷ 1000 × ~$0.06), but you do **not** have a documented service-fee rate, so don't fabricate a precise total — the exact combined figure (with service and discounts) is the one shown in the app.

### Discount for maintenance with GOMINING

#### What is the maximum maintenance discount I can receive by paying with tokens?

You can receive a maintenance discount of up to 20% by paying maintenance fees with GOMINING tokens from your virtual wallet. The discount amount depends on how many days your virtual wallet balance, together with your locked tokens, can cover maintenance fees.

**You do NOT need 360 days to get a discount.** The discount is **tiered by days of coverage**: it **starts at 18 days = 1%** and scales up to the **maximum 20% at 360+ days**. The 360-day figure is only for the *maximum* discount, not the entry threshold — any coverage of 18+ days already gives some discount. Use the full breakpoint table below when answering "how many days for X%".

#### Discount table based on the number of tokens:

| Days of maintenance | Discount |
| ------------------- | -------- |
| 0–17                | 0%       |
| 18–35               | 1%       |
| 36–53               | 2%       |
| 54–71               | 3%       |
| 72–89               | 4%       |
| 90–107              | 5%       |
| 108–125             | 6%       |
| 126–143             | 7%       |
| 144–161             | 8%       |
| 162–179             | 9%       |
| 180–197             | 10%      |
| 198–215             | 11%      |
| 216–233             | 12%      |
| 234–251             | 13%      |
| 252–269             | 14%      |
| 270–287             | 15%      |
| 288–305             | 16%      |
| 306–323             | 17%      |
| 324–341             | 18%      |
| 342–359             | 19%      |
| 360+                | 20%      |

To achieve the maximum 20% discount, you need to have enough tokens to cover more than 360 days of maintenance.

#### How many GMT do I need for a given discount? (formula / worked example)

The discount is driven by **days of maintenance coverage**, not by a fixed token count — so the GMT needed depends on **your own daily maintenance fee**, which varies with your fleet's TH and energy efficiency. Use this to self-calculate instead of dead-ending on "I can't see it":

> **Tokens needed ≈ (target days of coverage) × (your daily maintenance fee) ÷ (GMT price)**

Steps:
1. Pick the **target days** from the breakpoint table above (e.g. 18 days → 1%, 90 days → 5%, 360+ days → the max 20%).
2. Find your **daily maintenance fee** — shown on the Mining farm / Maintenance page (your balance + locked tokens are measured against it as "days covered").
3. Multiply days × daily fee to get the maintenance value to cover, then divide by the current GMT price for the token amount.

**Worked example:** if your daily maintenance is **$0.50/day** and you want the **1% tier (18 days)**: 18 × $0.50 = **$9 of maintenance coverage**; at a GMT price of, say, $0.30 that's about **30 GMT**. For the **max 20% (360 days)**: 360 × $0.50 = **$180**, ≈ **600 GMT** at $0.30. Plug in the user's actual daily fee and the live GMT price rather than these placeholders — do not present the placeholder numbers as their real figures. If the daily-maintenance figure isn't available from a tool, ask the user for the daily maintenance fee shown on their Maintenance page, then compute it with them.

#### How to activate payment with tokens to get a discount?

To activate payment with GOMINING tokens, select this option in the reward settings on the rewards page.

#### Does the discount apply to Bonus Miner?

The discount does not apply to Bonus Miner rewards.

---

### VIP Discount

It's based on your personal VIP status. The discount amount varies depending on the number of TH or veGOMINING votes owned. Players will receive a 0.3% discount for the Bronze II VIP level and a 6% discount for the maximum Elite level.

---

### Service Discount

When you click the Service button in your Mining farm, it can be used once per UTC day. Each day you click the button, your discount increases by +0.3%.
- Maximum discount: 3%
- To reach it, you need to click the button for 10 days in a row
If you miss a day and don't click the button within that UTC day, the discount progress resets.

**What the Service button looks like / where it is (web):** it's a **purple button at the top-right of the Mining farm panel**, immediately to the **left of the Settings (gear) button**, with a small **brush / broom ("service") icon**. Before you use it for the day it is **labelled "Service Button"**; once you click it, the label is replaced by a **countdown timer** (e.g. hours:minutes:seconds) showing the time left until you can click it again (the once-per-UTC-day cooldown). So if a user says they only see a timer and no "Service Button" text, that means they've already clicked it today — it will become clickable again when the timer runs out.

**If a user asks "what does the *Service* option/button do?"** (e.g. they see **Service** among the controls in the Mining farm / miner area), that **is** this Service Button — the free once-per-UTC-day click that builds a maintenance-discount streak (+0.3%/day, up to 3% after 10 days). Connect the label "Service" to this mechanic directly; don't treat it as an unknown feature or escalate.

**Notifications for the Service Button (or any mining notification) — route to support.**
The current app has no documented built-in push notification for the Service Button cooldown (you know only the on-screen timer described above). Whether such a notification existed in a prior version, was removed, or is on the roadmap is **not documented** — do not confirm or deny a past feature. When a user asks about notification behaviour ("there used to be a push notification, did it get removed?", "why don't I get notified when I can click again?", "can I turn notifications on for this?"), don't speculate on feature history. direct the notification issue to GoMining support — that's where notification questions and requests go. Briefly note the on-screen timer as the currently documented way to see the cooldown before escalating, so the user has something usable in the meantime.

---

### Mining Mode Discount

All users of Mining mode have an additional discount on maintenance fees. You don't have to do anything to activate it.

This discount is one of the categories that GoMining rewards cover. The amount of the discount depends on the Burn & Mint cycles of veTokenomics and on veGOMINING voting results.
