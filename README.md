# Trading Strategy Repository

This repository contains trading strategies and their backtest results.

## Repository Structure

```
strategy/
├── forex/                     # Forex market strategies
│   ├── 1h/                   # 1-hour timeframe strategies
│   │   └── 4h_trend_1h_confirm.pine
│   └── 5m/                   # 5-minute timeframe strategies
├── backtest_results/         # Backtest results from TradingView
│   └── forex/
│       └── 4h_trend_1h_confirm/
│           ├── screenshots/   # Performance charts and equity curves
│           └── metrics/      # CSV/JSON files with performance metrics
└── docs/                     # Strategy documentation
    └── forex/
        └── 4h_trend_1h_confirm.md

```

## Workflow

1. Develop strategy in Pine Script files under respective market/timeframe folders
2. Test strategy in TradingView
3. Save backtest results:
   - Take screenshots of performance charts
   - Export performance metrics
   - Document findings in strategy's doc file
4. Commit changes with meaningful descriptions

## Naming Convention

- Pine Script files: `[higher_tf]_[strategy_type]_[entry_tf].pine`
- Backtest results: Use same name as strategy file
- Documentation: Use same name as strategy file 