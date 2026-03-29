# Pending Orders

Pending orders are **limit orders** you've placed that haven't been filled yet. They stay open on the Polymarket order book until they are filled or you cancel them.

---

## Viewing Pending Orders

1. Open the main menu
2. Tap **Orders** (or send `/orders`)

You'll see a list of all your open orders with:
- Market name and outcome (YES/NO)
- Order type (Buy/Sell)
- Limit price
- Order size (USDC or shares)
- Time placed

---

## Cancelling an Order

1. Open **Orders**
2. Tap the order you want to cancel
3. Tap **Cancel Order**
4. Confirm

Cancelled orders release any reserved USDC back to your available balance.

---

## How Limit Orders Work

When you place a limit buy at $0.60:
- Your order sits on the order book
- If someone is willing to sell at $0.60 or lower, your order fills
- You receive shares at your limit price or better

Limit orders are **GTC (Good Till Cancelled)** — they don't expire automatically.

---

## Copy Trade and Stop-Loss Orders

Orders placed by the [Copy Trading](../automation/copy-trading.md) system and [Stop-Loss](../automation/stop-loss.md) automation also appear in your pending orders list. You can cancel these manually, but doing so may interfere with the automation.

---

## Notes

- Market orders (the standard buy/sell flow) are FOK (Fill-or-Kill) and either fill instantly or fail. They never appear as pending orders.
- Only GTC limit orders appear in the pending orders list.
