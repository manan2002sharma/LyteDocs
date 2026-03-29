# Stop-Loss

A stop-loss automatically sells your position when the market price drops to a level you set. It's the easiest way to limit your downside on a trade.

---

## Setting a Stop-Loss

### After Buying

When you buy shares, the success screen shows a **Set Stop-Loss** button. Tap it to immediately set a stop-loss for the position you just bought.

### From Positions

1. Open **Positions**
2. Tap a position
3. Tap **Set Stop-Loss** (or send `/sl`)

### Via Command

Send `/sl` and follow the prompts.

---

## How to Configure

1. **Choose a trigger method:**
   - **Percentage drop** — e.g. "sell if price drops 30% from current price"
   - **Custom price** — e.g. "sell if price drops below $0.45"

2. **Review the trigger price** — the bot shows exactly what price will trigger the sell.

3. **Confirm** — your stop-loss is now active.

---

## Example

You buy YES shares at $0.70. You set a stop-loss at 20% drop.

- Trigger price: $0.70 × (1 - 0.20) = **$0.56**
- If the YES price drops to $0.56, your shares are automatically sold at market price.

---

## How It Works Internally

The stop-loss monitor subscribes to the Polymarket price feed for your token via WebSocket. When a `price_change` event drops to your trigger price, the bot places a **GTC limit sell order** at just above floor price ($0.01).

This means the sell executes at the best available market price at that moment.

---

## Viewing Active Stop-Losses

Your active stop-losses are visible in the position detail view. Each shows:

- Token / Market
- Trigger price
- Shares it will sell

---

## Cancelling a Stop-Loss

1. Open **Positions** → tap the relevant position
2. Tap **Cancel Stop-Loss**

Or from the `/sl` command, select the active stop-loss and cancel it.

---

## Notes

- You can only have one stop-loss per position token.
- If a market resolves while a stop-loss is active, the stop-loss is automatically removed.
- Stop-losses are stored in the database and survive bot restarts.
- The price feed is real-time via WebSocket — stop-losses fire within seconds of the trigger.

---

## Combined SL + TP Flow

After buying, you can set both a stop-loss and take-profit in sequence from the success screen. This creates a fully automated risk management bracket for your position. See [Take-Profit](take-profit.md).
