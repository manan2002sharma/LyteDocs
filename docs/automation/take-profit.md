# Take-Profit

A take-profit automatically sells your position when the market price rises to a target you set. Lock in profits without watching the screen.

---

## Setting a Take-Profit

### After Buying

The buy success screen shows a **Set Take-Profit** button. Tap it to set a take-profit immediately after your trade.

### From Positions

1. Open **Positions**
2. Tap a position
3. Tap **Set Take-Profit** (or send `/tp`)

---

## How to Configure

1. **Choose a trigger method:**
   - **Percentage gain** — e.g. "sell if price rises 40% from current price"
   - **Custom price** — e.g. "sell if price reaches $0.85"

2. **Review the trigger price** — the bot shows the exact price that will trigger the sell.

3. **Confirm** — your take-profit is now active.

---

## Example

You buy YES shares at $0.60. You set a take-profit at 50% gain.

- Trigger price: $0.60 × (1 + 0.50) = **$0.90**
- When the YES price rises to $0.90, your shares are automatically sold.
- You lock in a **$0.30/share** profit (50% gain).

---

## How It Works

The take-profit monitor uses the same Polymarket WebSocket price feed as stop-losses. When a `price_change` event reaches your trigger price, the bot places a **GTC limit sell order**.

---

## Combining Stop-Loss + Take-Profit

For full automation, set both on the same position:

- **Stop-Loss at -20%** — limits downside
- **Take-Profit at +50%** — locks in upside

When either triggers, the other is automatically cancelled. This is called a **bracket order**.

The combined SL + TP setup flow is available directly from the buy success screen — tap **Set Stop-Loss**, complete it, then immediately set the take-profit.

---

## Cancelling a Take-Profit

1. Open **Positions** → tap the relevant position
2. Tap **Cancel Take-Profit**

---

## Notes

- You can only have one take-profit per position token.
- Take-profits survive bot restarts (stored in the database).
- If both SL and TP are set, whichever triggers first cancels the other.
- For markets priced near $0.99, take-profits above $0.99 will not trigger (prices are capped).
