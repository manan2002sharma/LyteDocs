# Managing Tracked Wallets

---

## Adding a Wallet

**In the Wallet Tracker bot:**

1. Send `/track`
2. Enter the wallet address (e.g. `0x1234...abcd`)
3. Enter a name for it (e.g. `"Alpha Trader"`)

The bot confirms the wallet is now being monitored.

**From the Leaderboard (main trading bot):**

1. Open **Leaderboard**
2. Find a trader you want to track
3. Tap **Track Wallet**
4. Optionally enter a custom name

**From a referral deep link:**

Leaderboard profiles shared via Telegram deep links include a **Track** button.

---

## Viewing Your Wallets

Send `/wallets` in the Wallet Tracker bot to see all your tracked wallets with pagination (3 per page).

Each card shows:
- Wallet name
- Wallet address (truncated)
- Status (Active / Paused)

---

## Pausing & Resuming Notifications

If you want to stop receiving notifications for a wallet temporarily without removing it:

1. Open `/wallets`
2. Find the wallet
3. Tap **Pause**

Tap **Resume** to re-enable notifications.

> Pausing affects notifications only — copy trade will still function for paused wallets.

---

## Renaming a Wallet

1. Open `/wallets`
2. Find the wallet
3. Tap **Rename**
4. Type the new name

---

## Deleting a Wallet

1. Open `/wallets`
2. Find the wallet
3. Tap **Delete**
4. Confirm with **Yes, Delete**

Deleting removes the wallet from monitoring and stops all notifications.

> If a deleted wallet is also a copy trade leader, copy trading for that wallet continues until you separately delete the copy trade config.

---

## Cancelling the Add Flow

If you started `/track` but want to cancel before completing it, send `/cancel`.

---

## Limits

There is no hard limit on the number of wallets you can track, but monitoring too many wallets may slow notification delivery.

---

## Commands Reference

| Command | Description |
|---------|-------------|
| `/track` | Start adding a new wallet |
| `/wallets` | View and manage all tracked wallets |
| `/cancel` | Cancel an in-progress `/track` flow |
| `/help` | Show all available commands |
