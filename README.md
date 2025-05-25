# Global Liquidity Dashboard (Enhanced v2)

A multi-asset liquidity proxy indicator for TradingView that helps detect Bitcoin trend breakouts and breakdowns using:

- Inverted DXY
- Yield Curve Spread (US10Y - US02Y)
- S&P 500 Index
- Gold
- BTC Price & Volume

### 🧠 Features

- Liquidity proxy normalized over 200 bars
- Smoothed EMA liquidity trend
- BTC momentum filter (vs. liquidity)
- Volume filter using SMA
- Cross-over alerts for BTC breakouts/breakdowns

### 📈 Chart Example
> Add a screenshot here: `screenshots/example_chart.png`

### 🔔 Alerts
- **BTC Breakout**: Cross above liquidity proxy with momentum and volume
- **BTC Breakdown**: Cross below liquidity proxy with momentum and volume

### 💡 How It Works
- `inv_dxy`, `rate_spread`, `gold`, `SPX` are normalized and weighted into a liquidity score
- BTC and NASDAQ are also normalized for comparison
- Momentum is calculated as EMA of the difference between BTC and liquidity
- Volume filter ensures breakout is confirmed by activity

### 📜 License

MikeBasse.
