# Wallet Tracker — Overview

The Wallet Tracker lets you monitor any Polymarket wallet and receive instant notifications whenever it trades.

---

## What Is It?

Lyte has a dedicated **Wallet Tracker bot** (separate from the main trading bot) that specializes in real-time wallet monitoring. Add any wallet address, give it a name, and get notified every time it buys or sells on Polymarket.

---

## Why Use It?

- **Follow smart money** — see what top traders are buying before you decide to trade
- **Monitor your own wallets** — get alerts when your external wallets trade
- **Find copy trade targets** — identify consistent performers before enabling copy trading
- **Research** — understand how specific wallets are positioned across markets

---

## Notification Format

When a tracked wallet trades, you receive a message like:

```
🔔 Alpha Trader

📈 BUY — Will Bitcoin exceed $100K by Dec 2025?
Outcome: YES
Shares: 500
Price: $0.68
Value: ~$340 USDC

🔗 [View Market]
```

Notifications arrive within seconds of the on-chain transaction being detected.

---

## Getting Started

Use the `/track` command (in the wallet tracker bot) to add your first wallet.

See: [Managing Tracked Wallets](managing.md)

---

## Integration with Copy Trading

Any wallet you track can be quickly added to [Copy Trading](../automation/copy-trading.md). From the main trading bot, you can directly copy trades from wallets you've been tracking.

---

## Integration with Leaderboard

The [Leaderboard](../tools/leaderboard.md) shows top-performing Polymarket traders. Each trader profile has a **Track Wallet** button that adds them directly to your tracker.

---

## How It Works Technically

The tracker subscribes to **ERC-1155 TransferSingle** events on Polygon via WebSocket for tracked wallet addresses. When a transfer from/to a known Polymarket exchange address is detected, it identifies the trade direction (BUY or SELL), fetches the market name and price, and sends the notification.

Detection latency is typically **under 5 seconds** from on-chain confirmation.
