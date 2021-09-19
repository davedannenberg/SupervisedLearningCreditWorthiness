# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

The purpose of this analysis is to determine the accuracy of predictive modeling in predicting creditworthiness. 
Many more borrowers were creditworthy than high-risk, so a resampling (specifically, oversampling) was performed in order to ensure that the model didn't undersample high-risk borrowers.
Value counts were obtained during the fitting process to understand how the model was fit to the training data.
The predictions were applied to the testing data once the model was trained.
Those predictions were then analyzed for accuracy.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
The accuracy score was 95%. This indicates how many "true" positive and negatives there were, as opposed to false positives/negatives, out of all the data. 
The precision of the model 1 in predicting low-risk borrowers was 100%, and in predicting high-risk borrowers it was 85%, meaning it failed to correctly identify 15% of high-risk borrowers that it detected.
The recall of the model 1 in predicting low-risk borrowers was 99%, and in predicting high-risk borrowers, it was 91%, meaning it failed to detect 9% of high-risk borrowers in the data set.

* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.
The accuracy score was 99%. This indicates how many "true" positive and negatives there were, as opposed to false positives/negatives, out of all the data. 
The precision of the model 2 in predicting low-risk borrowers was 100%, and in predicting high-risk borrowers it was 84%, meaning it failed to correctly identify 16% of high-risk borrowers that it detected.
The recall of the model 2 in predicting low-risk borrowers was 99%, and in predicting high-risk borrowers, it was 99%, meaning it failed to detect only 1% of both low and high-risk borrowers in the data set.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

It seems that model 2 performed a little better, because although the precision in detecting high-risk borrowers was slightly less than in model 1, it had more complete recall, so on an aggregate basis, it will be more accurate. This is reflected in the higher F-score (88% in model 1 vs. 91% in model 2). Since high-risk borrowers can be costly to a company if they default, and because there are several factors that contribute to classifying a borrower as high-risk, it is more difficult to predict the "1"s. For this reason I would recommend model 2 over model 1, though model 2 could likely be improved.

If you do not recommend any of the models, please justify your reasoning.
