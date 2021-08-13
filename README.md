# StockPredictions

**Authors**: Wil Dotson and Robert Oliver

## Project Goals:

We utilized a Yahoo Finance API to gather stock information. We wanted to create a reliable model to predict future stock prices. We also wanted to create a model so that we could potentially invest money into the stock market in order to see if our model could be profitable for ourselves. The final reason we chose this project was to gain knowledge on algotithmic training because it combines our in school major, while also utilizing our data science skills. 

## Data

We used 5 years worth of data from the day that you ran the function. So if it was October 10, 2021, then you would have data dating back to October 10, 2016. Our target was the closing price of the stock. We chose this as our target because a stock can still crash during the day, so high would not be as reliable to predict. The stocks we examined were the S&P 500 index, Dow Jones Industrial Average, Google, Facebook, and Regions. 

## Methods

We reformatted the dataframe so that the index was in the format of YYYY-MM-DD, and the only other column was close price. We experimented with Random Walk, Arima, Auto-Arima, Tensorflow Long Short Term Memory, and Facebook Prophet. We settled on Facebook prophet because it had the lowest RMSE (Root mean squared error), which is the average of how far off our predictions are, and our predictions were trending farely well compared to the actual prices. We optimized our model's parameters for each stock by utilizing a GridSearch. Our predictions were based on our test data, and future values. 

## Visuals 



## Conclusion

In conclusion, our model predicts well on stocks who exhibit clear trends over time, but poorly on stocks that have dramatic changes in established trends. In the end, the market is extremely hard to predict over a long term and that is why not everyone makes their living off of the stock market. 

## Future Work

In our future work we would like to implement real world events to help us better predict the trends and prices of stocks. Next, we would like to be able to pull predictions for every S&P 500 company. After this, we would like to further our search into neural networks like than Long Short Term Memory, to see if this could improve our model. Finally, we would like to do some time manipulation like downscaling the data into weeks instead of days, and having more than 5 years in our dataframe. We would also like to upscale our data to hourly, but with our current technology we would have to make the dataframe to range back to about 2 years. 