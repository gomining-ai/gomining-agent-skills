---
name: gomining-avatars
description: "GoMining avatar collections — functional avatars assignable to Digital Miners, each race with a unique ability. Covers the avatar races (Humans, Sentinels, Cryptiles, Luminars, Magmars), their unique abilities, Luminar VIP level boost rules, secondary marketplace for miners and avatars, and branded merchandise."
license: Apache-2.0
compatibility: "Compatible with Claude Code, Codex, and all Agent Skills spec tools."
metadata:
  author: gomining
  version: "1.0"
  tags:
    - avatars
    - nft
    - marketplace
    - luminars
    - miner-wars
  triggers:
    - "avatar collection"
    - "luminars"
    - "luminar vip boost"
    - "nft marketplace"
    - "gomining merch"
    - "avatar races"
---

# GoMining Avatar Collections

## Overview

Avatars are functional avatars that can be assigned to Digital Miners. Each race has its own **unique ability** (in addition to shared core benefits like a 5% discount on miner creation, presale access, and a Welcome pack). The unique ability activates only when the avatar is set as your profile picture, and only one ability can be active at a time. There will be 10 series in total. For information on Digital Miners themselves (blockchains, pricing, earning modes), see the [gomining-miners skill](../gomining-miners/SKILL.md).

---

## The Races

| # | Race | Collection URL | Unique Ability |
|---|------|---------------|----------------|
| 1 | **Humans** | app.gomining.com/gominers-collection/humans | **Automated Service** — applies the 3% maintenance discount automatically (no manual Service button) |
| 2 | **Sentinels** | app.gomining.com/gominers-collection/sentinels | **20% Discount on Spells** — every spell and boost in Miner Wars is 20% cheaper |
| 3 | **Cryptiles** | app.gomining.com/gominers-collection/cryptiles | **Enhanced Efficiency** — reduces miners' energy consumption by 1 W/TH (cannot go below 20 W/TH) |
| 4 | **Luminars** | app.gomining.com/gominers-collection/luminars | **+1 VIP Level** — raises VIP level by 1 without meeting standard requirements |
| 5 | **Magmars** | app.gomining.com/gominers-collection/magmars | **Blazing Multiplier (×1.4)** — applies a ×1.4 multiplier to base Simple Earn yield (equivalent to Legend 3 / VIP 18) |

---

## Luminar Avatar Rules

Luminars provide a unique VIP tier boost.

| Rule | Description |
|------|-------------|
| **VIP Boost** | Setting a Luminar avatar as your profile picture grants +1 VIP level immediately |
| **Eligibility** | Works without meeting the standard VIP requirements — there is no TH threshold |
| **Removal** | Removing the Luminar avatar (or unsetting it as profile picture) immediately reverts the VIP level |
| **GoBox Reward** | A GoBox is issued once when the new VIP level is reached |
| **Re-assignment** | GoBox is **not** re-issued if the Luminar is removed and reassigned |
| **Bronze Protection** | Bronze GoBox is **not** issued to prevent farming exploits |

### Luminar VIP Boost Flow

1. User sets a Luminar avatar as their profile picture.
2. Their VIP level increases by +1 immediately, without needing to meet the standard VIP requirements.
3. A GoBox corresponding to the new VIP level is issued (one-time).
4. If the user removes the Luminar avatar, VIP level reverts to the original.
5. Reassigning the same or different Luminar does **not** re-issue the GoBox for that level.
6. If the user is at Bronze tier, no GoBox is issued (anti-farming measure).

---

## Secondary Marketplace

The GoMining marketplace enables peer-to-peer trading of Digital Miners and avatars.

| Feature | Description |
|---------|-------------|
| **Miner Trading** | Buy and sell Digital Miners |
| **Avatar Trading** | Buy and sell avatars |
| **Listing** | Users set their own prices |
| **Settlement** | Transactions settled on-chain |
| **Supported Assets** | Digital Miners, Avatars (all races) |

---

## Merchandise

GoMining offers physical branded merchandise available through the marketplace ecosystem.

| Category | Description |
|----------|-------------|
| **Branded Products** | Official GoMining-branded physical items |
| **Availability** | Through the GoMining marketplace |
| **Shipping** | Details available at time of purchase |

---

## FAQ

### How do Luminar avatars affect my VIP level?
Setting a Luminar avatar as your profile picture gives an immediate +1 VIP level boost — without needing to meet the standard VIP requirements (there is no TH threshold). The boost is removed if you unassign the avatar or unset it as your profile picture.

### Will I get another GoBox if I reassign a Luminar?
No. The GoBox is issued once per VIP level achieved through Luminar assignment. Removing and reassigning does not re-issue the GoBox.

### Can I trade my avatar on the marketplace?
Yes, all avatar races (Humans, Sentinels, Cryptiles, Luminars, Magmars) can be traded on the secondary marketplace.

### What is GoMining merch?
GoMining offers physical branded products that can be purchased through the marketplace ecosystem.

---

## References

- [Avatar Collections](references/AVATAR-COLLECTIONS.md) — Race details and collection URLs
- [Marketplace](references/MARKETPLACE.md) — Trading mechanics for miners and avatars
- [FAQ: Collections Overview](references/FAQ-COLLECTIONS.md) — Overview of GoMiner NFT collections
- [FAQ: GoMiners Avatars](references/FAQ-AVATARS.md) — Avatar NFTs, races, and how to use them
- [FAQ: Main Collections](references/FAQ-MAIN-COLLECTIONS.md) — Details on the main GoMiners collections
