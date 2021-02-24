### Problem Statement

  Hiring and retaining top talent is an extremely challenge because companies spend 15-20 percent of the employees' salary to recruit in a new candidate. In this case, HR team extensive data on their emplyees, and ask for developing a model that could predict which employees are more likely to quit.


### Data:

  Human_Resources.csv from Kaggle
  
  
### EDA:

  - visualizations
    - Histgram
      - Some features are tail heavy
      - Drop 'EmployeeCount', 'Over18', 'StandardHours' because there are only one value for each
    - Heatmap
      - JobLevel is strongly correlated with total WorkingHours
      - MonthlyIncome is strongly correlated with JobLevel
      - MonthlyIncome is strongly correlated with total WorkingHours
      - Age is stongly correlated with MonthlyIncome
    - Countplot
      - Single employees tend to leave compared to married and divorced
      - Sales Representitives tend to leave compared to any other job
      - Less involved employees tend to leave the company
      - Less experienced (low JobLevel) tend to leave the company


### Data Preprocessing

   - One hot encoding
   - Data over sampling
   - Data Scaling
   
   
### Modeling:

  - Logistic Regression
  - Random Forest
  - Pipeline
  - Grid search

  
### Evaluation:

  - Confusion matrix

  
### Conclusions:

  In this case, both of Logistic Regression model and Random Forest model didn't have a very good performance. I think if we want to have a high accuracy for retention of employees that based on this dataset is not enough. Employees' turnover there are many factors, and most of them would be invisible. Thus, We should use the an employee's behavioral characteristics to predict whether an employee wants to leave or not. That's would be more reasonable.
