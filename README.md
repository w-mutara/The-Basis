# The-Basis
A trading strategy leveraging the difference between spot and futures prices (basis) for signal generation, trend confirmation and breakout detection.

# OVERVIEW:

This script analyzes the relationship between Nasdaq futures (NQ) and the Nasdaq index (NDX) using: BASIS = NQ - NDX

Price is transformed into "basis scale" to observe: Expansion (momentum), Equilibrium (mean reversion)

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
