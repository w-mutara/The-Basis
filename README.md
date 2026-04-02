# The-Basis
A trading strategy leveraging the difference between spot and futures prices (basis) for signal generation, trend confirmation and breakout detection.

# Overview:
This script analyzes the relationship between Nasdaq futures (NQ) and the Nasdaq index (NDX) using: 
- BASIS = NQ - NDX

The is used as a baseline for signal generation. The core idea is to use the max and min daily basis as entry routes for buying or selling in the market. When price breaks above the daily high, the trader can look to enter long or enter short when the prices breaks down below the daily low.

When observed over multiple days, price tends continue in the direction of the breakout and confirms the bias for the day. The equlibrium point is the mid line between the daily high n  daily low where traders can place there intial stop loss once price breaks out on either side. One the trend is confirmed, the trader may trail the stop loss and profit as price expands to the upsude or the downside.

------------------------------------------------------------------------------
STRUCTURE:
- Price > Basis High → Expansion up
- Price < Basis Low  → Expansion down
- The Basis Mid  → Equilibrium

------------------------------------------------------------------------------
TRADING IDEA:
- LONG: Price above Basis High
- SHORT: Price below Basis Low
- STOP: Mid line (dynamic)

The (MAX) Basis High and MIN Basis (Low), act as distance from the daily open
according to the basis where if price breaks or below those levels, it is likely to continue in that direction
for the reminder of the day. The mid line provides a dynamic stop and chop zone fiter where if price hovers within 
that area, traders should be expect the price to break out in either way. It cautions to saty away.

NOTE:
With Supervison and experienced trader insight, i believe this script has potential to be very profitable.
The difficulty commes in trailing profits and not to give back to the market too much incase price returns to MIN LOW 
or MAX HIGH but doesn't invalidate the trade and resumes its original direction. Pratice makes perfect in this area and can serve
as a building block to automate and be hands free on this strategy.

Traders have multiple options to view:
- Basis vwap
- Basis mean
- Basis Candles
- Price Candles etc...
