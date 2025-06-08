# 4H Trend 1H Confirmation Strategy

## Strategy Overview
- **Market**: Forex (EURUSD)
- **Primary Timeframe**: 4H (Trend)
- **Entry Timeframe**: 1H (Confirmation)
- **Version**: 1.0
- **Trading Hours**: 14:00-23:00 GMT+7 (Avoiding Asian session)

## Strategy Logic
The strategy combines higher timeframe trend analysis with lower timeframe confirmation:
1. Uses 4H chart for trend direction using EMA crossover system
2. Uses 1H chart for entry confirmation using RSI
3. Implements strict risk management with minimum stop loss
4. Avoids trading during Asian session for better reliability

## Entry Rules
### Long Entry
- 4H Fast EMA (50) above Slow EMA (200)
- 1H RSI below 30 (oversold)
- Current time is between 14:00-23:00 GMT+7

### Short Entry
- 4H Fast EMA (50) below Slow EMA (200)
- 1H RSI above 70 (overbought)
- Current time is between 14:00-23:00 GMT+7

## Exit Rules
- Stop Loss: Maximum of (30 pips, 1H ATR)
- Take Profit: 3x Stop Loss distance
- Position closes automatically when SL or TP is hit

## Risk Management
- Position Size: 100% of available equity per trade
- Stop Loss: Minimum 30 pips for EURUSD
- Take Profit: 1:3 risk-reward ratio
- No trading during Asian session (04:00-14:00 GMT+7)

## Technical Indicators
- 4H EMA (50) - Fast trend line
- 4H EMA (200) - Slow trend line
- 1H RSI (14) - Entry confirmation
- 1H ATR (14) - Dynamic stop loss calculation

## Backtest Results
### Latest Backtest (YYYY-MM-DD)
- Test Period: [Start Date] to [End Date]
- Net Profit:
- Win Rate:
- Profit Factor:
- Max Drawdown:
- Sharpe Ratio:

[Link to backtest screenshots and metrics in backtest_results/forex/4h_trend_1h_confirm/]

## Change Log
- 2024-03-19: Initial version
  - Implemented basic strategy with 4H trend and 1H confirmation
  - Added session filtering
  - Set minimum stop loss for EURUSD
  - Implemented 1:3 risk-reward ratio
- 2024-03-19: Updated timezone
  - Converted trading hours to GMT+7
  - Adjusted Asian session avoidance times 