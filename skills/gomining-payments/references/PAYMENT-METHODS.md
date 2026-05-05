# Payment Methods Reference

## Overview

GoMining supports multiple payment methods for purchasing cryptocurrency and Digital Miners. Each method has different asset support, currencies, commission rates, and chargeback policies.

## Payment Methods

### Card Payment

| Attribute | Detail |
|-----------|--------|
| Type | Card payment (Visa/Mastercard) |
| Supported Assets | GMT |
| Currencies | EUR, USD |
| Chargebacks | Yes |
| Settlement | Instant |
| Use Case | Direct GMT purchases via debit/credit card |

### On-Ramp

| Attribute | Detail |
|-----------|--------|
| Type | Crypto on-ramp |
| Supported Assets | BTC, ETH, SOL, and other major cryptocurrencies |
| Currencies | EUR, USD |
| Chargebacks | No |
| Settlement | Near-instant |
| Use Case | Purchasing various cryptocurrencies with fiat |

### Open Banking

| Attribute | Detail |
|-----------|--------|
| Type | Direct bank transfer (PSD2) |
| Supported Assets | BTC, ETH, and other major cryptocurrencies |
| Currencies | EUR, HUF |
| Chargebacks | No |
| Settlement | Instant (SEPA Instant) or 1-2 days (SEPA) |
| Availability | EU only (France, Spain, Estonia, Belgium, Hungary) |
| Protocol | SEPA / SEPA Instant |

## Method Comparison

| Method | Best For |
|--------|----------|
| Open Banking | EU users seeking low fees |
| Card Payment | Quick card purchases |
| On-Ramp | Multi-crypto purchases |

## MNPL (Mine Now, Pay Later)

| Parameter | Value |
|-----------|-------|
| APR | 0% |
| Down Payment | 25% of miner price |
| Max Down Payment | $5,000 |
| Payment Schedule | Equal monthly installments |
| Price Range | $0 - $20,000 |
| Restricted | India and other territories |
| Miner Activation | Immediate upon purchase |
