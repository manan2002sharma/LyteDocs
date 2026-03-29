# Auto Redeem

Auto Redeem automatically claims your winnings from resolved prediction markets — every hour, without you having to do anything.

---

## Enabling Auto Redeem

1. Open the main menu
2. Tap **Settings**
3. Tap **Auto Redeem: OFF** to toggle it ON

The button turns green when enabled.

---

## How It Works

When Auto Redeem is enabled:
1. Every hour, the system checks all your positions in resolved markets.
2. For each winning position found, it submits a gasless redemption transaction.
3. USDC is deposited to your Safe wallet.
4. You receive a Telegram notification with the amount redeemed.

---

## Manual Redemption

You can also redeem manually at any time:
1. Tap **Positions** → **Redeemable** tab
2. Tap **Redeem All**

Or send `/redeem`.

---

## Fees

Redemptions are completely free — no platform fee is charged.

---

## Notes

- Auto Redeem only applies to fully resolved markets where your outcome won.
- If there are no redeemable positions, no notification is sent.
- Auto Redeem is disabled by default. Each user controls their own setting.
- If the bot is offline during an hourly cycle, it will process on the next cycle when it comes back online.
