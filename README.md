# G-Research Data Engineering Challenge Worksheet

## What a load of Bollingers

Visualisation is an important part of what we do at G-Research. In this exercise we'll build a useful visualisation tool known as Bollinger band plot.

    Q1. Plot the daily closing price of Bitcoin and Ethereum together on to the same graph?
      a) What does this tell you?
      b) Can you find another crypto-currency that behaves in the same way?
      c) Can you find a crypto-currency that does not follow this pattern?

    Q2. The simple moving average is a technical indicator that investors and traders use to determine the trend of a crypto-currency e.g. whether it is going up in price, or going down. The simple moving average of a series can be calculated by adding up all of the values during a specific period and dividing them by the length of the period. For example, the three day simple moving average of the series [1, 2, 3, 4, 5] is [(1 + 2 + 3) / 3, (2 + 3 + 4) / 3, (3 + 4 + 5) / 3] = [2, 3, 4] which indicates that this series has a positive trend.
      a) Plot the simple moving average of the daily closing price of Bitcoin for each day
        i) Using the previous three day period
        ii) Using the previous seven day period
        iii) Using the previous fourteen day period
      b) Plot a simple moving average on the same graph as the daily closing price of Bitcoin. Choose the one you think is the most informative.
    
    Q3. Crypto-currency is a famously *volatile* asset. This means that the price of a crypto-currency can change by a large amount in a small amount of time. One way of measuring the volatility of a crypto-currency is by looking at the standard-deviation in the closing price over a period of time. The standard deviation reflects the average amount of stock price has differed from the mean over a period of time. It is calculated by determining the mean price for a period of time (the sum of the values in a period of time, divided by the number of values) and then subtracting this figure from each price point. The differences are then squared, summer and averaged to produce the variance. The standard deviation is the square root of the variance.
        a) Plot a bar chart showing the volatility of several crypto-currencies over all of time in the dataset, as measured by the standard deviation. Which crypto-currency is most volatile?

        Like the simple moving average, the standard deviation can also be used as an indicator for how volatility is changing over time.
        b) Plot the standard deviation of the daily closing price of Ethereum starting for each day
          i) Using the previous three day period
          ii) Using the previous seven day period
          iii) Using the previous fourteen day period
          
    [Hard]
    Q4. Using the simple moving average and the standard-deviation, we can plot 'Bollinger Bands', a type of statistical chart used in technical analysis. You can read more about how Bollinger bands are used online at Investopedia.
      a) Plot the simple moving average for a crypto-currency of your choosing. Use a time period of your choice (20 days is common).
      b) Plot a line which is two times the standard deviation of the same time period higher than the simple moving average.
      c) Plot a line which is two times the standard deviation of the same time period lower than the simple moving average.

## For one penny more...
In this exercise, we'll consider a set of questions based around buying and selling a single crypto-currency coin. We'll work our way up to a former interview question used at GR.

    Q1. If you bought a single Bitcoin on the 4th January 2018, how many days after would your investment:
      a) Been worth more than you paid for?
      b) Been worth less than you paid for?

    Q2. Whats the most money you could have made in one day on a single Monero coin?
      a) In absolute terms (e.g. you bought for £3000 one day and sold for £3300 the next day for £300 profit)
      b) In percentage terms (e.g. you bought for £3000 one day and sold for £3300 the next day for a 10% profit)

    Q3. If you bought a single Monero coin on the 15th May 2018 date, what is
      a) The greatest percentage profit you could have made by selling it later? What day would this have been?
      b) The worst percentage loss you could have sold for by selling it later? What day would this have been?

    [Hard - *A version of this was actually one of my interview questions here* ~ Joe]
    Q4. If you could have bought one Litecoin coin on any date, and sold on any later date
      a) What is the most money you could have made? What days would you choose?
      b) What is the most money you could lose? What days would you choose?
      c) Can you solve this problem using just one for loop?
      d) If you had to buy and sell one of EVERY coin on the same date, which days would you chose?

## Time-travel in the market
Predicting the stock market is hard, so a while back we invented a time-machine so that we could travel forward in time to see what the future price of stocks would be. Unfortunately it has a few bugs:

1) It can only go backwards in time and then back to the time it left from.
2) It can only travel to dates between 1st January 2018 and 21st September 2021 (*the dates we have data for, how convenient).

Using the crypto datasets in front of you, perhaps you'll be able to make use of it.

Hint: For these question you will want to consider the *expected* return, how much money could you make on average for each strategy, considering you could arrive at any date in the dataset.

    Q1. If you were sent back in time to a random date in the past with one Bitcoin worth £20,000 in today’s prices. What is the probability it will be worth more when you arrive in the past?

    Q2. You get sent back in time to a random date in the past. You don't know the date, and you only have time to make one decision before you are transported back to the current day. What would you do in these situations, if you are
        a) ...sent back with one Bitcoin worth £20,000 in today’s money, should you sell the coin or do you keep it? For each strategy, how much money would you make on average?
        b) ...sent back with money but no crypto-currency, should you buy one Bitcoin? For each strategy, how much money would you make on average?

    Q3. You will be sent back to the 21st September 2021 (the most recent day in the dataset) and then will be sent back again to an earlier date:
        Should you:
        1) Buy a Bitcoin when you arrive in September and keep it till you are transported back to 2022?
        2) Buy a Bitcoin when you arrive in September and sell it when you are transported to an earlier date?
        3) Not buy a Bitcoin at all.

    [Hard]
    Q4. Its the 1st January 2018 (the start of the dataset) and a future version of G-Research has just sent back a working time machine back.
        a) Whats the most money that could be made in the next three years if you knew what the closing price of Bitcoin would be tomorrow?
        b) Would you have still made money if you used your previous strategy, but the time machine was broken, such that you actually knew the closing price from one week before you thought? For example the 'known' price at the 8th September 2019 is actually the price at the 1st September 2019.
