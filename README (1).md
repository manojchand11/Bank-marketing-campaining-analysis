# Bank-Marketing-Campaign-Analysis
This project analyzes a bank marketing campaign dataset to optimize marketing campaigns for attracting more customers to term deposit subscriptions. A term deposit is a deposit that a bank or financial institution offers with a fixed rate (often better than just opening a deposit account) in which your money will be returned back at a specific maturity time.   

### Data
The dataset contains banking marketing campaign data. We can use it to predict the marketing campaign outcome and to find out factors that affect the success of the campaign.

### Approach
- Import data and perform initial analysis
- Look at the number of rows.
- Look for missing values.
- Look at dataset columns and their values respective to the campaign outcome.
- Clean the data
- Remove irrelevant columns.
- Deal with missing and incorrect values.
- Turn categorical columns into dummy variables.
- Use machine learning techniques to predict the marketing campaign outcome- 
- Find out factors that affect the success of the campaign.

### Analysis
- The dataset is imbalanced, with more "no" values for the deposit outcome than "yes" values. Undersampling of the majority class is used to address this imbalance.
- Outliers are identified in the "pdays", "campaign", and "previous" columns. These outliers are imputed with mean values during data cleaning.
- Feature importances from the XGBoost model reveal that the most important features for predicting the campaign outcome are:
1) Customer's account balance
2) Customer's age
3) Number of contacts performed during this campaign and contact duration
4) Number of contacts performed before this campaign   

### Key Recommendations
- Focus marketing campaigns on customers with account balances greater than $1490.
- Target customers from age categories below 30 years old and above 56 years old.
- Limit the number of contacts with the customer during the campaign to a maximum of 4.

### Code
The Python script for this project is a Jupyter notebook that can be found in the repository.

### Data Source : 
https://archive.ics.uci.edu/dataset/222/bank+marketing
