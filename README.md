# The-Basis
A trading strategy leveraging the difference between spot and futures prices (basis) for signal generation, trend confirmation and breakout detection. The nasdaq 100 futures and spot price are used for back-testing but can work across other futures symbols.

# Overview:
This script analyzes the relationship between Nasdaq futures (NQ) and the Nasdaq index (NDX) using: 
- BASIS = NQ - NDX

It is used as a baseline for signal generation. The core idea is to use the max and min daily basis as entry routes for buying or selling in the market. When price breaks above the daily high, the trader can look to enter long or enter short when the prices breaks down below the daily low.

When observed over multiple days, price tends to continue in the direction of the breakout and confirms the bias for the day. The equlibrium point is the mid line between the daily high and daily low where traders can place there intial stop loss once price breaks out on either side. Once the trend is confirmed, the trader may trail the stop loss and profit as price expands to the upside or the downside.

# STRUCTURE:
- Price > Basis High → Expansion up
- Price < Basis Low  → Expansion down
- The Basis Mid  → Equilibrium

# TRADING IDEA:
- LONG: Price above Basis High
- SHORT: Price below Basis Low
- STOP: Mid line (dynamic)

The (MAX) Basis High and MIN Basis (Low), act as distance from the daily open according to the basis where if price breaks or below those levels, it is likely to continue in that direction for the reminder of the day. The mid line provides a dynamic stop and chop zone fiter where if price hovers within that area, traders should be expect the price to break out in either way. It cautions to saty away.

With Supervison and experienced trader insight, i believe this script has potential to be very profitable. The difficulty comes in trailing profits and not to give back to the market too much incase price returns to MIN LOW or MAX HIGH but doesn't invalidate the trade and resumes its original direction. Pratice makes perfect in this area and can serve as a building block to automate and be hands free on this strategy.

Traders have multiple options to view:
- Basis vwap
- Basis mean
- Basis Candles
- Price Candles etc...

# Screenshots and Videos
<img width="1181" height="855" alt="image" src="https://github.com/user-attachments/assets/37e3fe15-acf9-4738-a941-4296f6ff3995" />
<img width="1294" height="943" alt="image" src="https://github.com/user-attachments/assets/55f4f3fb-bba6-4215-b66d-f665a7b5e727" />
<img width="1292" height="936" alt="image" src="https://github.com/user-attachments/assets/552c4c2d-efd1-4ca5-8709-23cc361a4fdc" />
<img width="1289" height="941" alt="image" src="https://github.com/user-attachments/assets/ed286fa0-2fcf-4aa7-82f0-f67efae3a675" />
<img width="1297" height="943" alt="image" src="https://github.com/user-attachments/assets/2dcc915a-1fc6-4456-9d04-ae63cc2436e6" />
<img width="11

https://github.com/user-attachments/assets/3777ba4c-8b5a-437d-b970-46bf7ff20ae7

79" height="889" alt="image" src="https://github.com/user-attachments/assets/faf69c15-ca81-4272-8e27-18cce26a02c1" />



