# Computing Power

### Overview

Computing power is one of the most important characteristics of our digital miners.

In general, the computing power of a miner is the amount of computational resources, typically measured in hashes per second (H/s), that a device or network is capable of contributing to the process of verifying and adding transactions to a blockchain.

Our digital miners, just like real ones, have computing power as they are backed by the power of real miners in the data centers. Each of our digital miners is initially configured with computing power for mining.

The computing power of the digital miners by GoMining is measured in TeraHash/s (TH/s): `1 TH = 1000000000000 H`

By purchasing a digital miner, the holder takes ownership of a portion of the computing power of the device fleet, which is already engaged in mining Bitcoin. The more computing power your digital miner has, the more rewards you get in Mining mode, and the more potential to win you have in Miner Wars.

Also, the total computing power of all your digital miners determines your VIP level, regardless of the mode.

You can find the total computing power of all your digital miners in the Mining farm section.

### Why is the Create Miner calculator's energy efficiency fixed at 12 W/TH? / I can't change it

That's **expected — not a bug.** In the **Create Miner** calculator the energy efficiency is fixed at **12 W/TH** because **all new miners are currently created at 12 W/TH**. Unlike the power / price / expected-BTC-price sliders, the efficiency field there isn't freely adjustable — every newly created miner starts at 12 W/TH. So a user who says the calculator is "stuck on 12 W/TH and can't change it" is seeing correct behaviour; reassure them it's intended. (Efficiency can still be improved **later** on an owned miner through its in-app **Upgrade → Efficiency** flow — that's separate from the create calculator.)

### Power Upgrade

You can upgrade the computing power of your digital miners to get more rewards.

We've introduced a gradation of 20 power levels, topping out at **5000 TH/s** (level 20). The main feature of this differentiation is the unique upgrade price of moving from one stage to another.

> **Minimum power is now fractional.** In supported countries the minimum purchasable/upgradable power is **0.75 TH** (it is no longer a 1 TH floor), with an upgrade step of **0.1 TH**. Whether the 0.75 TH entry tier is available to a given user is decided by their **KYC-verified country**: a user who completed KYC in a non-eligible country won't see the 0.75 TH miner regardless of where they browse, while a user **without** KYC whose profile country is on the eligible list **does** see it. Where the 0.75 TH tier isn't available, the entry level remains higher — don't promise 0.75 TH to everyone.

Our goal is to make the upgrade cost less than buying a new miner of the appropriate power. The higher the level of your digital miner, the cheaper it will cost you to buy additional hashrate.

To increase the performance of your digital miner:

1. Go to the Mining farm page and select the digital miner whose power you want to increase
2. Click on the Upgrade button and select Power
3. You'll see all the information about the available upgrade and its cost

Upgraded miners can be sold on the secondary market and upgraded again to a maximum power of up to 5000 TH.

### How do I pay for an upgrade? Can I pay with my crypto (e.g. mined BTC)?

**Yes — you can pay for a miner upgrade with crypto from your GoMining virtual wallet, including your mined BTC.** In the **Upgrade miner** flow (open the miner → **Upgrade**) you choose **One-time** or **Monthly**, then **Power** or **Efficiency**, pick a preset amount (each preset shows the added TH, the extra BTC/day, and an ROI %) or **Custom**, and then select the **payment asset**.

The payment-asset selector offers, all at **0% fee**:

- **Crypto (from your virtual wallet):** **GOMINING, USDT, BTC, TON, USDC, SOL, BNB, ETH** — so paying with your mined **BTC** balance is supported; just select **BTC** in the list.
- **USDT** is shown as the **Recommended** option, but you are free to pick any of the above.
- Fiat options such as card / **Apple Pay** / Google Pay are also available.

So if a user says "I can only pay with Apple Pay and not with my crypto": that's not a restriction on the product — the crypto assets (including BTC) are in the **payment-asset selector** on the upgrade/purchase screen. Point them to open that selector and choose the crypto asset they want. If the chosen asset's balance is too low, the flow shows a **deposit screen** (amount to send, network, address, QR) to top that asset up first. Only if the crypto options genuinely do not appear for them after checking the selector should you contact GoMining support.

### I only have a tiny balance (e.g. $1.98) — why can't I upgrade with it / why is only card offered?

Every upgrade has a **minimum amount**: the smallest **Custom** upgrade starts at roughly **$15.55**, and the preset tiers start around **$39.99**. A wallet balance **below the smallest available upgrade** (e.g. ~$2) simply isn't enough to fund an upgrade from that balance, which is why the flow may fall back to offering **card** payment (to cover the amount) rather than the wallet balance. So with only a couple of dollars, the options are to **top up** the asset you want to pay with (the flow shows a deposit screen) or pay by card — you can't upgrade using a balance smaller than the minimum upgrade. The exact price thresholds are shown live in the Upgrade flow and vary by miner; if the user needs the precise routing rule for their case, contact GoMining support rather than guessing.
