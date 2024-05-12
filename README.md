# credit-risk-classification

This analysis looked at a dataset with financial information on individuals who had taken out loans, including loan size, interest rate, borrower income, debt to income ratio, number of accounts, derogatory marks, total debt, and loan status. This data was used to create an algorithm that could be used to predict the loan status variable, which was either a healthy loan (0), suggesting that person was safe to lend to, or a high-risk loan (1), suggesting that person was risky to lend to. 

After dividing the data into labels (loan status) and features (all other data), the data was split 70/30 into training and testing data. The training data was used to fit a logistic regression model algorithm. After training the model with data, the model was used to make predictions using the testing data, and compared to the actual data labels.

The performance of the logistic regression model was evaluated by accuracy, precision and recall scores, as well as a confusion matrix.  
* The accuracy score of the logistic regression model was 0.99, showing that the model is quite good overall at accurately predicting loan status risk. 
* The precision scores of the logistic regression model were 1.00 for healthy loans, and 0.87 for high-risk loans, showing that the model gives results with higher reproducibility for healthy loans than risky loans.
* The recall scores of the logistic regression model were 1.00 for healthy loans, and 0.89 for high-risk loans. This along with the confusion matrix show a higher false positive rate (i.e. someone being classified as high-risk when they actually are low risk) than a false negative rate (i.e. someone being classified as low-risk when they actually are high risk)

Overall, the logistic regression model has a high accuracy score and performs well at predicting loan status risk. The model does have higher precision and recall for predicting 0s (healthy loans) than 1s (high-risk loans). However, the higher false positive than false negative rate is to the benefit of the company. The risk of losing a potential customer due to incorrectly labeleing them as high-risk does not have as detrimental consequences as incorrectly labeling a customer as low-risk, approving a loan, and having them default on the loan. Therefore, I would recommend the use of the logistic regression algorithm to predict credit risk in individuals seeking loans. 
    
    