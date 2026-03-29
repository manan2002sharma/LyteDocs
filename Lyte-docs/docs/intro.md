---
sidebar_position: 0
---

# Introduction

Welcome to the official documentation for **Lyte** — a Telegram bot for trading on [Polymarket](https://polymarket.com), the world's largest prediction market platform.

---

## What is Lyte?

Lyte lets you trade prediction market shares on Polymarket directly through Telegram — no browser, no MetaMask, no gas fees needed. The bot manages a custodial wallet on your behalf (powered by Privy), executes trades via Polymarket's CLOB API, and gives you powerful tools like stop-loss, copy trading, and real-time wallet tracking.

---

## Key Features

| Feature | Description |
|---------|-------------|
| **Instant Trading** | Buy and sell shares in any Polymarket market directly in Telegram |
| **Stop-Loss** | Automatically sell when a position drops to your trigger price |
| **Take-Profit** | Automatically sell when your position hits a target price |
| **Copy Trading** | Mirror trades from any Polymarket wallet in real-time |
| **Wallet Tracker** | Get notified whenever tracked wallets trade |
| **Referral Rewards** | Earn 60% of fees from users you refer, 10% from their referrals |
| **Cashback** | Earn 10% cashback on every trade you make |
| **Auto Redeem** | Automatically redeem winning positions every hour |
| **Leaderboard** | Discover top traders and view their stats |
| **No Gas Fees** | All transactions are gasless via Polymarket's relay infrastructure |

---

## How It Works

```
You (Telegram) → Lyte Bot → Privy Server Wallet → Polymarket CLOB → Polygon
```

1. You send a message or tap a button in Telegram.
2. The bot uses your **Privy server wallet** (a non-custodial smart account you own).
3. Trades are signed and submitted to **Polymarket's CLOB** (Central Limit Order Book).
4. On-chain settlement happens on **Polygon** via a Gnosis Safe smart account.

---

## Getting Started

New? Start here: [Setup & Wallet Creation](getting-started/setup.md)

Already set up? Jump to: [Buying Shares](trading/buying.md)

---

## Support

Have questions or found a bug? Reach out on Telegram.
