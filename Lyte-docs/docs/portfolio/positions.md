# Positions

Your positions are the prediction market shares you currently hold. View them to track your portfolio, monitor P&L, and sell when ready.

---

## Viewing Positions

1. Open the main menu
2. Tap **Positions** (or send `/positions`)

Your positions are split into three tabs:

| Tab | Description |
|-----|-------------|
| **Open** | Active positions in markets still trading |
| **Redeemable** | Winning positions in resolved markets — claim your $1.00/share |
| **Closed** | Positions you've sold or that expired worthless |

---

## Open Positions

For each open position you'll see:

- Market title and outcome (YES/NO)
- Shares held
- Current price
- Current value (shares × price)
- Your average buy price
- Unrealized P&L (profit or loss)

Tap any position to:
- **Sell** — open the sell flow for that position
- **View Market** — open the market detail page
- **Share PNL Card** — generate a shareable image of your P&L

---

## Redeemable Positions

When a market resolves, winning shares are worth **$1.00 each**. These appear in the **Redeemable** tab.

Tap **Redeem** to collect your USDC. Or enable [Auto Redeem](../automation/auto-redeem.md) to redeem automatically every hour.

---

## Closed Positions

The **Closed** tab shows your trade history — positions you've already sold or that resolved against you.

For each closed position:
- Entry price vs. exit price
- Realized P&L
- Date closed

---

## PNL Cards

Every position has a **Share PNL Card** button that generates a shareable image card showing:

- Market name and outcome
- Your profit/loss in dollars and percentage
- Amount invested
- Current position value
- Bot branding

Great for sharing wins on social media.

---

## Notes

- Positions are fetched in real-time from Polymarket's Data API.
- Prices update each time you load the positions screen.
- Shares with a value below $0.01 may not appear in the list.
