# Module_12_Challenge
***
## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
> The purpose of this analysis is to use a provided csv dataset of historical lending data to build & evaluate a predictive model that determines the creditworthiness of potential borrowers.
* Explain what financial information the data was on, and what you needed to predict.
> The provided csv file gave histoical lending data on borrowers.  The features of the data set included loan size, interest rate, borrower income, debt to income, number of accounts, derogatory marks & total debt.  The targert or response of the data set was termed loan status.  A 0 indicated a good/healthy loan and a 1 indicated a loan that was at high risk of default.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
> The data set had a total of 77,536 records.  The number of healthy loans in the data set was 75,036 and the nubmer of high risk loans was 2500.  This can be categorized as an imbalanced data set (75036 vs 2500).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).
> The stages of the ML process used for this analysis began with initial import of dependencies and a read in of the csv file used for the analysis. Next data preprocessing & EDA was undertaken. In these steps the data was split into features (X) and response (y), examined for balance and split into a training set and testing set using the train test split methodology in scikit-learn.  Following this, ML was performed on the data as presented using a model-->fit-->predict workflow.  The model utilized for this was a Logistic Regression model that was fitted to the training data and then predictions were made on the test data for outcome.  Noting earlier that the data was imbalanced, the ML process was subsequently repeated but the intial data was resampled using the random over sampler function in scikit-learn. This allowed the model-->fit-->predict process to be run on a balanced representative data set. 
## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
> Model 1 had a balanced accuracy score of 0.95 or 95%. The use of the balanced accuracy score is useful for imbalanced data sets (as is the case here) as it avoids inflated performance estimates.  Thus, we can conclude that overall Model1 was 95% "correct".
> Model 1 had a precision score of 1.0 for predicting healthy loans and a precision score of 0.85 for high risk loans. Prediction is a maeasure of how well the "positives" class is predicted. So we can say that all positives were predicted 100% correctly for the good loans and 85% correct for the high risk loans. Finally recall represents the ability to predict positives from actual positives.  Model1 was able to achieve 99% recall on the healthy loans and 91% on the high risk loans.


* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.

