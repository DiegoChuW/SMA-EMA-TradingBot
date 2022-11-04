# SMA-EMA-TradingBot
- This is a basic trading bot that was created using Ninja Script 8
- This bot is fully Autonomous and can generate income on the side
- The trading bot relies on the momentum of EMAs and SMAs to place in a trade
- The Trading Bot relies on 1min candles and was backtested using btc/usd

![sum](https://user-images.githubusercontent.com/109917826/199863044-ab0d727d-492e-478c-84db-3bcd7ca58b76.JPG)

# What's an SMA or an EMA?
- A simple moving average (SMA) is an arithmetic moving average calculated by adding recent prices and then dividing that figure by the number of time periods in the calculation average. For example, one could add the closing price of a security for a number of time periods and then divide this total by that same number of periods. Short-term averages respond quickly to changes in the price of the underlying security, while long-term averages are slower to react. There are other types of moving averages, including the exponential moving average (EMA) and the weighted moving average (WMA).
- An exponential moving average (EMA) is a type of moving average (MA) that places a greater weight and significance on the most recent data points. The exponential moving average is also referred to as the exponentially weighted moving average. An exponentially weighted moving average reacts more significantly to recent price changes than a simple moving average simple moving average (SMA), which applies an equal weight to all observations in the period.

![chart](https://user-images.githubusercontent.com/109917826/199861194-5da742b5-46c7-4d8d-97ba-51bf1693bb0a.JPG)

# In what conditions does it buy?
- The Strategy first looks at the EMA 12 and the EMA 26
- If the EMA 12 is greater than the EMA 26 then it would look at the SMAs
- The SMAs would be the SMA 12 and the SMA 26
- If it sees that the SMA 12 is also greater than the SMA 26 then it would order a buy with a quantity of 1
- The order is only placed once the conditions have been met after 1 candle close

![analysis2](https://user-images.githubusercontent.com/109917826/199861353-1768fd8c-a612-4e6a-86ce-8b3d672df585.JPG)

# In what conditions does it short?
- The Strategy first looks at the EMA 10 and the EMA 20
- If the EMA 10 is less than the EMA 20 then it would look at the SMAs
- The SMAs would be the SMA 10 and the SMA 20
- If it sees that the SMA 10 is also less than the SMA 20 then it place a short order with a quantity of 1
- The order is only placed once the conditions have been met after 1 candle close

![analysis](https://user-images.githubusercontent.com/109917826/199861378-caab366d-5baa-4d7e-8c24-240076bb861a.JPG)

# In what conditions does it take profit or stop loss?
- The strategy uses percentages to tp and sl
- sl and tp don't work that well with this strategy but are important for all trading strategies
- The sl is executed once the trade is on a 2% loss
- The tp is executed once the trade is on a 6% win
- All trades will also close after trading hours to prevent low volatility

# DISCLAIMER!
**This strategy has only been backtested using past data and there's no guarantee that this strategy will succeed. Trading involves a significant risk of loss and is not suitable for everyone. This bot is not flawless and is meant to be used as a simple template to get you started. This strategy just takes advantage of the relation between SMA and EMA on momentum.**
