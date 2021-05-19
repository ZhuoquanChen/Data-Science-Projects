### Overview

If a company want to become competitive and grow their sales, they need to leverage machine learning predictive models so they can be able to forecast sales in the future. Predictive models attempt at forecasting future sales based on historical data while taking into account seasonality affects, demend, hilidays, promotions and competition.

In this project, I leveraged time series models to predict future product sales such as Facebook prophet time series forecasting model for prediction of weekly, monthly and yearly trends.

The purpose of this project is to leveraged Facebook prophet time series forecasting model to predict products sales in the future.
  - Predicted sales trend by weekly, monthly and yearly for each store.


### Problem Statement

Let's say I work as a data scientist in Sales Department, and the sales team provided me with data from 1100 stores. The objective is to predict future daily sales based on some features such as stores promotion, location, holidays, competition, product types and so on.


### Data:

  Data Source: 
  [https://www.kaggle.com/c/rossmann-store-sales/data](https://www.kaggle.com/c/rossmann-store-sales/data)
  
  
### EDA:

- Data Cleaning 
  - Handling nulls
  - Getting rid of unwanted fetures
- Visualizations
  - sales.csv
    - Average 600 customers per day, maximum is 4500 (note that describe shows that 7388 so it should be a outlier!)
    - Data is equally distibuted across various Days of the week (about 150000 observations x 7 day = about 1.1 million observation) 
    - Stores are open about 80% of the time
    - Data is equally distributed among all stores (no bias)
    - Promo #1 was running about 40% of the time 
    - Average sales around 5000-6000 Euros
    - School holidays are around about 18% of the time
  - store.csv
    - Half of stores are involved in promo 2
    - Half of the stores have their competition at a distance of 0-3000m (3 kms away)
- Outliers detection
- Meerged sales.csv and sales.csv
  - correlation between target and each feature 
  - Discomposing 'Date' column into year, month and day by DatetimeIndex function
  - The average 'Sales' and 'Customers' per month
  . <img src="https://github.com/ZhuoquanChen/Data-Science-Projects/blob/main/Future_Sales_Prediction/avg_sales_permonth.png" width="600" height="400">
  - The average 'Sales' and 'Customers' per day in a month
  . <img src="https://github.com/ZhuoquanChen/Data-Science-Projects/blob/main/Future_Sales_Prediction/avg_customers_permonth.png" width="600" height="400">
  - Average 'Sales' of different type of stores
  - <img src="https://github.com/ZhuoquanChen/Data-Science-Projects/blob/main/Future_Sales_Prediction/diff_stores.png" width="600" height="400">
  - How does the promo effect Sales and Customers
  . <img src="https://github.com/ZhuoquanChen/Data-Science-Projects/blob/main/Future_Sales_Prediction/promo2.png" width="1000" height="350">
   
### Modeling:
  - Facebook Prophet Model
  - Renamed two columns in data frame which are 'Date' column as 'ds'(x axis) and 'Sales' column as 'y'(y axis)
  - The first training without holidays
    ![](https://github.com/ZhuoquanChen/Data-Science-Projects/blob/main/Future_Sales_Prediction/without_holidays.png) 
  - The second training with holidays
    ![](https://github.com/ZhuoquanChen/Data-Science-Projects/blob/main/Future_Sales_Prediction/with_holidays.png) 
    
    - StateHoliday: indicates a state holiday. Normally all stores, with few exceptions, are closed on state holidays. Note that all schools are closed on public holidays and weekends. a = public holiday, b = Easter holiday, c = Christmas, 0 = None
    - SchoolHoliday: indicates if the (Store, Date) was affected by the closure of public schools
