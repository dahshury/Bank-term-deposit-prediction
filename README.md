<h1>Bank Term Deposit prediction</h1>

![Alt text](img.jpeg)

Exploratory Data Analysis (EDA), Data cleaning, feature extraction on 12 features and testing several ML models to predict whether a customer will subscribe to a term deposit. 
  
 <h3>About the Dataset</h3>

 [Bank Term Deposit Predictions - Kaggle.com](https://www.kaggle.com/datasets/thedevastator/bank-term-deposit-predictions)

 Predicting Subscription to Term Deposits through Marketing Campaigns

This dataset, titled Direct Marketing Campaigns for Bank Term Deposits, is a collection of data related to the direct marketing campaigns conducted by a Portuguese banking institution. These campaigns primarily involved phone calls with customers, and the objective was to determine whether or not a customer would subscribe to a term deposit offered by the bank.

The dataset contains various features that provide insights into customer attributes and campaign outcomes. These features include: age, job, martial status, education, default, balance, housing loan, contact type, day, duration, campaign contacts count, days passed since last contact, previous outcome of contact.

### Results

### Validation Data Results:

#### SGD Classifier:
- ROC Score: 0.8901

#### Classification Report for SGD Classifier:

| Metric    | Class 0 | Class 1 |
|-----------|---------|---------|
| Precision | 0.93    | 0.57    |
| Recall    | 0.95    | 0.47    |
| F1-Score  | 0.94    | 0.52    |
| Support   | 7952    | 1091    |
| Macro Avg | 0.75 | 0.71 | 0.73 |
| Weighted Avg | 0.89 | 0.89 | 0.89 |
---

#### Logistic Regression:
- ROC Score: 0.9025

#### Classification Report for Logistic Regression:

| Metric    | Class 0 | Class 1 |
|-----------|---------|---------|
| Precision | 0.92    | 0.66    |
| Recall    | 0.97    | 0.36    |
| F1-Score  | 0.94    | 0.46    |
| Support   | 7952    | 1091    |
| Macro Avg | 0.79 | 0.67 | 0.70 |
| Weighted Avg | 0.89 | 0.90 | 0.89 |
---

#### KNeighbors Classifier:
- ROC Score: 0.8026

#### Classification Report for KNeighbors Classifier:

| Metric    | Class 0 | Class 1 |
|-----------|---------|---------|
| Precision | 0.91    | 0.56    |
| Recall    | 0.97    | 0.26    |
| F1-Score  | 0.94    | 0.36    |
| Support   | 7952    | 1091    |
| Macro Avg | 0.73 | 0.62 | 0.65 |
| Weighted Avg | 0.86 | 0.89 | 0.87 |
---

#### Random Forest:
- ROC Score: 0.9148

#### Classification Report for Random Forest:

| Metric    | Class 0 | Class 1 |
|-----------|---------|---------|
| Precision | 0.92    | 0.65    |
| Recall    | 0.97    | 0.37    |
| F1-Score  | 0.94    | 0.48    |
| Support   | 7952    | 1091    |
| Macro Avg | 0.78 | 0.67 | 0.71 |
| Weighted Avg | 0.89 | 0.90 | 0.89 |
---

#### XGBoost Classifier:
- ROC Score: 0.9100

#### Classification Report for XGBoost Classifier:

| Metric    | Class 0 | Class 1 |
|-----------|---------|---------|
| Precision | 0.93    | 0.60    |
| Recall    | 0.96    | 0.46    |
| F1-Score  | 0.94    | 0.52    |
| Support   | 7952    | 1091    |
| Macro Avg | 0.76 | 0.71 | 0.73 |
| Weighted Avg | 0.89 | 0.90 | 0.89 |


The best model is Random Forest, with an F-1 score of 0.52. One possible improvement is to fine-tune the model using cross-validation and grid-search.
We also could pick a different threshold, where we would not have as many true negatives (134), but have more false positives (291). This is due to the reason that marketing resources aren't more valuable than a subscribing customer. We would rather have more calls to people who wouldn't subsribe, than not calling people who would.

### Contact Me

[Linkedin](https://www.linkedin.com/in/dahshory/)

### Acknowledgements

Thanks to [Samir Gouda](github.com/SamirGouda) & [Omar Eldahshoury](github.com/omareldahshoury) for thier support.
