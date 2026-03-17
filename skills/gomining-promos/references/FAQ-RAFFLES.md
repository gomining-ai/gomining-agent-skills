# Raffles & Contests

## Raffles

### What is a raffle, and why should I join?

GoMining raffles are part of a **Gamified Loyalty Program** — they are not a lottery or gambling activity. Instead, raffles are promotional campaigns that give you extra rewards for purchases and actions you already take in the app.

Participation in a raffle is always tied to qualifying transactions (like buying miners or upgrades). You never pay an additional fee or place a wager to join — your regular purchases and actions automatically generate raffle tickets.

Each raffle has its own rules, but the more tickets you have, the higher your chances of winning. At the end of the raffle, winners are selected randomly using a transparent, blockchain-based algorithm. Prizes can include GoMiners miners, tokens, and other exclusive rewards.

This way, raffles add a fun and rewarding layer on top of your usual app activity.

---

### Who can participate?

Anyone with a GoMining account can take part in raffles, but most raffles require you to have at least one active miner (besides the Bonus miner) to collect tickets.

You'll start collecting tickets automatically if you meet the raffle conditions — but to appear in the list of participants and be eligible to win, you must confirm your participation by tapping the **Take part** button in the raffle.

If you haven't confirmed, your tickets still accumulate — they'll be counted once you join.

---

### How do raffle tickets work?

You earn raffle tickets with unique numbers by completing certain actions (like creating a miner or upgrading its power). The more you do, the more tickets you get. Conditions for earning tickets may differ from raffle to raffle.

> For example, if 1 ticket = $10 spent on upgrades, spending $99 will earn you 9 tickets.

Tickets are only awarded after you confirm participation in the raffle. If you've already made purchases during the raffle period before joining, don't worry — they'll still count once you opt in.

---

### Ticket assignment rules

Ticket numbers are assigned only after you confirm your participation. Numbers are assigned sequentially from `0` to `N - 1`, where `N` is the total number of tickets issued in the raffle. If you earn multiple tickets for a single action, like upgrading a miner, they'll be assigned consecutively.

If two users make purchases at the same time, the user with the lower user ID gets their tickets assigned first.

If a qualifying purchase is later canceled, the associated tickets become inactive, but their numbers remain in the system. Once a raffle ends, **no more tickets can be issued**.

---

### How is the winner chosen?

When the raffle ends, we:

1. Take the hash of the latest closed Bitcoin block and convert it into a decimal number
2. Divide this number by the total number of tickets, and the **winner is the ticket with the remainder of that division**

**What if something goes wrong?**

* If the winning ticket was canceled
* If a duplicate winning ticket is selected (for raffles with multiple prizes)
* If another prize needs to be awarded (for raffles with multiple prizes)

Then the draw is repeated: we use the hash of the previous Bitcoin block and divide it by `N - 1`, `N - 2`, and so on — until a valid winner is found.

> Prizes are awarded to winning tickets. If you have multiple winning tickets, you get a prize for each one.

---

### How do I claim my prize?

All prizes must be claimed manually by tapping the **Claim Prize** button on the raffle screen. Some prizes will be credited to your account automatically right after you tap the button. Others may require contacting our support team — in that case, you'll see clear instructions in the app.

> GoMining will never contact you via Telegram, WhatsApp, or other messengers to say you've won. If someone does — it's a scam. Never share your personal information with anyone.

---

## Contests

### What is a contest?

A contest is a competition where users complete specific tasks to climb the leaderboard and win prizes.

The leaderboard ranks participants based on how well they perform in the contest — like referring new users, purchasing power, etc. The more you do, the higher you rank.

Each contest has a clearly defined start and end date. Winners are determined once the contest ends.

---

### What rewards can I win?

Each contest has a set of prizes for the top participants. The number of winners and reward details are listed on the contest page.

---

### How can I win?

Complete the contest task as much as possible, depending on the rules. The more you contribute, the better your chances of ranking high.

---

### How do I claim my prize?

In most cases, prizes are credited automatically to your account. If manual claiming is needed, a Claim Prize button will appear on the contest page.

---

### Why am I not showing up on the leaderboard?

Some contests have specific requirements or conditions you need to meet to be included. Double-check the contest rules to make sure you've completed everything needed during the contest period.

If everything looks good on your end and you're still not showing up, feel free to reach out to our support team.
