# FAQ & Troubleshooting

Common pain points and edge cases. Grouped by area.

---

## Spells & Power-ups

### My Instant Boost didn't add points — what happened?

Instant Boosts (and Focus Boosts) have a **3-second delay** before they take effect. If the round ends during those 3 seconds, you do not receive the points. There is no refund — the GMT is spent.

**Avoid this by:** casting Instant/Focus Boosts early in a round, especially in low-multiplier rounds that may resolve quickly.

### My Focus Boost timed out — why?

Focus Boosts grant a large number of points but the points are **only valid for 5 minutes**. If the round runs longer than 5 minutes from your cast, the points expire.

**Use Echo Boosts instead** for rounds you expect to be long — Echo grants points every 2 minutes with no expiration.

### My Power-up cost changed since last round

**Power-up and Clan Power-up costs scale with your base PPS.** Adding TH or upgrading energy efficiency increases the price for these spells specifically. In Spell Bot, these spells are flagged with a yellow icon as a reminder. Setup TOTAL can shift between rounds even without edits.

### Can I cast the same spell twice?

Yes — but **not by adding it twice in Spell Bot**. Use the quantity buttons (− / +) to increase how many times the bot casts it per round. Manually you can cast as many as your budget allows (subject to per-spell rules; e.g. Power-up is **once per round**).

### Miner Service didn't fire — why?

Miner Service is **free but has a daily cooldown** (once per day). It cannot be cast twice in 24 hours. Don't add it to a Spell Bot Setup — cast it manually once per day to keep the consecutive-day streak going for the cumulative maintenance discount (+0.3%/day, max 3% after 10 days).

### My Copy Boost didn't amplify the boost I wanted

Copy Boosts copy a percentage of the **next** boost cast in the same round. If you cast Copy *after* the target boost, it copies nothing useful.

**Manual order:** cast Copy first, then the target boost.
**Spell Bot order:** place Copy **earlier** in the cast priority list than the target.

---

## Spell Bot

### All my Setups are off — I only disabled one

**An empty budget disables every Setup**, not just the active one. Check the SPELL BOT BUDGET card — if it's at 0.00, transfer GMT in and they'll re-enable.

### Some spells in my Setup didn't fire mid-round

The bot casts spells **top to bottom** in your Setup. If the budget runs low mid-round, lower-priority spells get skipped. **Drag the most important spells to the top.**

### My Setup cost shows a different total each round

That's expected if the Setup includes Power-up or Clan Power-up — their costs scale with PPS (see "My Power-up cost changed" above).

---

## Clans

### I was removed from my Clan without warning

If you are **not the Clan Owner**, your membership can be revoked without explanation. When this happens, your mining farm **automatically switches back to Mining Mode** — you won't be silently sitting out of both modes.

### I'm a Clan Owner and my VIP just dropped below Gold I

| Time to Cycle end | What happens |
|---|---|
| **More than 24 hours** | You keep ownership through the current Cycle. If Gold I is not restored by Cycle end, ownership transfers to the highest-TH member next Tuesday. |
| **Less than 24 hours** | You keep ownership through the **next** Cycle. |

### My Bonus Miner power isn't counted for Clan entry

Correct — **Bonus Miner power is excluded** from Clan entry requirements (TH and GMT minimums). It also only adds to your Miner Wars stats **if you own at least one Digital Miner** — a Bonus Miner on its own does not let you participate. Once you do own a miner, its power adds on top inside a Clan.

### Can I create more Clans?

You can create up to **3 Clans per year** if you're Gold I+. There is no upgrade path beyond that.

### My Clan logo was rejected

Logos must be: JPG/PNG, ≤ 2 MB, original, no trademarks or third-party project names, no references to religion/nationality/culture, no offensive content.

---

## Rewards

### My Clan won blocks but I got 0 BTC

BTC inside a Clan is distributed **proportional to individual mining power**. If your TH is very small relative to the Clan total, your share may round down to near-zero — especially when the Clan's total share is split across many members.

### I spent a lot of GMT on spells but got 0 GMT back

