# Credit Card Approval Prediction

Credit Scoring is an analysis run by financial institutions to determine whether to give credit or not to clients.
Credit score uses personal data submitted by credit card applicants to predict the probability of future defaults.

Link to the Kaggle Dataset: https://www.kaggle.com/datasets/rikdifos/credit-card-approval-prediction

## How can the issuance of credit card to clients be determined?

### Summary
- Used 20 __feature__ columns and 1 __target__ column
- 12 Categorical and 8 Continuous columns
- Split data into training and validation sets using sklearn’s __train_test_split__ function.
- Used __Vintage Analysis__ to construct the label into __good__ or __bad__.
- __Undersampling__ is used to balance the skewed class distribution.
- It took less than __a minute__ to train the model.

### Feature Transformation
- The __window__ column was created from the difference between the __open_month__ and the __end_month__ . The Performance Window used are those greater than __20 months__.
- Used the __proc_data__ function to convert columns to Categorical features, and to fill NaN with modal data

### Training
Obtained an ROC AUC Score of __1.0__, a mean absolute error of __0.0__ and a mean accuracy of __1.0__

### Conclusion
- Logistic Regression is a good model for Binary Classification of the Credit Score data.
- The ROC AUC Score is __1.0__. The model really learnt well and generalized on the new data. Which validates the fact that Logistic Regression, a simple model, can be used to implement solutions to problems like Credit Scoring as quickly as possible.
- L1 penalty was used to combat overfitting by shrinking the parameters towards 0. This helped in achieving the Mean Accuracy of 1.0.



# By Ubajaka, Chijioke

## Prerequisites:
- Google Colab | IPython Notebook
- Sklearn
- Google Drive (Optional)
