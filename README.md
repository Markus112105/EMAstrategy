# EMA_Trading_Strategy

This Python program implements a stock trading strategy based on exponential moving averages (EMAs) to predict price movements. It calculates EMAs for a given stock with different time periods and compares them to determine buy or sell signals.

## How It Works

The strategy involves the following steps:

1. Calculate EMAs for the stock using various time periods.
2. Compare shorter-term EMAs to longer-term EMAs.
3. Buy the stock when shorter-term EMAs are higher than longer-term EMAs.
4. Sell the stock when shorter-term EMAs are lower than longer-term EMAs.
5. Track the percentage change in the stock's price between buy and sell points.
6. Calculate statistics such as average gain, average loss, and gain/loss ratio based on these percentage changes.

## Usage

1. Input a stock ticker symbol, start date, and end date.
2. Retrieve the stock's data for the specified time period using the `pandas_datareader` library and save it to a CSV file.
3. Read the data from the CSV file and store it in a Pandas DataFrame.
4. Calculate EMAs for the stock using a range of time periods and store them in the DataFrame.
5. Iterate through each date in the DataFrame and compare EMAs to determine buy or sell signals.
6. Calculate and print various statistics based on the trading results.
