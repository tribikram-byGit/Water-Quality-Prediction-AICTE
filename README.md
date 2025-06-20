# Water-Quality-Prediction-AICTE
I have tried to execute a model for Water Quality Prediction on Google Colab based on a dataset provided by the mentor.
Here, we have imported pandas, numpy, matplot, seaborn, scikit-learn. We are going to import MultiOutputRegressor, RandomForestRegressor, train_test_split, mean_squared_error, re_score
The data was loaded, we have summarised the data by df.info() then we got to know the statistics of the data(count,min,max,mean,std)
To find the missing values we used df.isnull() and summed up to find the count of missing values
Since the date column is in object format we are going to fix it into datetime format
After sorting the data by id and date, we've extracted the year and month and defined the list of Pollutants