GMT rewards go to **personal-battle winners**. Spending doesn't guarantee a personal win — it raises your PPS for the rounds you participate in. If you didn't place high enough in personal rankings, you get nothing.

The economics: 97.5% of all GMT spent on spells goes into the personal-battle pool. **It's a competitive redistribution** — high spenders without high relative performance subsidize the winners.

### BTC withdrawal is disabled

To enable BTC withdrawals, you must have created **at least one miner directly on the GoMining platform**. If your miners are all from the secondary market (OpenSea, Magic Eden, Getgems) or imported from external wallets, BTC withdrawals stay disabled until you create a primary miner through GoMining.

### Withdrawal options:
- **Fast** — within 1 hour, fixed fee, **KYC required**
- **Standard** — within 24 hours, **no fees**

### How much GMT can I withdraw per day?

Up to **30,000 GMT/day** via BEP-20, ERC-20, or TON.

---

## Modes

### I switched a miner to Miner Wars mid-Cycle — did I lose the BTC I had earned?

No. Rewards already earned in the previous mode are kept. Going forward, the miner contributes to whichever mode it's currently set to.

### Can I keep some miners in Mining Mode and others in Miner Wars?

Yes — the mode setting is **per-miner**. There is no platform rule that all miners must be in one mode. Hybrid strategy: keep high-TH/high-efficiency miners in Miner Wars (better PPS contribution), keep MNPL or subscription-locked miners in Mining Mode (they can't reinvest anyway).

### Which miners can't be in Miner Wars?

There's no hard exclusion, but these miners are typically left in Mining Mode because they can't reinvest BTC into TH:
- Miners with an active monthly power upgrade subscription
- Miners listed for sale
- Miners purchased via MNPL (installment)

---

## Cycle & Rounds

### When does the Cycle end? My rewards aren't showing

Cycles run **Tuesday 00:00 UTC → next Tuesday 00:00 UTC**. Rewards are calculated and distributed at Cycle end automatically. If you don't see rewards immediately after, give it a short delay — distribution is automatic but not always instant.

### A round ran really long / really short

Round length is bound to the Bitcoin network — a new Bitcoin block confirmation ends the round. Block intervals are irregular by design (~10 minutes average, but can be 1 minute or 30+). Average ~120–150 rounds per day.

### Why is my multiplier so low / high?

Round multipliers are based on **how many Bitcoin blocks are mined simultaneously**. You can't influence them. Higher leagues unlock higher max multipliers (Dune x32 → Odyssey x256), so league promotion is the only way to access bigger multipliers.

---

## Bans & Fair Play

### What gets me banned?

- Third-party software / bots (Spell Bot is **fine** — official)
- Operating multiple accounts
- Collusion / coordinated outcome manipulation
- **League Hopping or Clan Cycling** — moving between Clans/accounts to manipulate league placement, bypass difficulty scaling, or monopolize promotion slots

Penalties range from **temporary suspension to permanent ban**.

### Is Spell Bot allowed?

**Yes — it's an official GoMining feature.** Using it never triggers a ban.

---

## Cross-skill

### Does my Platinum+ discount apply in Spell Bot?

Yes — Platinum+'s 15% spell discount applies to **every** spell the bot casts, just like manual casts.

### Does the Platinum+ discount stack with GoMiners Avatar discount?

**No — they don't stack.** The **highest** of the two applies. If your Avatar discount is higher, Platinum+ contributes nothing on top.

### Does veGOMINING voting actually change my rewards?

Indirectly. veGOMINING holders vote on weekly emission allocation. One of the allocations is the **Miner Wars prize fund** (extra GMT for Odyssey winners). More votes for that bucket → larger Odyssey personal-battle pool.

### Do I need to be in Miner Wars to get referral electricity rewards?

No. Mining Mode referrals → daily electricity rewards. **Miner Wars Mode referrals → weekly electricity rewards** at Cycle end, based on weighted-average EE. The 2.5% bonus on referrals' boost spending applies only in Miner Wars Mode.
