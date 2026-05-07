# Smart Money Concepts Indicator

This indicator is designed for TradingView's Pine Editor (v5). It helps identify key market structure and liquidity elements used in Smart Money Concepts (SMC) trading.

## Features

- **Liquidity Sweeps/Grabs**: Identified when the price moves beyond a previous pivot high or low but closes back within the range.
- **Change of Character (CHoCH)**: Signals a potential trend reversal when a significant high/low is broken.
- **Break of Structure (BOS)**: Signals trend continuation when a previous high/low in the direction of the trend is broken.
- **Fair Value Gaps (FVG)**: Highlights imbalances in price action.
- **Order Blocks (OB)**: Marks the last candle before a significant move that caused a BOS or CHoCH.
- **Optimal Entry Signals**: Generated when there's a confluence of a liquidity grab followed by a CHoCH or BOS.

## How to Use

1. Open a chart on [TradingView](https://www.tradingview.com/).
2. Click on the **Pine Editor** tab at the bottom of the screen.
3. Click on **Open** -> **New indicator**.
4. Delete all the default code in the editor.
5. Copy the code from `indicator.pine` in this directory and paste it into the Pine Editor.
6. Click **Save** and give it a name (e.g., "SMC Indicator").
7. Click **Add to Chart**.

## Customization

You can adjust the following settings in the indicator's settings menu:
- **Pivot Lookback Length**: Controls the sensitivity of high/low detection.
- **Show/Hide**: Toggle Fair Value Gaps, Order Blocks, and Liquidity Sweeps.
- **Colors**: Customize the colors for various elements to match your chart theme.
