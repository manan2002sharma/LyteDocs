# Setup & Wallet Creation

When you use Lyte for the first time, the bot automatically creates a secure wallet for you. This only needs to happen once.

---

## Step 1 — Start the Bot

Send `/start` to the bot in Telegram.

If someone referred you, use their referral link instead:

```
https://t.me/YourBotUsername?start=r_XXXXXXXX
```

Using a referral link links your account to the referrer so they earn commissions on your trades.

---

## Step 2 — Wallet Setup (Automatic)

The bot will automatically:

1. **Create a Privy embedded wallet** — a private key generated and managed server-side.
2. **Derive a Gnosis Safe** — a smart contract account on Polygon that holds your USDC.
3. **Deploy your Safe** — on-chain deployment via Polymarket's gasless relay (no gas needed).
4. **Set token approvals** — allows the CLOB and relay to interact with your USDC.
5. **Create CLOB API credentials** — signs trades on the Polymarket order book.

This process takes **10–30 seconds**. Do not send any messages while it runs.

---

## Step 3 — Deposit USDC

Once setup is complete, you'll see the main menu. Your wallet is ready but empty.

Tap **Deposit** to get your wallet address and start funding it.

See: [Deposit USDC](deposit.md)

---

## Your Wallet Architecture

| Component | What It Is |
|-----------|-----------|
| **EOA (Externally Owned Account)** | Your Privy private key — signs CLOB orders |
| **Safe (Smart Account)** | Your on-chain vault — holds USDC, executes trades |
| **CLOB Credentials** | API key pair for the Polymarket order book |

> **Security note:** Your private key is stored in Privy's secure server wallet infrastructure. Lyte never logs or exposes your key.

---

## Referral Links

If you want to share your referral link after setup:

1. Open the main menu
2. Tap **Rewards** (or send `/referral`)
3. Copy your unique referral link

Anyone who signs up through your link earns you **60% of their trade fees** and **10% from their referrals**.

---

## Troubleshooting

**Setup seems stuck?**
Send `/start` again. The bot detects partial setup and resumes from the last completed step.

**"Please complete wallet setup first"?**
Your wallet isn't fully set up yet. Send `/start` and wait for the "Setup complete!" message before trading.
