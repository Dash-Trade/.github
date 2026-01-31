# Dash Trade

![Dash Trade Banner](./og-banner.png)

Dash Trade is a perpetual futures trading dApp on Base with account abstraction.
It provides real-time oracle pricing, advanced order types, and automated execution. This repository
contains the smart contracts, backend services, and frontend web app.

## Features

- **Real-time oracle prices**: Pyth Network feeds with signed prices for on-chain verification
- **Multi trading pair**: Support crypto, forex, indices, commodities, stocks
- **Indonesia stocks**: Support IHSG, BBCA, and BBRI for trading
- **High leverage trading**: Up to 100x on majors (per protocol limits)
- **Advanced orders**: Limit, stop-loss, take-profit, and grid trading
- **Gasless UX**: Relay service with USDC gas payments
- **Automated execution**: Keepers for limit orders, TP/SL, and liquidations
- **One Tap Profit**: Short-term price prediction betting settlement
- **TradingView charts**: Oracle overlay and live PnL updates
- **Privy wallets**: Email/social login with embedded smart wallets

## Projects

- `dash-sc` - Smart contracts (perps, staking, vaults)
- `dash-be` - Backend oracle, relayer, and trading automation (Express)
- `dash-fe` - Frontend web app (Next.js)

## Quick Start

Follow the README inside each project:

- Smart contracts: `dash-sc/README.md`
- Backend: `dash-be/README.md`
- Frontend: `dash-fe/README.md`

## Local Dev (Short Version)

```bash
# Backend
cd dash-be
npm install
cp .env.example .env
npm run dev

# Frontend
cd ../dash-fe
npm install
cp .env.example .env
npm run dev
```

## Notes

- Make sure contract addresses, chain ID, and RPC URLs are consistent across `.env` files.
- Backend signer/keeper wallets must be granted roles in the contracts and funded for execution.
