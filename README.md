# AlgoScalpPro MT5

This code is a sample implementation of the AlgoScalpPro MT5 forex robot developed by the Forex Robot Easy Team. The robot is designed to execute a scalping strategy on the MetaTrader 5 platform. 

## Features
- Follows FIFO (First-In-First-Out) rules to comply with trading regulations.
- Implements a recovery function to increase lot size after executing successful trades.
- Retrieves symbol information for the selected trading instrument.
- Executes trades based on the implemented scalping strategy.

## Libraries Used
- Trade: Provides functions for executing trades.
- PositionInfo: Provides functions for retrieving position information.
- SymbolInfo: Provides functions for retrieving symbol information.

## Functions

### isFIFOCompliant()
- Checks if FIFO rules are being followed by verifying that all open positions have the same symbol.
- Returns true if FIFO rules are being followed, false otherwise.

### increaseLotSize(double lotSize)
- Increases the lot size by multiplying it by 2.
- Returns the increased lot size.

### OnTick()
- Main function for executing the scalping strategy.
- Checks if FIFO rules are being followed.
- Refreshes symbol information.
- Implements the scalping strategy (to be filled by the user).
- Executes trades based on the strategy.
- Implements recovery function to increase lot size once.

### OnInit()
- Initialization function.
- Initializes the position info and symbol info objects.
- Returns INIT_SUCCEEDED to indicate successful initialization.

### OnDeinit(const int reason)
- Deinitialization function.
- Deinitializes the position info and symbol info objects.

### OnStart()
- Entry point of the program.
- Runs the scalping strategy on every tick.
- Sleeps for 100 milliseconds before executing the next tick.

## Product Description

AlgoScalpPro MT5 is an advanced scalping robot developed by the Forex Robot Easy Team. It is designed to execute a scalping strategy on the MetaTrader 5 platform. The robot follows FIFO rules to comply with trading regulations and implements a recovery function to increase lot size after executing successful trades.

The robot utilizes the Trade, PositionInfo, and SymbolInfo libraries to execute trades, retrieve position information, and retrieve symbol information respectively. The scalping strategy is to be implemented by the user, allowing for customization and adaptation to different market conditions.

Please note that ForexRobotEasy is not the official developer of this product. We only provide a sample code that can work as described in the product. For detailed reviews and trading results of AlgoScalpPro MT5, please visit [forexroboteasy.com](https://forexroboteasy.com/forex-robot-review/algoscalppro-mt5-review-advanced-scalper-with-loss-recovery/). To find the official developer of this product, please use MQL5.
