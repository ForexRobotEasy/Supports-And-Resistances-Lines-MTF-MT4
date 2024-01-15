# Supports And Resistances Lines MTF MT4

This code is a custom indicator designed to draw support and resistance lines on a MetaTrader 4 (MT4) chart. It supports multiple timeframes and allows the user to customize the line colors, line style, and line thickness.

## Input Parameters

- `timeframe1`, `timeframe2`, `timeframe3`: The timeframes for which the support and resistance lines will be calculated and drawn. The default values are M1, M5, and M15.
- `supportLineColor`: The color of the support lines. The default value is green.
- `resistanceLineColor`: The color of the resistance lines. The default value is red.
- `lineStyle`: The style of the lines. The default value is solid.
- `lineThickness`: The thickness of the lines. The default value is 1.

## How It Works

The indicator uses three different timeframes to calculate and draw support and resistance lines. It first clears any previously drawn lines on the chart. Then, for each timeframe, it calculates the support and resistance levels using the `CalculateSupportLevel()` and `CalculateResistanceLevel()` functions. Finally, it draws the lines using the `DrawLine()` function.

The `CalculateSupportLevel()` and `CalculateResistanceLevel()` functions are placeholders that need to be implemented by the user. These functions should perform the necessary calculations based on the specified timeframe and return the support and resistance levels.

The `DrawLine()` function is responsible for drawing a support or resistance line on the chart. It creates a trend line object with a unique name, sets the line style, width, and color, and positions the line at the specified level.

The `OnInit()` function is the initialization function for the indicator and returns `INIT_SUCCEEDED` to indicate successful initialization.

The `OnCalculate()` function is the iteration function for the indicator. It is called on each new tick or bar and is responsible for calculating and drawing the support and resistance lines. It calls the `DrawSupportAndResistanceLines()` function and returns the number of calculated bars.

## Product Description

The Supports And Resistances Lines MTF MT4 indicator is a powerful tool for identifying key support and resistance levels on multiple timeframes. It can help traders make informed decisions and improve their trading strategies.

Key Features:
- Supports multiple timeframes (M1, M5, and M15 by default).
- Customizable line colors, line style, and line thickness.
- Easy to use and integrate into existing trading systems.
- Provides clear visual representation of support and resistance levels.

Please note that ForexRobotEasy is not the official developer of this product. We only provide a sample code that can work as described in this product. For detailed reviews and trading results of this product, please visit the official developer's website at [Forex Robot Easy - MTF MT4 Review](https://forexroboteasy.com/forex-robot-review/mtf-mt4-review-unveiling-forex-softwares-real-results/). To find the official developer of this product, please refer to MQL5.
