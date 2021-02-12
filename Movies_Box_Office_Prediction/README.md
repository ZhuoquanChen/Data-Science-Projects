# TMDB_Box_Office_Prediction

## Problem Statement

Watching movies is now one of people's choices for leisure and recreation. As we all know, some movies make a lot of money at the box office, while others make a lot of money at the box office. So what determines the box office? The purpose of this project will try to predict the box office of a movie based on some information before its release.


## Data:
- TMDB Box Office dataset
- Kaggle. https://www.kaggle.com/c/tmdb-box-office-prediction/data
- This dataset includes a train.csv and test.csv, which are 3000*23 and 4398*22
  
  
## Methodology:

### Data Cleaning 
- Extract data in some JSON-formatted data columns, such as key actors, themes, categories, series, publishers, etc
- Getting rid of unwanted data and null

### EDA:
- See the revenue of different language movies
- The status of movies release on weekday
- The revenue of weekday
- movies release by months

### Data Preprocessing
- Log transforms
- Scaling
      
### Modeling:
  - Linear Regression
  - Random Forest
  - Lasso
  - Bagging
  - GradientBoosting
  - Neural Networks
  - Gridsearching/hyperparameter tuning
