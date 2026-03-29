# Selling Shares

You can sell your shares at any time before a market resolves to lock in profits or cut losses.

---

## How to Sell

### From Positions

1. Open the main menu and tap **Positions**
2. Find the position you want to sell
3. Tap the position to open the detail view
4. Tap **Sell**
5. Choose a percentage to sell (your presets, or type a custom %)
6. Confirm

### From Market Search

1. Search for the market or browse to it
2. Tap the outcome you hold
3. The bot detects your position and shows the sell option

---

## Sell Presets

You can customize 4 preset sell percentages in [Settings](../settings/settings.md).

Default presets: **25% / 50% / 75% / 100%**

To sell everything: use the **100%** preset.

---

## How Sell Orders Work

Sell orders are **Fill-or-Kill (FOK) market orders** that execute immediately at the best available price.

- You specify a **percentage** of your position to sell (not a fixed share count)
- The bot calculates the exact shares based on your current holdings
- No slippage setting applies to sells — only buys are slippage-protected

---

## Sell Price

The bot sells at the current market bid price. Because prediction market prices range from $0.01 to $0.99, liquidity can vary. For very illiquid markets, the fill price may be significantly worse than the displayed price.

---

## After Selling

Once your sell order fills, you'll see:
- Shares sold
- USDC received
- Net proceeds after fees

Your USDC is returned to your Safe wallet immediately.

---

## Selling Resolved Markets

If a market has resolved and you hold winning shares, do **not** use the sell flow — use [Redeem](../portfolio/redeem.md) instead. Redeeming pays out the full $1.00 per share with no fee.
