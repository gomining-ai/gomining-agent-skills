# Reinvestment Options

## Can I set different reinvestment options for different miners?

No. All miners in your account operate under a **single reward mode** at the same time. You can choose only one option:

- Reinvest rewards into **TH** (mining power)
- Reinvest rewards into **GOMINING tokens**
- Receive rewards in **BTC**

It is not possible to apply different reinvestment options to individual miners.

### TH Reinvestment

- Rewards from all miners are pooled and reinvested into a **single selected miner**.
- Requires **Silver I VIP status** or above.
- +5% bonus on mining rewards at Silver I; +10% at Diamond I.
- The selected miner must be stored in your **GoMining virtual wallet** or a **linked external wallet**.
- **Minimum daily-reward threshold: $0.10.** TH reinvestment only converts a day's reward into TH if that day's net BTC reward is **at least $0.10**. If a day's reward is **below $0.10**, it is credited **directly to your virtual wallet in BTC** for that day — it is **not** reinvested into TH, and the TH-reinvest setting isn't paused or disabled (it just doesn't apply to sub-$0.10 days). No user action is required; the setting stays on and will resume converting to TH the next day the reward crosses $0.10.

> **How to answer the "what happens if BTC price drops and my daily reward falls under $0.10?" question:** the reinvest-eligibility rule above is the answer — the day pays out as BTC to the virtual wallet, and larger-reward days continue reinvesting as normal. There is no auto-pause, no notification, no eligibility lockout — just per-day routing based on that day's reward size. Answer this directly when asked (previously a documentation gap that led to unnecessary escalation).

**Where to set it up and see the expected daily gain:**

1. Open the **Mining farm** tab.
2. Tap **Settings** (gear icon, top-right of the Mining farm card).
3. In the **Reinvestment** section, toggle it on and select **TH**.
4. Choose the miner to reinvest into under **Select miner**.

Once TH is selected, the panel shows **"Expected daily rewards in Mining mode"** as the daily TH that will be added (e.g. ~0.10 TH/day). This is the only built-in figure available for TH reinvestment.

> **No time-to-target projection exists.** The app does **not** have a calculator that tells you how long it will take to reach a target TH (e.g. "from 10 TH to 50 TH"). Do not tell users such a calculator exists. The only available figure is the expected **daily** TH gain shown above. A rough manual estimate is *remaining TH ÷ expected daily TH gain*, but this understates speed because the daily gain grows as power increases (compounding) and the figure shifts with live TH price, efficiency, and discount. For a precise estimate, direct the user to the GoMining support team or community.

### GOMINING Token Reinvestment

- Rewards are automatically converted to GOMINING tokens and credited to your virtual wallet.
- A **2.25% fee** applies to reinvestment into GOMINING tokens. (TH reinvestment has no fee — the fee is only on the GOMINING-token option.)

> **"I earn / accumulate GMT from mining" is a real flow — don't over-correct.** Mining itself pays **BTC**, but with **GOMINING-token reinvestment** enabled, those BTC rewards are auto-converted to **GMT**. So when a user says they "earn GOMINING from mining" or asks how much GMT they'll accumulate over time, do **not** keep correcting them with "mining only pays BTC" — recognise they have GMT reinvestment on and work with that. You may do arithmetic on figures the user supplies (e.g. "0.5 GMT/day at $0.30"); if you need the live GMT price and the price tool fails, **ask the user for the current price immediately** rather than retrying and stalling. Don't fabricate a forward compounding projection from an assumed price — use their numbers or the calculator.

### Why isn't my per-miner BTC milestone counter (e.g. "toward 0.01 BTC") increasing?

The most common reason is that **reinvestment is enabled**: if you're reinvesting into TH or GOMINING, your BTC rewards are being **converted** rather than accumulating as BTC, so a per-miner "BTC earned toward 0.01 BTC" style counter won't move. Check the Reinvestment setting first — if it's on and the user wants BTC to accumulate, they'd switch reinvestment off (Mining Farm → Settings → receive rewards in BTC). If **reinvestment is off** and the counter is still stuck for days, there is **no tool to read that per-miner milestone counter** — don't guess further explanations; contact GoMining support.

---

## Where Can I See My Reinvestments?

- **GOMINING token reinvestments:** visible in your virtual wallet and in the Rewards section.
- **TH reinvestments:** shown in the email confirmation you receive. You can also check manually by opening each reward entry in the dashboard.

---

## Can I Switch to Solo Mining Without Leaving My Clan?

No. GoMining only allows one mining mode at a time. To mine solo, you must leave your clan first.
