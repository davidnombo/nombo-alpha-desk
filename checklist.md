# Nombo Alpha Desk — Agent Wallet Checklist

Last updated: 2026-06-16

## Completed

- [x] Early Access approved.
- [x] MetaMask Agent Wallet CLI installed in Nombo sandbox.
- [x] Nombo authenticated with MetaMask Agent Wallet.
- [x] Agent Wallet initialized as server-wallet + Guard Mode.
- [x] Agent Wallet address confirmed: `0xb50ba1e05718f782a03412b095e606daf0fbd5f7`.
- [x] Wallet funded on Ethereum mainnet with ETH.
- [x] Wallet balance checked: approximately $305 in ETH on Ethereum mainnet.
- [x] Hyperliquid venue discovered through Agent Wallet.
- [x] Hyperliquid markets discovered through Agent Wallet.
- [x] Hyperliquid perps balance checked: $0.
- [x] Hyperliquid open positions checked: none.
- [x] First Nombo Alpha Desk dashboard shell built locally.
- [x] First paper strategy signals generated from Hyperliquid market data.
- [x] Bridge quote from Ethereum ETH to Arbitrum USDC tested successfully.
- [x] Bridge quote showed about 0.02 ETH to ~35.5 USDC on Arbitrum, with visible bridge fee around $0.31.
- [x] Bridge execution attempted.
- [x] Bridge execution failed safely with beta/tooling error: `PollingBlockTracker - no idleTimeTracker specified`.
- [x] Post-failure safety check: ETH balance unchanged, no pending wallet requests, quote remained unexecuted.
- [x] Retry with verbose attempted; same execution error reproduced.
- [x] PTY retry attempted; same execution error reproduced.
- [x] Hyperliquid perps deposit dry-run tested; it prepares correctly and expects USDC on Arbitrum.

## Current state

- Wallet has ETH on Ethereum mainnet.
- Wallet has no Arbitrum USDC.
- Wallet has no Hyperliquid perps balance.
- Bridge quote works, but bridge execution currently fails in this Nombo/mm environment.
- Hyperliquid deposit path appears to require USDC on Arbitrum and likely small ETH on Arbitrum for gas.

## Next options

### Option A — Manual funding from Coinbase / another wallet

Send to Agent Wallet address on Arbitrum:

- Small USDC amount on Arbitrum, suggested: $25–$50.
- Small ETH amount on Arbitrum for gas, suggested: a few dollars worth.

Then Nombo can deposit USDC into Hyperliquid perps and verify balance.

### Option B — Keep testing Agent Wallet bridge execution

Continue trying alternate swap/bridge routes and amounts, but current error appears to be a beta/tooling bug before transaction submission.

### Option C — Ask Consensys / Telegram

Report: bridge quote works but execution fails with `PollingBlockTracker - no idleTimeTracker specified`. Ask if there is a known workaround or required environment setting.

## Pending build tasks

- [ ] Add checklist into public/live Alpha Desk dashboard.
- [ ] Publish dashboard to GitHub Pages.
- [ ] Add paper trade ledger persistence.
- [ ] Add Telegram listener integration if Nombo developer enables read-only group ingest.
- [ ] Deposit small USDC into Hyperliquid once Arbitrum USDC/gas is available.
- [ ] Run first perps quote/dry-run after funding.
- [ ] Execute tiny live open/close only after explicit approval.
