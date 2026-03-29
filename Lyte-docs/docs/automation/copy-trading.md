# Copy Trading

Copy trading automatically mirrors trades from any Polymarket wallet. When a wallet you're copying buys or sells, the bot executes the same trade in your account.

---

## Getting Started

1. Open the main menu
2. Tap **Copy Trade** (or send `/copytrade`)
3. Tap **+ Add** to set up a new copy
4. Enter the wallet address you want to copy
5. Configure your strategy (see below)
6. Confirm

---

## Strategy Types

Choose how much to invest per copied trade:

| Strategy | How It Works |
|----------|-------------|
| **Fixed Amount** | Invest a fixed USDC amount per trade (e.g. $25 per trade) |
| **Percentage** | Copy the same number of shares as a % of the leader's position (e.g. 50% of leader's shares) |
| **Portfolio-Weighted** | Scale your investment proportionally to the leader's trade size relative to their portfolio |

---

## Buy Price Modes

Control the price you're willing to pay when copying a buy:

| Mode | Behavior |
|------|----------|
| **Any** | Buy at up to $0.99 (always fills) |
| **Exact** | Match the leader's last trade price exactly |
| **N% slippage** | Accept up to N% above the leader's price (e.g. 5% slippage) |

---

## Sell Price Modes

| Mode | Behavior |
|------|----------|
| **Any** | Sell at as low as $0.01 (always fills) |
| **Exact** | Match the leader's sell price exactly |
| **N% slippage** | Accept up to N% below the leader's price |

When the leader sells, the bot sells **100% of your position** in that market.

---

## Managing Copy Trades

Send `/copytrade` or tap **Copy Trade** in the main menu to see all your active copy configs.

For each config you can:
- **Edit** — change strategy, amounts, price mode
- **Pause / Resume** — temporarily disable without deleting
- **Delete** — remove the copy trade

---

## How It Works

1. Lyte monitors the leader wallet in real-time via blockchain event subscriptions.
2. When the leader makes a trade (detected within seconds via on-chain events), the bot evaluates your copy config.
3. A **GTC limit order** is placed at your configured price.
4. You receive a notification when the copy trade executes.

> Copy trades use **limit orders** (not market orders) to avoid excessive slippage on illiquid markets.

---

## Latency

Copy trades fire within a few seconds of the on-chain event being detected. However, by the time your order is placed, the market price may have moved. Use the price mode settings to control how aggressively you chase the leader's price.

---

## Finding Wallets to Copy

Use the [Leaderboard](../tools/leaderboard.md) to discover top-performing traders. From the leaderboard, you can tap **Copy Trade** directly on any trader's profile to start copying them.

---

## Notes

- You can copy multiple wallets simultaneously.
- Copy trades do not trigger stop-loss or take-profit automation on the copied positions.
- Minimum trade size: depends on your strategy amount setting.
- If your balance is too low to execute a copy trade, it is silently skipped.
