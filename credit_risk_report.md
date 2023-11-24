# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

For this analysis, it was made to look at the risk level of loans over time. The data used was lending data	with 77,000+ entries.
Using machine learning, what we needed to predict is the grouping of the loans into healthy loans and unhealthy loans, which measures
the risk factor of the loans itself. For the variables, the y variable is the loan status of the all the loans, while the X variable
is all the features that is not the loan status in the dataset. The machine learning process for this analysis was broken down into
splitting the data, creating a Logistic Regression Model that is later used to make predictions. This is later used to make predictions
on a resampled dataset using RandomOverSampler.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
  * Balanced Accuracy Score: 0.9520479254722232
  * Confusion Matrix Results: 
  	* Actual Healthy Loans vs. Predicted Healthy Loans (True Positive): 18663
	* Actual Healthy Loans vs. Predicted Not Healthy Loans (False Negative): 102
	* Actual Not Healthy Loans vs. Predicted Healthy Loans (False Positives): 56
	* Actual Not Healthy Loans vs. Predicted Not Healthy Loans (True Negatives): 563
  * Precision Scores:
	* Healthy: 100%
	* Not Healthy: 85%
  * Recall Scores:
	* Healthy: 99%
	* Not Healthy: 91%



* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.
  * Balanced Accuracy Score: 0.9936781215845847
  * Confusion Matrix Results: 
  	* Actual Healthy Loans vs. Predicted Healthy Loans (True Positive): 18649
	* Actual Healthy Loans vs. Predicted Not Healthy Loans (False Negative): 116
	* Actual Not Healthy Loans vs. Predicted Healthy Loans (False Positives): 4
	* Actual Not Healthy Loans vs. Predicted Not Healthy Loans (True Negatives): 615
  * Precision Scores:
	* Healthy: 100%
	* Not Healthy: 84%
  * Recall Scores:
	* Healthy: 99%
	* Not Healthy: 99%

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.

With both machine learning models, the one with the resampled data performed better in accuracy, but was almost the same in precision.
This is shown by their balanced accuracy scores and precision scores. According to the confusion matrices of both machine learning models,
it looks mostly the same, only having noticable differences in False Positives and True Negatives, where the second model did better in having
less false positives and more True negatives. For the models, I would recommend the second one, since it is slightly more accurate.