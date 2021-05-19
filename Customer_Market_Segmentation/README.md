### Overview

Marketing is extremely critical and crucial for any business. One of the key pain points for marketers is to know thier customers and identify thier needs in order to grow the revenue. By understanding the customers, marketers can launch a target ad marketing campaign that is tailored for their specific needs or basically cater to them. If data about the customers is available, data scientist can applied to perform market segmentation. 

In this project, I leveraged the data science skills and machine learning skills to perform market segmentation and transform the marketing department including exploratory data analysis, visualize customers dataset, as well as to fill out missing data or null elements. Found the optimal number of clusters using the Elbow Method. Then applied K-Means cluster algorithms to perform the segmentation of the dataset. Applied principle component analysis to perform dimensuinality reduction for the dataset. Applied auto-encoder to perform dimensionality reduction to build and train an auto-encoder models in Keras.

The purpose of this project is to help Marketing Department of banks to segment the consumption market by clustering customers based on their credit cards consumption data, then launch ads to target it percisely in order to grow or extend business.
  - The customer dataset was divided to 6 clusters by K-Mean algorithms.
  - The dimensionality of the dataset was reduced to 2 dimension for visualzation.

### Problem Statement

In this case, I have been hired as a data scientist to a bank in New York City, which has extensive data about their customers for the past months. The Marketing team want to launch a targeted ad marketin campaign by dividing the customers into at least three different groups based on credit card consumption.


### Data:

  - Data Source: [Credit Card Dataset for Clustering](https://www.kaggle.com/arjunbhasin2013/ccdata)
  
  
### Methodology:

  - Data Cleaning 
    - Handling nulls
    - Getting rid of unwanted characters
  - Data Visualization


### EDA:

- Dataset
  - Mean balance is 1564 
  - Balance frequency is frequently updated on average 0.9
  - Purchases average is 1000
  - one off purchase average is 600
  - Average purchases frequency is around 0.5
  - average ONEOFF_PURCHASES_FREQUENCY, PURCHASES_INSTALLMENTS_FREQUENCY, and CASH_ADVANCE_FREQUENCY are generally low
  - Average credit limit is 4500
  - Percent of full payment is 15%
  - Average tenure is 11 years
  - Really good opportunity to add visualizations
- Correlation
  - Correlation between PURCHASES and ONEOFF_PURCHASES and INSTALLMENTS_PURCHASES 
  - Trend between PURCHASES and CREDIT_LIMIT and PAYMENTS
  - PURCHASES have high correlation between ONEOFF_PURCHASES, INSTALLMENTS_PURCHASES, 
  - PURCHASES_TRX(purchase transactions), CREDIT_LIMIT and PAYMENTS. 
  - Strong Positive Correlation between PURCHASES_FREQUENCY and PURCHASES_INSTALLMENT_FREQUENCY


### Data Preprocessing

   - Scaling
   - PCA
   
   
### Modeling:
  - K-Means
  - Autoencoder
