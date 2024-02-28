# ICT London MT5

ICT London MT5 is an AI-powered Forex strategy developed by the Forex Robot Easy Team. This code serves as a sample implementation of the strategy and is not the official code developed by the product's creators. For detailed reviews and trading results of this product, please visit the official website at [https://forexroboteasy.com/forex-robot-review/ict-london-mt5-review-ai-powered-forex-strategy-for-us30/](https://forexroboteasy.com/forex-robot-review/ict-london-mt5-review-ai-powered-forex-strategy-for-us30/).

## Custom Indicator Inputs

- `period` (int): Period for calculating the moving average.
- `applied_price` (ENUM_APPLIED_PRICE): Price used for calculation.

## Global Variables

- `asian_session_start` (datetime): Start time of the Asian session.
- `asian_session_end` (datetime): End time of the Asian session.

## Expert Advisor Inputs

- `lot_size` (double): Lot size for trading.
- `stop_loss` (double): Stop loss in points.
- `take_profit` (double): Take profit in points.

## Expert Advisor Initialization

The `OnInit()` function initializes the Asian session start and end times based on the current local time.

## Expert Advisor Start

The `OnTick()` function is called on each tick and determines whether to perform Asian session analysis or London session trading based on the current session.

## Function: IsAsianSession

The `IsAsianSession()` function checks if the current time is within the Asian session by comparing it to the Asian session start and end times.

## Function: IsLondonSession

The `IsLondonSession()` function checks if the current time is within the London session by comparing it to the Asian session end time and adding the period of one hour.

## Function: AnalyzeAsianSession

The `AnalyzeAsianSession()` function performs analysis of the Asian session by analyzing historical data and market sentiment to determine the prevalent market direction. It also utilizes AI technology and mathematical calculations to derive insights into potential market reversals.

## Function: TradeLondonSession

The `TradeLondonSession()` function identifies and trades opportunities during the London session based on the analysis conducted during the Asian session. It implements trading logic to capitalize on potential market reversals and opens trades with the specified lot size, stop loss, and take profit.

## Expert Advisor Deinitialization

The `OnDeinit()` function is called when the expert advisor is being deinitialized and can be used for any necessary cleanup or deinitialization.

Please note that ForexRobotEasy is not the official developer of this product. We only provide a sample code that can work as described in the official product. To find the official developer of this product, please visit the MQL5 website.
