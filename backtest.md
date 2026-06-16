# Nombo Alpha Desk — First Backtest Snapshot

Generated: 2026-06-16T21:30:49.984549Z

This is a rough 30-day 15-minute-candle research backtest using Hyperliquid public candles. It is for strategy triage only, not live-trade proof. It includes simple fee assumptions and does not fully model slippage, funding, margin, or liquidation mechanics.

## BTC
Window: 2026-05-17T21:30:00Z → 2026-06-16T21:30:00Z (2881 candles)

- EMA 12/48 crossover, 2x notional simulation: return -34.07%, trades 85, win rate 21.2%, max drawdown 37.59%
- 24-candle breakout, 8-candle hold, 2x notional simulation: return -47.03%, trades 129, win rate 41.1%, max drawdown 47.47%

## ETH
Window: 2026-05-17T21:30:00Z → 2026-06-16T21:30:00Z (2881 candles)

- EMA 12/48 crossover, 2x notional simulation: return -17.01%, trades 80, win rate 20.0%, max drawdown 36.08%
- 24-candle breakout, 8-candle hold, 2x notional simulation: return -48.12%, trades 115, win rate 36.5%, max drawdown 54.92%
