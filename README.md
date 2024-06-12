# credit-risk-classification

# Module 20 Report 

## Overview of the Analysis


The purpose of the analysis was to build a model that can identify the creditworthiness of borrowers. 
For the analysis and building a model of historical dataset has been used from a peer-to-peer lending services company


Date set included following relevant information:

    -  size of the loan
    -  interest rate
    -  borrower's income
    -  debt to income ratio
    -  number of account a borrower hold
    -  number of derogatory marks 
    -  total debt
    -  loan status

### Method used

To predict the the loan status (0 - healthy loan, 1 loan at a high rist of defaulting) Logistic Regression model has been used.
Logistic Regression model is used for predicting binary outcomes from date ( in this cases healthy vs unhealthy loan).

The process involved:

    1. Preprocessing
    2. Splitting the data - dividing the dataset into training and testing sets using a 75%-25% split with train_test_split and random_state=1 to ensure reproducibility
    3. Training the Model: fitting the Logistic Regression model to the training data.
    4. Prediction: Using the trained model to predict loan statuses on the test set.

## Results


* Logistic Regression, following scores have been achieved:
  
        1. Accuracy : 99%
        2. Precision: 
            * healthy loans: 1.00 
            * unhealhy loans: 0.85 
        3. Recall: 
            * healthy loans: 0.99 
            * unhealhy loans: 0.91
## Summary


With overall accuracy of 99% we can confirm that the logistic regression model perfomance is very good.
Howevery, the precision for predicting unhealthy loans is relatively low (only 85%) compared to 100 % for good loans.
Similarly, the recall scores the recall scores are higher for healthy loans (99 %) nd slightly lower for bad loans (91% of actual positives were labeled as positive).

If the goal is to predict unhealthy loans more accurately, this model might fall short, and it would be advisable to explore other models. However, if the primary interest is in predicting healthy loans, this model performs very well.


