 
# TradeWatcher
 
Display Big trades from Crypto Exchanges BitMex and Bitfinex using websocket
          
Version : 0.03


## Installation

Simply copy tradewatcher.html and open it with a webbrowser

## Usage

All numbers are displayed in USD:

Current pairs are : 
  - Bitmex XBT/USD
  - Bitfinex BTC/USD
  - Bitfinex ETH/USD
  - Bitfinex XRP/USD

Displayed informations : 
- Totals since app started ( including all trades)
- 10 biggest trade
- Historical list of trades > 10000

## Configuration

Exchanges, pairs and amount limit can be manualy setup using the **listeners** variable at the end of the javascript code

## Todo
  
- Clean code, split logical/view
- User interface
- Implement some Charts
- Better HTML integration, auto adding columns
- Better handling of WS response, errors, limits, ban

## Ideas

### Volume indicator

- make some time bucket : 1min
- display total buy / total sell
- display with quantity bucket : 10 50 100 200