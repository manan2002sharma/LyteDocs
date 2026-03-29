# Bot Settings

Customize the bot's behavior to match your trading style.

---

## Opening Settings

1. Open the main menu
2. Tap **Settings** (or send `/settings`)

---

## Buy Presets

Four preset buy amounts that appear as quick-tap buttons during the buy flow.

**Defaults:** $10 / $25 / $50 / $100

**To change a preset:**
1. Tap **Buy Presets** in Settings
2. Tap the preset slot you want to change
3. Enter the new dollar amount

You can set any positive dollar value (e.g. $5, $200, $1000).

---

## Sell Presets

Four preset sell percentages that appear as quick-tap buttons during the sell flow.

**Defaults:** 25% / 50% / 75% / 100%

**To change a preset:**
1. Tap **Sell Presets** in Settings
2. Tap the preset slot you want to change
3. Enter the new percentage (1–100)

---

## Slippage

Controls how much above the current market price you're willing to pay for a buy order.

**Default:** 10 cents (¢)

**Example:** If YES is priced at $0.65 and your slippage is 10¢, your worst-case buy price is $0.75.

Higher slippage = higher fill rate (fewer cancelled orders), but worse average price.
Lower slippage = better price, but orders may cancel if the market moves quickly.

**To change:**
1. Tap **Slippage: 10¢** in Settings
2. Enter a new value between 1 and 99 cents

> Slippage only applies to **buy orders**. Sell orders are not affected.

---

## Auto Redeem

Automatically redeems your winning positions from resolved markets every hour.

**Default:** OFF

**To toggle:**
1. Tap **Auto Redeem: OFF** in Settings
2. It turns **ON** (green indicator)

See: [Auto Redeem](../automation/auto-redeem.md)

---

## Settings Summary

| Setting | Default | Description |
|---------|---------|-------------|
| Buy Preset 1–4 | $10 / $25 / $50 / $100 | Quick-tap buy amounts |
| Sell Preset 1–4 | 25% / 50% / 75% / 100% | Quick-tap sell percentages |
| Slippage | 10¢ | Max price above market for buy FOK orders |
| Auto Redeem | OFF | Auto-claim winning resolved positions hourly |

---

## Resetting to Defaults

There is no one-tap reset. To restore defaults, manually set each value back to its default in the Settings menu.
