# Redeem Resolved Markets

When a Polymarket market resolves, each winning share is worth exactly **$1.00 USDC**. Redemption converts your winning shares into USDC in your wallet.

---

## Manual Redemption

1. Open the main menu
2. Tap **Positions** → switch to the **Redeemable** tab
3. Tap **Redeem All** to redeem all winning positions at once

Or send `/redeem` to redeem all redeemable positions in one step.

---

## Auto Redeem

Don't want to manually redeem? Enable **Auto Redeem** in [Settings](../settings/settings.md) to have the bot automatically redeem all your winning positions every hour.

See: [Auto Redeem](../automation/auto-redeem.md)

---

## What Happens During Redemption

1. The bot identifies all your positions in resolved markets where you hold the winning outcome.
2. For each position, it submits a redemption transaction via Polymarket's relay (gasless).
3. USDC is deposited directly into your Safe wallet.
4. You receive a Telegram notification confirming the amount redeemed.

---

## Fees

Redemption is **free** — no platform fee is charged on redemptions. You receive the full $1.00 per winning share.

---

## Losing Positions

If you hold shares in the losing outcome of a resolved market (e.g. you bought YES but NO won), those shares expire worthless. They move to the **Closed** tab in your positions view.

---

## Notes

- Only positions in **fully resolved** markets can be redeemed.
- Markets in the redeemable tab show the winning outcome (YES or NO) and your total payout.
- If a market is disputed or in review, redemption may be delayed until resolution is confirmed.
