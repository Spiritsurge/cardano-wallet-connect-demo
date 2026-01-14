# 🔗 Cardano Wallet Connect Demo (CIP-30)

A minimal, browser-based demo showing how to detect and connect to Cardano wallets using the **CIP-30 dApp Connector API** (`window.cardano`).

The demo:

- Detects installed Cardano wallets (Nami, Eternl, Flint, etc.)
- Requests wallet access via `enable()`
- Reads a used address from the wallet
- Converts the address from hex to **bech32** using Cardano Serialization Lib
- Does **not** move funds or sign transactions

This is intended as a **learning reference** and lightweight proof-of-concept.

---

## 🧠 What This Demo Covers

- CIP-30 wallet discovery (`window.cardano`)
- Wallet permission flow (`enable`)
- Reading used addresses
- Hex → bech32 address conversion
- Graceful handling of different wallet capabilities
- Pure HTML + JavaScript (no frameworks)

---

## 🧱 Tech Stack

- **Vanilla HTML / CSS / JavaScript**
- **CIP-30 Cardano dApp Connector**
- **@emurgo/cardano-serialization-lib (browser build via CDN)**

---

## 📁 Project Structure

cardano-wallet-connect-demo/
└── index.html

---

## ▶️ How to Run

### Option 1: Open directly (quickest)

1. Install a Cardano wallet browser extension (e.g. Nami, Eternl, Flint)
2. Open `index.html` in a modern browser
3. Click **Connect** on a detected wallet

> ⚠️ Some wallets require HTTPS. If detection fails, use Option 2.

---

### Option 2: Local dev server (recommended)

```bash
# using npm
npx serve .

# or with Python
python -m http.server
```
