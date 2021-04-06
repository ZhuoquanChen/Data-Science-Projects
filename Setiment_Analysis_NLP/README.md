# Setiment Analysis for Alexa

  This project used NLP technology that can immediately judge a customer whether satisfy a product or not with their sentiment analysis. It can greatly reduce manual judgment, thus saving lots of time and money for enterprises.
    - Visualized the phrases basis of key judgment results
    - Naive Bayes Model with 91.7% accuracy for new data
    - Logistic Regreesion Model with 94.7% accuracy for new data
   

### Problem Statement

  I worked as a Data Scientist in Amazon. Currently, the Products Department collected extensive data on the text reviews of their products at alexa from global customers. Based on this data, the Product Department would like me to build a model to predict whether customers are satisfied with the products or not.


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

  - Data Preprocessing
    - Data augmentation (encoding categorical variables)
    - Using CountVectorizer for text data
    - Tokenization
    - Vectorizing
   
   
### Modeling:

  - Naive Bayes - MultinomiaNB
  - Logistic Regression
  - GridsearchCV
  
### Results:

  - MultinomiaNB - training scores: 0.938, testing scores: 0.917
  - Logistic Regression - training scores: 0.973, testing scores: 0.947

  
### Conclusions:

  The confusing matrixes show that both Naive Bayes and Logistic Regression performed well, the accuracies are up to 90%. The surprise here is that the Logistic Regression model is performing better than Naive Bayse in this case. 
