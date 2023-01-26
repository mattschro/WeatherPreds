# WeatherPreds

- 'weather_and_market_scraper.ipynb'
  - Gets live high temperature forecasts for two major U.S. cities from an API
  - Plots the current day and next day's projected temperature
  - Accesses live market data from the prediction market's API on what probabilities other traders are assigning to high temperature buckets (47 F or below, 48 to 49 F, 50 to 51 F, 52 F or above, etc.)
  - Visualizing the yes ask and no ask prices (what you would have to pay to buy yes and no shares) as well as the cumulative price of these shares
- 'daily_historical_chi_weather.csv'
  - Historical daily measurements of Chicago weather since 1/1/1980
- 'DailyWeatherPrediction.ipynb'
  - Reads in the historical Chicago weather
  - Explaining the variables / data cleaning
  - Builds linear regression, k nearest neighbors, and random forest models w/ RMSE of just over 5
- 'hourly_historical_chi_weather.csv'
  - Hourly, but definitely not always on the hour, measurements of Chicago weather since 1/1/2000
- 'HourlyWeatherPrediction.ipynb'
  - Reads in hourly weather data
  - Custom function throws out variables that have null values over a certain threshold
  - Cleaned temperature variable
  - Simple LTSM or SARIMA w/ only time and temp to be built, but currently, main blockers:
    - Missing temperature observations (~15%)
    - Non-constant interval between observations
    - Reality that professional forecasters are *almost certainly* better at this task than someone (me) without domain expertise!
   
