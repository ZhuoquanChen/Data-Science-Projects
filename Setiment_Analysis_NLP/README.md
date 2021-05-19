### Overview

Nature language processing can be used to build predictive models to perform sentiment analysis on social media posts and reviews. It works by converting words into numbers and training a machine learning model to make predictions. In that way, we can know if customers are happy or not without manually going through a number of posts and reviews information.

In this project, I leveraged data science skills to deal with text data, perform exploratory data analysis, create world could visualizations, apply natural language processing toolkit to perform tokenization, apply feature extraction by using CountVectorizer, deal with unbalanced data set to train in Naive Bayes classified model and Logistic Regression model.

The purpose of this project is to determine a customer whether satisfied or not with a product of Amazon by analyzing their feedback.
  - Naive Bayes Model with 91.7% accuracy for new data, and with 89% accuracy for detecting people who are not satisfied.
  - Logistic Regression Model with 94.7% accuracy for new data, and with 89% accuracy for detecting people who are not satisfied.
   

### Problem Statement

I work as a data scientist at a multinational corporation, and the Public Relations Department team has provide me extensive data on the customers such as product reviews with text format. The team would like to predict whether the customers are satisfied with the product or not.


### Skills

  - NLP (Natural Language Processing)
  - Features Extraction with CountVectorizer
  - Data Visualization
  - Sampling
  - Naive Bayes Classifiers & Logistic Regression Classifiers
  - GridSearchCV
  - Confusing Matrix


### Data:

  - This dataset is about the feedback of products of Amazon alexa
  - https://www.kaggle.com/sid321axn/amazon-alexa-reviews/kernels
  
  
### Methodology:

  - Data Cleaning 
    - Removing useless columns
    - Extracing data
    - Removing punctuations

  - EDA:
    - Rates score of each product
    - Distribution of rates
    - The top frequence of positive words in customers' feedbacks
    <img src="https://github.com/ZhuoquanChen/Data-Science-Projects/blob/main/Setiment_Analysis_NLP/images/8.png" width="700" height="270"> 

  - Data Preprocessing
    - Data augmentation (encoding categorical variables)
    - Using CountVectorizer for text data
    - Tokenization
    - Vectorizing  
    <img src="https://github.com/ZhuoquanChen/Data-Science-Projects/blob/main/Setiment_Analysis_NLP/images/3.png" width="600" height="350"> 
   
   
### Modeling:

  - Naive Bayes - MultinomiaNB
  - Logistic Regression
  - GridsearchCV
  <img src="https://github.com/ZhuoquanChen/Data-Science-Projects/blob/main/Setiment_Analysis_NLP/images/6.png" width="500" height="150">
  
### Results:

  - MultinomiaNB - training scores: 0.938, testing scores: 0.917
  - Logistic Regression - training scores: 0.973, testing scores: 0.947
  <img src="https://github.com/ZhuoquanChen/Data-Science-Projects/blob/main/Setiment_Analysis_NLP/images/4.png" width="300" height="280">
  <img src="https://github.com/ZhuoquanChen/Data-Science-Projects/blob/main/Setiment_Analysis_NLP/images/5.png" width="300" height="280">

  
### Conclusions:

  The confusing matrixes show that both Naive Bayes and Logistic Regression performed well, the accuracies are up to 90%. The surprise here is that the Logistic Regression model is performing better than Naive Bayse in this case. 
