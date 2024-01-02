**Doteki Heikin Ashi for MT5**

This code is a custom indicator for MetaTrader 5 that calculates and visualizes the Exponential Moving Average (EMA) on a chart. The EMA period is set by the user as an input parameter. The indicator also detects trend direction changes based on the relationship between the current close price and the EMA.

The indicator is initialized in the `OnInit()` function. It checks if the user has set a valid EMA period and sets up the EMA line on the chart using the `SetIndexBuffer()`, `SetIndexStyle()`, and `SetIndexLabel()` functions.

In the `OnDeinit()` function, the indicator removes the EMA line from the chart when it is no longer needed.

The main calculation and trend detection logic is implemented in the `OnCalculate()` function. It receives the necessary price data as input parameters and uses the `iMA()` function to calculate the EMA. The EMA values are stored in the `EMA_Period` array.

The code then checks if the current close price is above or below the EMA to determine the trend direction. If the close price is above the EMA, a bullish trend is detected. If the close price is below the EMA, a bearish trend is detected. The code sends a notification whenever there is a change in trend direction.

The calculated rates are returned at the end of the `OnCalculate()` function.

**Product Description:**

Doteki Heikin Ashi for MT5 is a custom indicator developed by the Forex Robot Easy Team. It calculates the Exponential Moving Average (EMA) and provides trend direction detection on MetaTrader 5 charts.

With Doteki Heikin Ashi, traders can easily identify bullish and bearish trends based on the relationship between the current close price and the EMA. This indicator helps traders make informed trading decisions and optimize their forex trading strategies.

Key Features:
- Calculates and displays the EMA on the chart
- Detects trend direction changes
- Sends notifications on trend direction change
- Customizable EMA period

To use Doteki Heikin Ashi, simply add the indicator to your MetaTrader 5 chart and set the desired EMA period. The indicator will then display the EMA line and notify you whenever there is a change in trend direction.

Please note that Forex Robot Easy is not the official developer of this product. We are providing sample code that can work as described in this product. For detailed reviews and trading results of Doteki Heikin Ashi, please visit the official developer's website or search for the product on MQL5. 

For more information and to download the indicator, visit our website: [Doteki Heikin Ashi for MT5](https://www.forexroboteasy.com)
