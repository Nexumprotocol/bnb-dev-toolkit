# 🛠️ BNB Dev Toolkit

> Open-source developer toolkit for BNB Smart Chain — built for the BSC Testnet ecosystem.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![BNB Chain](https://img.shields.io/badge/BNB%20Chain-Testnet-F0B90B?logo=binance)](https://www.bnbchain.org)
[![Live Demo](https://img.shields.io/badge/Live%20Demo-Netlify-00C7B7?logo=netlify)](https://bnb-dev-toolkit.netlify.app)
[![Chain ID](https://img.shields.io/badge/Chain%20ID-97-blue)](https://testnet.bscscan.com)

-----

## 🎯 Problem

BSC developers waste significant time during the development cycle on repetitive, fragmented setup tasks:

- **Hunting testnet faucets** — 8+ faucets scattered across different sites, no single status view
- **Checking gas prices** — no lightweight, always-on gas tracker for testnet
- **Manual MetaMask setup** — typing RPC URLs, chain IDs, and explorers manually every time
- **Contract verification** — no quick way to check if a contract is deployed without BSCScan
- **Network monitoring** — no simple health dashboard for testnet RPC endpoints

Every new developer onboarding to BSC Testnet goes through the same painful multi-tab setup. **BNB Dev Toolkit solves all of this in one place.**

-----

## ✅ Solution — 5 Tools, One Dashboard

### 🚰 Tool 1: Faucet Hub

All 8 active BSC Testnet faucets aggregated in one view.

- Live status indicators (Online / Verify / Offline)
- Filter by: No Requirements, High Amount, Discord
- See claim amounts and cooldowns at a glance
- Paste wallet address once, apply to all

### ⛽ Tool 2: Live Gas Tracker

Real-time gas price data pulled directly from BSC Testnet RPC.

- Slow / Standard / Fast tiers with Gwei values
- Estimated USD cost per transaction
- Live block number
- Visual gas history chart (last 20 polls)

### 📡 Tool 3: Network Health Monitor

Live health metrics for BSC Testnet infrastructure.

- Block height with sync status
- RPC latency (ms) with trend bars
- Peer count monitoring
- Multi-endpoint RPC table with individual latency checks
- One-click copy for all RPC URLs

### 🔍 Tool 4: Contract Checker

Instant contract verification on BSC Testnet without BSCScan.

- Detect if address is a contract or EOA (wallet)
- Bytecode size in bytes
- tBNB balance
- Transaction count
- Direct link to BSCScan Testnet

### 🧰 Tool 5: MetaMask Config Generator

One-click network setup for MetaMask — no manual typing.

- BSC Testnet, BSC Mainnet, opBNB Testnet, opBNB Mainnet
- `wallet_addEthereumChain` integration
- Copy individual parameters (RPC URL, Chain ID, etc.)
- Works on desktop MetaMask + mobile in-app browser

-----

## 🚀 Live Demo

**<https://bnb-dev-toolkit.netlify.app>**

-----

## 📦 Tech Stack

|Layer   |Technology                                                               |
|--------|-------------------------------------------------------------------------|
|Frontend|Vanilla HTML5, CSS3, JavaScript (ES2020)                                 |
|Data    |BSC Testnet Public RPC (`eth_gasPrice`, `eth_blockNumber`, `eth_getCode`)|
|Hosting |Netlify (static, zero backend)                                           |
|Wallet  |MetaMask `wallet_addEthereumChain` API                                   |
|Fonts   |JetBrains Mono, Inter (Google Fonts)                                     |

**Zero dependencies. Zero build step. One file.**

-----

## 🗂️ Project Structure

```
bnb-dev-toolkit/
├── index.html        # Full application (single-file)
├── README.md         # This file
├── LICENSE           # MIT License
└── netlify.toml      # Netlify deployment config
```

-----

## 🔧 Local Development

```bash
# Clone the repo
git clone https://github.com/Nexumprotocol/bnb-dev-toolkit.git

# Open in browser — no build required
open index.html
```

Or serve locally:

```bash
npx serve .
# Visit http://localhost:3000
```

-----

## 🌐 Deploy Your Own

### Netlify (Recommended)

1. Fork this repo
1. Connect to [Netlify](https://netlify.com)
1. Deploy — done. No config needed.

### Manual

Upload `index.html` to any static hosting (GitHub Pages, Vercel, Cloudflare Pages).

-----

## 📡 RPC Endpoints Used

|Network      |RPC URL                                   |Chain ID|
|-------------|------------------------------------------|--------|
|BSC Testnet  |`https://bsc-testnet-rpc.publicnode.com`  |97      |
|BSC Mainnet  |`https://bsc-rpc.publicnode.com`          |56      |
|opBNB Testnet|`https://opbnb-testnet-rpc.publicnode.com`|5611    |
|opBNB Mainnet|`https://opbnb-rpc.publicnode.com`        |204     |

-----

## 🗺️ Roadmap

### v1.0 (Current)

- [x] Faucet Hub — 8 faucets aggregated
- [x] Live Gas Tracker — real RPC data
- [x] Network Health Monitor — multi-endpoint
- [x] Contract Checker — bytecode + balance
- [x] MetaMask Config — one-click add

### v1.1 (Planned)

- [ ] Wallet balance checker (tBNB balance lookup)
- [ ] Transaction decoder (paste tx hash, get human-readable breakdown)
- [ ] ABI encoder / decoder
- [ ] Faucet auto-status pinger (real uptime monitoring)

### v2.0 (Future)

- [ ] opBNB full tool support
- [ ] BNB Greenfield testnet tools
- [ ] Browser extension version
- [ ] REST API for faucet status data

-----

## 🤝 Contributing

Contributions are welcome. Please open an issue first to discuss what you’d like to change.

```bash
# Fork → Branch → PR
git checkout -b feature/your-feature-name
```

-----

## 📄 License

MIT © [Nexum Protocol](https://github.com/Nexumprotocol)

-----

## 🔗 Links

- [BNB Chain Official](https://www.bnbchain.org)
- [BNB Chain Grants](https://www.bnbchain.org/en/grants)
- [BSCScan Testnet](https://testnet.bscscan.com)
- [BNB Chain Discord](https://discord.com/invite/bnbchain)

-----

<p align="center">Built for the BNB Chain developer community 🟡</p>