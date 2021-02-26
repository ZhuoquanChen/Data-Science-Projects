### Problem Statement

  Let's say I have been hired as a consultant to a bank in New York City. The bank has extensive data on their customers for the pass six months. They want to have a model that can cluster customers into different groups or categories by launching a targetted ad marketing campaign.


### Data:

  - Data Source: [SAT](https://www.kaggle.com/arjunbhasin2013/ccdata)
  
  
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
