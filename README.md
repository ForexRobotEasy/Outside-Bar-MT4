# Outside Bar MT4 - ReadMe

This code is an implementation of the Outside Bar trading strategy for MetaTrader 4 (MT4). It identifies outside bars and places buy or sell stop orders based on the pattern formed.

## Functionality

The code consists of the following functions:

1. `IsOutsideBar(int bar)`: This function checks if the current bar is an outside bar by comparing the high and low of the current bar with the high and low of the previous bar.

2. `IsBullishOutsideBar(int bar)`: This function checks if the current bar is a bullish outside bar by comparing the high, low, close, and open of the current bar.

3. `IsBearishOutsideBar(int bar)`: This function checks if the current bar is a bearish outside bar by comparing the high, low, close, and open of the current bar.

4. `PlaceBuyStopOrder(double price)`: This function places a buy stop order at the specified price. It calculates the stop loss (sl) and take profit (tp) levels based on the current spread.

5. `PlaceSellStopOrder(double price)`: This function places a sell stop order at the specified price. It calculates the stop loss (sl) and take profit (tp) levels based on the current spread.

The code also includes the following main functions:

1. `OnInit()`: This function is called during the initialization of the expert advisor. It returns `INIT_SUCCEEDED` to indicate a successful initialization.

2. `OnDeinit(const int reason)`: This function is called during the deinitialization of the expert advisor. It can be used to perform any necessary cleanup.

3. `OnTick()`: This function is called on every tick and is the main entry point for the expert advisor's trading logic. It identifies the current bar, checks if it is an outside bar, and places the appropriate stop order based on the type of outside bar.

## Usage

To use this code, simply copy and paste it into your MetaEditor in MetaTrader 4. Compile the code, and it will be ready to use as an expert advisor.

Please note that ForexRobotEasy is not the official developer of this product. We are only providing a sample code that can work as described in the product. For detailed reviews and trading results of this product, please visit [https://forexroboteasy.com/forex-robot-review/outside-bar-mt4-review-revolutionize-your-forex-trading-strategy/](https://forexroboteasy.com/forex-robot-review/outside-bar-mt4-review-revolutionize-your-forex-trading-strategy/).

For the official developer of this product, please refer to the MQL5 platform.

## Disclaimer

ForexRobotEasy is not the official developer of this product. We are simply showcasing a sample code that implements the described functionality. Trading in the forex market carries a high level of risk and may not be suitable for all investors. Before using any expert advisor or trading strategy, please ensure that you understand the risks involved and seek professional advice if needed.
