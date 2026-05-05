# Deposit & Withdrawal Rules — GoMining Wallet

## Deposits

### General Rules

| Rule | Description |
|------|-------------|
| Wallet type | Custodial (Fireblocks-powered) |
| Address generation | Unique deposit address per asset/network |
| Minimum deposit | Varies by asset (see table below) |
| Confirmation | Requires blockchain confirmations before crediting |

### Minimum Deposit Amounts

| Asset | Min Deposit |
|-------|------------|
| BTC | 0.0001 BTC |
| USDT | 10 USDT |
| USDC | 10 USDC |
| GMT | 10–50 GMT (varies by network) |
| ETH | 10 (USD equivalent) |
| BNB | 10 (USD equivalent) |
| SOL | 10 (USD equivalent) |
| TON | 10 (USD equivalent) |

> **Warning:** Deposits below the minimum threshold may not be credited to your account.

---

## Withdrawals

### Minimum Withdrawal Amounts

| Asset | Min Withdrawal | Network Fee |
|-------|----------------|-------------|
| BTC | varies | 0.00006 BTC |
| USDT | 1–10 (by network) | 1–4 USDT |
| USDC | 0.0025–10 (by network) | 0.0005–1 USDC |
| GMT | 50–250 (by network) | 1–10 GMT |
| ETH | 0.0025 ETH | 0.0005 ETH |
| BNB | 0.013 BNB | 0.001 BNB |
| SOL | 0.02 SOL | 0.01 SOL |
| TON | 1 TON | 0.2 TON |

### Daily Withdrawal Limits

| Asset | User Daily Limit | System Daily Limit |
|-------|------------------|--------------------|
| USDT | 12,500 | 60,000 |
| USDC | 12,500 | 100,000 |
| ETH | 2.14 | 6.3 |
| BNB | 11.8 | 35 |
| SOL | 55 | 55 |
| TON | 3,050 | 30,700 |
| GMT | 37,500 | 1,000,000 |

> **Note:** If the system daily limit is reached, all user withdrawals for that asset are paused until the next day.

---

## Withdrawal Processing Times

| User Category | Account Age | Processing Delay |
|---------------|-------------|-----------------|
| New users | Less than 1 month | 15 minutes |
| Established users | 1 month or older | 2 minutes |

---

## KYC Requirements

### Access Without KYC Level-1

| Feature | Available? |
|---------|-----------|
| Deposits | Yes |
| Withdrawal of GOMINING | No |
| Withdrawal of USDT | No |
| Withdrawal of USDC | No |
| Withdrawal of BTC (instant) | No |
| Miner operations | No |
| Marketplace sales | No |

### Access With KYC Level-1

| Feature | Available? |
|---------|-----------|
| All deposits | Yes |
| All withdrawals | Yes |
| Miner operations | Yes |
| Marketplace sales | Yes |
| Full platform access | Yes |

> **Important:** Complete KYC Level-1 verification to unlock full wallet functionality including all withdrawal types, Miner operations, and marketplace access.

---

## BTC Withdrawal Rules

BTC withdrawals have special rules tied to mining and game reward balances.

### Before Any BTC Deposit

| Rule | Description |
|------|-------------|
| Mining rewards | Cannot be withdrawn |
| Game rewards | Cannot be withdrawn |
| Unlock condition | Create a personal miner to gain access |

### After BTC Deposit

| Rule | Description |
|------|-------------|
| Withdrawable amount | Only the portion exceeding accumulated mining rewards |
| Calculation | Withdrawal limit = Total BTC balance - Accumulated mining rewards |

**Example:**
- Mining rewards accumulated: 0.005 BTC
- User deposits: 0.01 BTC
- Total balance: 0.015 BTC
- Withdrawable amount: 0.01 BTC (the deposited amount, since it exceeds mining rewards)

---

## Fireblocks Architecture

The GoMining Wallet is built on Fireblocks infrastructure. Private keys are managed by Fireblocks — users do not control keys directly.

---

## Frequently Asked Questions

### Can I deposit without KYC?

Yes. Deposits are available without KYC verification. However, you will need KYC Level-1 to withdraw GOMINING, USDT, USDC, and BTC (instant).

### What happens if I deposit below the minimum?

Deposits below the minimum threshold may not be credited to your account. Always check the minimum deposit amount for your chosen asset and network before sending.

### Why is my withdrawal delayed?

Withdrawal processing time depends on your account age. New accounts (less than 1 month old) have a 15-minute delay. Established accounts (1 month or older) have a 2-minute delay.

### Can I withdraw BTC earned from mining?

Only after you have deposited BTC into your wallet. Before any BTC deposit, mining and game rewards cannot be withdrawn. After depositing, you can withdraw amounts exceeding your accumulated mining rewards.

### What is the system daily limit?

Each asset has a system-wide daily withdrawal limit shared across all users. If the system limit is reached, no further withdrawals for that asset are processed until the next day.

### What networks can I use for USDT?

USDT is supported on five networks: ERC-20 (Ethereum), BEP-20 (BSC), TRC-20 (Tron), Solana, and TON. Network fees and minimum withdrawals vary by network.

### Is the wallet custodial?

Yes. The GoMining Wallet is a custodial solution powered by Fireblocks. Private keys are managed by Fireblocks infrastructure, not by the user directly.

