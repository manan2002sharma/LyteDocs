# Deposit USDC

Lyte uses **USDC.e** (bridged USDC) on Polygon for all trades. You need to deposit funds before you can trade.

---

## Your Deposit Address

1. Open the main menu (send `/start` or tap **Main Menu**)
2. Tap **Deposit**
3. The bot shows your **Safe address** — this is where you send USDC.e

> Your Safe address is a Gnosis Safe smart contract on Polygon. It's your trading vault.

---

## Supported Asset

| Asset | Network | Contract |
|-------|---------|----------|
| USDC.e | Polygon | `0x2791Bca1f2de4661ED88A30C99A7a9449Aa84174` |

**Only send USDC.e on Polygon.** Do not send native USDC (Circle's USDC), ETH, MATIC, or assets on other networks.

---

## How to Get USDC.e on Polygon

**Option A — Bridge from another chain:**
Use [Polygon Bridge](https://wallet.polygon.technology/polygon/bridge) to bridge USDC from Ethereum to Polygon.

**Option B — Buy directly on Polygon:**
Use a DEX like QuickSwap or a CEX that supports Polygon withdrawals (Binance, OKX, etc.).

**Option C — Transfer from another Polygon wallet:**
If you already hold USDC.e on Polygon, just send it directly to your Safe address.

---

## Checking Your Balance

Use `/balance` or tap **Balance** in the main menu to see your current USDC.e balance.

---

## Minimum Deposit

There is no enforced minimum deposit. However, the cheapest trades typically require **$1–5 USDC** to be meaningful.

---

## Notes

- Deposits are detected automatically once confirmed on Polygon.
- There is no deposit fee from the bot. Standard Polygon network fees apply (usually fractions of a cent).
- Your funds are held in your own Gnosis Safe — the bot cannot withdraw them without your signed transactions.
