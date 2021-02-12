# Games-Classification
Webscraping, APIs, and Natural Language Processing (NLP)

# Problem Statement
Scrape a games post from Reddit and develop a Natural Language Processing model that identify which content of posts belong to board games and which content of posts belong to card games. In addition, it would be better if was able to find more insight with all content.
- Used CountVectorizer to tokenize datasets
- Used couple models, like Logistic Regression, RandomForest, Gradient Boosting Regression Tree.
- In the evaluation part, I uses confusion matrix 

# Data
Used Web APIs scrape game posts as datasets.
- Scraped from Reddit
- Corpus: 4000 documents
- Feature amount: 5
- Type: String

# Methodology
Data Cleaning
- Getting rid of unnecessary features
- Data combination

# EDA
- found and visualized the distribution of length of authors' names
- found the median number of words of title 
- found and visualized the distribution of number of words of title
- found the average of letters of author's names between the calsses of board games and card games
- found and visualized the most / least 20 most common words in dataset

# Modeling
- Used features as title and subreddit
- Used Logistic Regression, RandomForest, Gradient Boosting Regression Tree
- Used GridSearch and hyperparameter tuning

# Result
- Logistic Regression, Train score:  0.622, Test score:  0.636, Confusion matrix, accuracy: 0.636
- RandomForest, Train score:  0.866, Test score:  0.834, Confusion matrix, accuracy: 0.834
- Gradient Boosting Regression Tree, Train score:  0.866, Test score:  0.834, Confusion matrix, accuracy: 0.834

# Conclusion
- In Logistic Regression model, evaluation metric tell its sensitivity is 0.625, specificity is 0.648
- In RondomForest model, evaluation metric tell its sensitivity is 0.786, specificity is 0.901
- In Gradient Boosting Regression Tree, evaluation metric tell its sensitivity is 0.786, specificity is 0.901


# Next Steps
I would like to change CountVectorizer to TfidfVectorizer to try and want to see how that outcomes are different.


