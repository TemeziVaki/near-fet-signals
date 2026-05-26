# NEAR & FET Signal Analyzer

A real-time cryptocurrency signal dashboard for **NEAR/USDT** and **FET/USDT** on Binance.

## Features

- Real-time data from Binance public API — no API key required
- RSI (14) — momentum & oversold/overbought detection
- MACD (12, 26, 9) — trend direction & bullish/bearish crossovers
- Volume analysis — confirms price moves vs 20-period average
- Composite signal score (-100 to +100): Strong Buy to Strong Sell
- 1H / 4H / 1D timeframes, auto-refresh every 5 minutes
- Responsive dark-mode UI

## Tech Stack

- Vanilla HTML/CSS/JavaScript — zero dependencies, zero build step
- Chart.js for charting
- Binance public REST API for market data

## Signal Logic

| Indicator | Weight | Bullish Trigger | Bearish Trigger |
|-----------|--------|-----------------|-----------------|
| RSI (14)  | 35%    | RSI < 30        | RSI > 70        |
| MACD      | 45%    | Bullish crossover | Bearish crossover |
| Volume    | 20%    | High vol + up move | High vol + down move |

## Disclaimer

Educational purposes only. Not financial advice.

## License

MIT
