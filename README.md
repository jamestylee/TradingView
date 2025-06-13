# MEGA Multi-Indicator & PNL Tracker Suite for TradingView

This repository contains two powerful, all-in-one Pine Script indicators for TradingView, authored by `-Tylee-`. These scripts are designed to provide a comprehensive trading dashboard directly on your chart, combining multiple popular technical analysis tools with a unique, manual multi-position PNL tracker.

## Core Features (Common to Both Scripts)

Both indicators are packed with the same set of powerful analysis tools:

*   **📈 On-Chart Visual Indicators:**
    *   **Bollinger Bands (BB):** Customizable standard deviation bands with a choice of MA type (SMA, EMA, WMA, etc.).
    *   **Ichimoku Cloud:** Provides key support/resistance levels and trend direction.
    *   **Triple Moving Averages:** Three configurable EMAs (defaults: 50, 100, 200) for trend analysis, complete with visual alerts for Golden Cross and Death Cross events.
    *   **Auto Fibonacci Retracement:** Automatically draws and updates Fibonacci levels based on the most recent significant price swings (pivots), powered by the ZigZag indicator.

*   **📊 Information Tables:**
    *   **Manual PNL Tracker:** The standout feature. Manually track up to 6 open futures/spot positions across any symbol. The table displays:
        *   A custom label for each position.
        *   Trade direction (Long/Short).
        *   Your entry price.
        *   The live current price of the asset.
        *   Real-time **Unrealized PNL** in USD.
        *   **Percentage distance to your liquidation price**, with color-coding for risk awareness.
        *   A running **Total PNL** for all active positions.
    *   **Indicator Directions Dashboard:** A compact table that shows the current sentiment (Bullish, Bearish, or Neutral) of four key oscillators:
        *   Vortex Indicator
        *   Momentum (MOM)
        *   Directional Movement Index (DMI)
        *   Money Flow Index (MFI)

## The Scripts: A Side-by-Side Comparison

This repository includes two versions of the indicator. `MEGA Multi-Order v4 - FINAL` is the direct successor to `MEGA Multi Indicator 25`, adding a key usability feature.

| Feature / Aspect                   | `MEGA Multi Indicator 25`                               | `MEGA Multi-Order v4 - FINAL`                            |
| ---------------------------------- | ------------------------------------------------------- | -------------------------------------------------------- |
| **Core Indicator Calculations**    | ✅ Identical                                            | ✅ Identical                                             |
| Bollinger Bands                    | ✅ Yes                                                  | ✅ Yes                                                   |
| Ichimoku Cloud                     | ✅ Yes                                                  | ✅ Yes                                                   |
| Triple MAs & Crosses               | ✅ Yes                                                  | ✅ Yes                                                   |
| Auto Fibonacci                     | ✅ Yes                                                  | ✅ Yes                                                   |
| Indicator Directions Table         | ✅ Yes                                                  | ✅ Yes                                                   |
| **PNL Tracker Functionality**      | ✅ Yes                                                  | ✅ Yes                                                   |
| **PNL Tracker Layout**             |  Horizontal (Fixed)                                     | **✅ Horizontal & Vertical (User's Choice)**             |
| **Code Base**                      | Original Version                                        | Refined, with logic for switchable table layouts         |

### Key Difference: PNL Table Layout

The **only significant functional difference** between the two scripts is the flexibility of the PNL Tracker's table display.

1.  **`MEGA Multi Indicator 25 by -Tylee-.txt`**
    *   This script features a PNL table with a **fixed horizontal layout**. Each position is a row, and the data (Label, PNL, etc.) is spread across columns. This is great for wide screens but can take up significant horizontal space.

2.  **`MEGA Multi-Order v4 - FINAL by -Tylee-.txt`**
    *   This is the upgraded version. It introduces a **"Table Layout"** option in the indicator's settings, allowing the user to choose between:
        *   **Horizontal:** The classic layout from the previous version.
        *   **Vertical:** A new, compact layout that stacks the data for each position vertically. This is ideal for traders who want to conserve chart space or use the indicator on smaller screens.

## How to Install and Use

1.  **Open TradingView:** Navigate to any chart on [TradingView](https://www.tradingview.com).
2.  **Open Pine Editor:** Click on the "Pine Editor" tab at the bottom of the screen.
3.  **Copy and Paste:** Open either `.txt` file from this repository, copy the entire script, and paste it into the Pine Editor, replacing any default text.
4.  **Add to Chart:** Click the "Add to chart" button.
5.  **Configure:** Click the gear icon (⚙️) on the indicator's name on your chart to open the settings. Here you can:
    *   Enable/disable and configure every visual indicator.
    *   Input your 6 trades into the PNL Tracker section. Be sure to set the `Active` checkbox, `Symbol`, `Entry Price`, `Size`, and `Liq. Price`.
    *   (For v4) Choose your preferred PNL table layout (Horizontal/Vertical).

## Credits

*   **Original Author:** All credit for the creation, logic, and implementation of these fantastic indicators goes to **-Tylee-**.
*   **Libraries:** This script utilizes the `ZigZag` library by `TradingView/ZigZag/7` for its Auto Fibonacci functionality.
