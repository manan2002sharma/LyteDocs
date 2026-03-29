# Buying Shares

Buying shares in a prediction market means you are taking a position on an outcome (YES or NO). If you're right when the market resolves, each share pays out $1.00 USDC.

---

## How to Buy

### Method 1 — Search for a Market

1. Send the name of a market as a text message (e.g. `"Bitcoin ETF"` or `"US election"`)
2. The bot returns matching markets from Polymarket
3. Tap on a market to see its outcomes
4. Tap **YES** or **NO** to start a buy

### Method 2 — Browse Markets

1. Tap **Markets** from the main menu
2. Browse active markets by category
3. Select a market and choose an outcome

---

## Placing a Buy Order

After selecting an outcome:

1. **Choose an amount** — tap one of your preset amounts ($10, $25, $50, $100) or type a custom amount
2. **Review the order** — the bot shows:
   - Current market price
   - Number of shares you'll receive
   - Worst-case buy price (your price + slippage setting)
   - Platform fee (0.5%)
3. **Confirm** — tap **Confirm Buy** to execute

The order is a **Fill-or-Kill (FOK) market order**. It executes immediately at the best available price, up to your slippage limit.

---

## Buy Presets

You can customize your 4 preset buy amounts in [Settings](../settings/settings.md).

Default presets: **$10 / $25 / $50 / $100**

---

## Slippage

Slippage protects you from buying at a worse price than expected. The default is **10 cents** above the current market price.

Example: If a YES share is priced at $0.65, your worst-case buy price is $0.75. If the market price spikes above $0.75 before your order fills, the order is cancelled.

You can adjust slippage in [Settings](../settings/settings.md).

---

## After Buying

Once your order fills, you'll see a success message with:
- Shares purchased
- Average fill price
- Total cost

From the success screen you can immediately:
- **Set a Stop-Loss** — automatically sell if price drops
- **Set a Take-Profit** — automatically sell when price rises

---

## Platform Fee

A **0.5% fee** is charged on every trade. This fee is taken from the USDC you spend.

10% of the fee is returned to you as **cashback**. See [Rewards](../rewards/overview.md).
