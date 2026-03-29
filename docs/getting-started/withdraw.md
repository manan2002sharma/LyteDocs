# Withdraw Funds

You can withdraw your USDC.e balance to any Polygon wallet at any time.

---

## How to Withdraw

1. Open the main menu
2. Tap **Withdraw** (or send `/withdraw`)
3. Enter the amount you want to withdraw (e.g. `50` for $50 USDC)
4. Enter the destination Polygon wallet address
5. Confirm the withdrawal

The funds will be sent from your Safe to the destination address.

---

## Fees

Withdrawals are **gasless** — processed via Polymarket's relay infrastructure. There is no gas fee charged to you.

A small platform fee may apply (same 0.5% fee as trades).

---

## Notes

- You can only withdraw USDC.e that is not currently committed to open orders.
- Positions (shares you hold) cannot be withdrawn directly — you must sell them first.
- Redeemable positions from resolved markets can be [redeemed](../portfolio/redeem.md) to USDC before withdrawing.
- Minimum withdrawal amount: $0.01 USDC.

---

## Withdrawing Everything

To withdraw your full balance, enter your entire available USDC balance. The bot shows your current balance in the withdrawal prompt.

---

## Troubleshooting

**"Insufficient balance"?**
Your available balance doesn't cover the requested amount. Check `/balance` to see your current funds.

**Transaction pending for a long time?**
Polygon transactions typically confirm in under 5 seconds. If delayed, it may be a temporary network issue — your funds are safe.
