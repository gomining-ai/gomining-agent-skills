# Burn & Mint Cycles

### What is the Burn & Mint Cycle?

This is a 1-week cycle, at the end of which we burn all GOMINING tokens spent on digital miner maintenance and immediately mint new ones. Each cycle runs from Tuesday to Tuesday.

---

### How long until all GOMINING tokens are distributed? When does emission end?

There is **no fixed distribution schedule or end date** — GOMINING is not a token that gets "fully distributed" by some deadline. It works as a perpetual **Burn & Mint** model: every weekly cycle burns the tokens spent on maintenance and mints new ones, and because each cycle mints **less** than it burns, the total supply gradually **decreases** rather than running out.

The direction is supply *reduction*, from **436,915,240 GOMINING** (the maximum in circulation at the veTokenomics launch) toward a long-term target of **100,000,000 tokens**. There is no fixed completion date — the pace depends on how much is burned each cycle and on the mint-to-burn coefficient set by Epochs and governance Voting. So the accurate answer is that emission is ongoing and indefinite, with supply trending down over time, not toward a one-time full distribution.

---

### How are GOMINING tokens burned and minted?

All miner holders pay for maintenance, and some do so in GOMINING tokens from their virtual wallets.

There's a smart contract wallet that stores the same amount of tokens as all virtual wallets in our system:

> 0xC13F2778B92699e93e6df8c92D1aF8b50c340C3D

When holders pay for maintenance with their GOMINING virtual wallets, the smart contract wallet withdraws the same total amount of tokens. These withdrawn tokens go to the Burn & Mint smart contract:

> 0x44DDEF36f5d4926de2edc495938ADF854C93fA5C

The Burn & Mint smart contract accumulates these tokens during the cycle. And on Tuesday, at the end of the cycle, the smart contract burns all received tokens and right after that mints new ones.

The exact ratio of burned and minted tokens is determined by the Epoch and the governance Voting.

---

### How are the minted tokens distributed?

Every Tuesday, newly minted GOMINING tokens are distributed in fixed proportions:

* **65% to hashpower service providers**
* **20% to veGOMINING vote holders as rewards**
* **10% as GOMINING rewards**
* **5% to the GoMining team**

---

### What are the GOMINING rewards?

The 10% share of weekly emissions (GOMINING rewards) fuels key initiatives:

* **Extra Mining mode discount** — additional discount on maintenance fees for all Mining mode users
* **Miner Wars prize fund** — extra GOMINING rewards for personal victories in the Odyssey league players
* **The Greedy Machines power increase** — TH upgrades for all miners from The Greedy Machines collection

veGOMINING vote holders decide how the GoMining rewards are split between these categories.
