 
# TradeWatcher
 
Display Big trades from Crypto Exchanges BitMex and Bitfinex using websocket

## Installation

Simply copy tradewatcher.html and open it with a browser

Or use [Preview](https://htmlpreview.github.io/?https://github.com/the023/tradewatcher/blob/master/tradewatcher.html)


## Usage

All numbers are displayed in USD:

Current pairs are : 
  - Bitmex XBT/USD
  - Bitfinex BTC/USD
  - Bitfinex ETH/USD
  - Bitfinex XRP/USD

Displayed informations : 
- Delta : difference between buy and sell volume
- Total 
- Price Change since : 1 2 5 10 30 60 120 minutes
- Chart of buy/sell percentage per minute
- 15 biggest trades, time sorted
- Historical list of trades > 10000

## Configuration

Exchanges, pairs and amount limit can be manualy setup using the **listeners** variable at the end of the javascript code


## Changelog : 
- 0.04  Big trades are sorted by date, add stuff to todo
- 0.03  Display volume chart


## Todo
  
General:
- Clean code, split logical/view
- Get a host and make a website  

Data : 
- Add Exchanges with websocket : binance gdax bittrex
- Find a way to validate data consistency
    - Compare with trade list extract from exchange
    - Compare with BitmexRekt, bitmex whale
    - Check Bitmex Doc to extract more data
    - Validate order size on Bitmex
- Fix Bitfinex disconnection : understand why, auto reload when off . create a reload button

UI:
- Choose a Front lib, react/vue/? and build User interface
- UI: choose exchange, pairs, limit, display option
- UI: remember user configuration
- UI: Button to turn off websocket
- Implement some Charts
- Better HTML integration, auto adding columns
- Better handling of WS response, errors, limits, ban

Charts:
- Choose way to chart:
    - pur canvas
    - d3.js
    - React-stockchart 
    - other lib
- What to chart :
    - price / volume overtime   
    - %buy/sell
    - time/levels with big trades
    
## Ideas


### Volume indicator

- make some time bucket : 1min
- display percentage buy vs sell and total volume over time
- for each period (1m,5m,...) display buy/sell volume with sum splitted by order size(buckets) 0.01 0.1 1 5 ... 10 000 000

- display price zone with more volume, VPVR style ?