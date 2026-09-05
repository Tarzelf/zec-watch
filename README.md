# ZEC Watch / Flow

One-page swap into Zcash. You send USDC, ETH, BTC, or SOL. You receive ZEC on a transparent address. No account.

Live API: [NEAR Intents 1Click](https://docs.near-intents.org/).

## Run it

Open `index.html` or turn on GitHub Pages for this repo.

```bash
python3 -m http.server 8080
```

## Fees

Default listed fee is **20 bps (0.20%)** via `appFees`.
NEAR 1Click keeps half. You keep half — **10 bps net** — once you set a NEAR account in the page settings.

Without a 1Click JWT the protocol also adds ~10 bps. Solver spread is on top and shown as all-in rate.

Set `FEE_NEAR` in the page (gear) before taking live volume. Until then fees go nowhere useful.

## Honest limits

- Destination is a **transparent t1/t3** ZEC address. Shield after in Zodl / Zashi / YWallet.
- Refund address must be on the **same chain** as the asset you send.
- Send the **exact** quoted amount to the deposit address.

## What this is not

Not a ZEC AMM. Not shielded-native DeFi. Those wait on ZSAs.
