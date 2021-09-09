# Cotton-price-prediction
Cotton is a commodity, which is perhaps the most volatile among all the agricultural commodities traded. Due to high volatility in cotton prices, it is very difficult to predict the future market trend . Thus an artificial Intelligence based solution is developed which may calculate the probability of future market trend on the basis of past years data . Various time series models are fit under trial and error method substantiating the efficacy of LSTM model subsequently.

#Methodology

The dataset is collected from a reliable website which is said to consist of two attributes with a discrete set of
values - DATE and VALUES (price of cotton measured in USD per pound) . 
It takes into
account around 5 decades of cotton’s prices for analysis . 
Initially the dataset is preprocessed by checking for null values . 
Then date is set as the index of the dataframe for better visualisation . 
After that a simple graph with date in the x-axis and price in the y-axis is plotted to categorize it as stationary or non-stationary .
As far as stationarity is concerned two values are not dependent based on time.
Instead it relies on the rule of realizations. 
That is correlation between two variables are not dependent on their values but on the lag between them.
Then a duplicate data frame is created with date and target variable so that any changes acquired in the process aren't reflected on the original data. 
Later the data set is split into training and validation sets with 80% of data.
Now after a basic exploration of the dataset it is evaluated using various models like moving average , KNN , autoarima , prophet and LSTM . 
So after comparing the model with lower RMSE(root mean square error) value and a higher accuracy rate is considered as the best fit . 

#Result

At last the LSTM model was found to be the precise one . 
