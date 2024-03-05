# EMA_Trading_Strategy
This code is a stock trading strategy that uses exponential moving averages (EMAs) to try to predict the movement of a stock's price. It does this by calculating EMAs for a given stock with several different time periods, then comparing the EMAs with shorter time periods to the EMAs with longer time periods.
## How it works
The strategy buys the stock when the EMAs with shorter time periods are higher than the EMAs with longer time periods, and sells the stock when the opposite is true. It keeps track of the percentage change in the stock's price between each buy and sell, and calculates various statistics such as the average gain, average loss, and the gain/loss ratio based on these percentage changes.
## Usage
- Input a stock ticker symbol, a start date, and an end date.
- Retrieve the stock's data for the specified time period using the pandas_datareader library and save it to a CSV file.
- Read the data back from the CSV file and store it in a Pandas DataFrame.
- Calculate EMAs for the stock using a range of time periods and store them in the DataFrame.
- Iterate through each date in the DataFrame and compare the EMAs with shorter time periods to the EMAs with longer time periods. If the EMAs with shorter time periods are higher than the EMAs with longer time periods, buy the stock and record the price at which it was bought. If the EMAs with shorter time periods are lower than the EMAs with longer time periods, sell the stock and record the percentage change in the stock's price between the buy and sell.
- Calculate various statistics based on the percentage changes and print them to the console. These statistics include the batting average (the proportion of trades that resulted in a gain), the gain/loss ratio (the ratio of the average gain to the average loss), the average gain, the average loss, the maximum return, the maximum loss, and the total return over all trades.
## Disclaimer
Please note that this code is provided for educational purposes only and is not intended to be used for actual stock trading. Past performance does not guarantee future results, and the accuracy of this code or the results it produces cannot be guaranteed. Trading stocks carries inherent risks, and you should always do your own due diligence and consult with a financial professional before making any investment decisions.
# EMAstrategy
