# Nombo Alpha Desk

A fast beta dashboard for the MetaMask Agent Wallet Early Access program.

Nombo Alpha Desk is a public-facing prototype showing how a voice/chat agent can sit on top of MetaMask Agent Wallet to:

- monitor wallet state,
- inspect Hyperliquid perps capability,
- run paper-trading strategy experiments,
- track beta issues and product feedback,
- maintain a build checklist for the Nombo + MetaMask Agent Wallet project.

## Current status

- MetaMask Agent Wallet authenticated in Nombo.
- Wallet initialized as server-wallet + Guard Mode.
- Wallet funded on Ethereum mainnet.
- Hyperliquid venue and markets are visible through the Agent Wallet CLI.
- Hyperliquid perps account is not funded yet.
- Bridge quote from Ethereum ETH to Arbitrum USDC works.
- Bridge execution currently fails with `PollingBlockTracker - no idleTimeTracker specified`, which is tracked as beta feedback.
- First paper/backtest scans have been created from Hyperliquid public market data.

## Safety

This project is not financial advice. It is a beta dashboard for research, testing, and product feedback. Live fund movement or trades require explicit human approval.
