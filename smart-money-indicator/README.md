# Smart Money Concepts Indicator (Refined)

This indicator is designed for TradingView's Pine Editor (v5). It implements high-precision Smart Money Concepts (SMC) logic with strict validation rules.

## Key Refinements

- **Obvious Liquidity Sweeps**: Detects significant grabs where price wicks beyond a previous pivot by a minimum distance (adjustable via ATR multiplier) but closes back within the range.
- **Body-Close CHoCH**: Change of Character (CHoCH) is only confirmed on a candle body close above/below a pivot high/low. Candle wicks do not trigger a CHoCH.
- **CHoCH before BOS**: A valid Break of Structure (BOS) is only identified *after* a CHoCH has already established a new trend direction.
- **Strict Fair Value Gaps (FVG)**: FVGs are identified only when there are 3 consecutive candles of the same color (e.g., 3 bullish candles for a bullish FVG) with a gap between the first and third.
- **POI-Based Entry Signals**: Optimal entry signals occur when price retraces into a Point of Interest (Order Block) following a confirmed Break of Structure (BOS).

## How to Use

1. Open a chart on [TradingView](https://www.tradingview.com/) (recommended timeframe: 15m).
2. Click on the **Pine Editor** tab at the bottom of the screen.
3. Click on **Open** -> **New indicator**.
4. Delete all the default code in the editor.
5. Copy the code from `indicator.pine` in this directory and paste it into the Pine Editor.
6. Click **Save** and name it "SMC Refined".
7. Click **Add to Chart**.

## Customization

- **Pivot Lookback Length**: Higher values identify more "obvious" structure.
- **Sweep Distance Multiplier (ATR)**: Controls how far a wick must extend to be considered a significant liquidity grab.
- **Show/Hide**: Toggle Fair Value Gaps, Order Blocks, and Liquidity Sweeps.
