# Security Mode

## What is Security Mode?

**Security Mode** is a **12-hour hold** placed automatically on **withdrawals** and **miner sales** whenever the credentials protecting a GoMining account change. Everything else continues to work — the hold exists only to give the account owner time to react if the credential change wasn't theirs.

Security Mode is applied to **every account**, no exceptions.

## When does Security Mode turn on?

Security Mode starts automatically after **any** of these three actions on the account:

- The **email address** linked to the account is changed
- The **password** is changed
- **Two-factor authentication (2FA) is disabled**

## What is paused during Security Mode?

For **12 hours** after the qualifying credential change, the account **cannot**:

- **Withdraw funds** from the GoMining wallet
- **Sell miners**

Everything else works as usual during the hold:

- Miners keep mining
- Rewards keep arriving in the virtual wallet
- Deposits are credited normally
- Convert, purchases, Simple Earn, Miner Wars, Instant Funds positions already open, VIP progression — unaffected

Do not tell users their **rewards stop** or their **account is frozen** during Security Mode — only withdrawals and miner sales are held; everything else is fine.

## How does a user know Security Mode is active?

The **withdrawal screen** and the **miner-selling screen** show the message **"Your account is in security mode"** with a **countdown** of the time left in the 12-hour hold.

If the user reports seeing this message and asks what it means, the answer is Security Mode — do not tell them their account is blocked, restricted, or under investigation. It's the standard 12-hour post-credential-change hold and it lifts automatically at the countdown's end.

## Can the hold be lifted sooner?

**Yes.** The user contacts the GoMining support team via **live chat on app.gomining.com** or by email at **support@gomining.com**. Once support confirms the request is coming from the account owner, they can restore access before the 12-hour countdown ends.

When a user asks *"can I remove Security Mode faster?"*, direct them to GoMining support — that's the only path to lift it early.

## "I made the change myself — why is my account still on hold?"

Security Mode is applied to every account, no exceptions. Changing an email, a password, or 2FA is the **first move an attacker makes** after getting into an account, so the 12-hour pause gives the real owner a window to react if the change wasn't theirs. When it *was* the user, support can confirm that on request and lift the hold early (see above).

Reassure the user that this is not a punishment or a sign of suspicion, and that miners keep mining and rewards keep arriving during the hold — only withdrawals and miner sales are held.

## Assistant guardrails

- Do not call Security Mode a "ban", "freeze", "block", "restriction", or "account lock" — it is a **12-hour hold on withdrawals and miner sales specifically**, everything else works.
- Do not invent other triggers — the only three that start Security Mode are **email change**, **password change**, and **2FA disable**. Do not extend to "login from a new device", "KYC change", "large deposit", "IP change", etc. — those are not documented triggers.
- Do not invent other paused actions — only **withdrawals** and **miner sales** are paused. Do not tell users Simple Earn, mining, deposits, Convert, or Instant Funds pause during Security Mode.
- The hold is **fixed at 12 hours** and lifts automatically. Do not describe it as "up to 24/48/72 hours" or as needing manual review by default — the automatic countdown is the standard path.
- **Support can lift it early** on request once they confirm the owner's identity — this is the documented shortcut; contact GoMining support (and mention **support@gomining.com** as the second channel).
- If a user asks whether disabling 2FA now will trigger a hold — yes, it will; that's the third trigger.
- If a user asks whether re-enabling 2FA after a disable triggers another hold — this isn't documented; don't guess. Escalate if they need a definitive answer.
