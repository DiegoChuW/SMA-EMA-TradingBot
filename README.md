# SMA-EMA-TradingBot
- This is a basic trading bot that was created using Ninja Script 8
- Ninja Script 8 is a program which facilitates the creation of trading bots using built in data
- The trading bot relies on EMAs and SMAs to place in a trade
- This bot is not flawless and is meant to be used as a simple template to get you started
- The Trading Bot relies on 1min candles and was backtested using btc/usd

![sum](https://user-images.githubusercontent.com/109917826/199863044-ab0d727d-492e-478c-84db-3bcd7ca58b76.JPG)

# What's an SMA or an EMA?
- A simple moving average (SMA) is an arithmetic moving average calculated by adding recent prices and then dividing that figure by the number of time periods in the calculation average. For example, one could add the closing price of a security for a number of time periods and then divide this total by that same number of periods. Short-term averages respond quickly to changes in the price of the underlying security, while long-term averages are slower to react. There are other types of moving averages, including the exponential moving average (EMA) and the weighted moving average (WMA).
- An exponential moving average (EMA) is a type of moving average (MA) that places a greater weight and significance on the most recent data points. The exponential moving average is also referred to as the exponentially weighted moving average. An exponentially weighted moving average reacts more significantly to recent price changes than a simple moving average simple moving average (SMA), which applies an equal weight to all observations in the period.
![chart](https://user-images.githubusercontent.com/109917826/199861194-5da742b5-46c7-4d8d-97ba-51bf1693bb0a.JPG)

# In what conditions does it buy?
- The Strategy takes 
![analysis2](https://user-images.githubusercontent.com/109917826/199861353-1768fd8c-a612-4e6a-86ce-8b3d672df585.JPG)

# In what conditions does it sell?
![analysis](https://user-images.githubusercontent.com/109917826/199861378-caab366d-5baa-4d7e-8c24-240076bb861a.JPG)

# DISCLAIMER!
**This strategy has only been backtested using past data and there's no guarantee that this strategy will succeed. Trading involves a significant risk of loss and is not suitable for everyone. This strategy just takes advantage of the relation between SMA and EMA on momentum.**
