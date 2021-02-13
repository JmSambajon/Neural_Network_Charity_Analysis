# Neural_Network_Charity_Analysis

## Overview of the analysis: Explain the purpose of this analysis.

Using Machine learning and neural networks, I'll use the features in the provided dataset to create a binary classifier that is capable of predicting whether which organizations will be successful if funded by the non-profit philanthropic company, Alphabet Soup.

##Results

### Data Preprocessing
* What variable(s) are considered the target(s) for your model?
	* IS_SUCCESSFUL
* What variable(s) are considered to be the features for your model?
	* APPLICATION_TYPE
	* AFFILIATION
	* CLASSIFICATION
	* USE_CASE
	* ORGANIZATION
	* STATUS
	* INCOME_AMT
	* SPECIAL_CONSIDERATIONS
	* ASK_AMT
* What variable(s) are neither targets nor features, and should be removed from the input data?
	* EIN
	* NAME

### Compiling, Training, and Evaluating the Model
* How many neurons, layers, and activation functions did you select for your neural network model, and why?
	The best performance was achieved using the following:

	![layers]("Pictures/layers.png")

* Were you able to achieve the target model performance?
	No, I was not able to achieve the targeted model performance model of 75%. Those best model achieved 72.47%

	![layers]("Pictures/accuracy.png")

* What steps did you take to try and increase model performance?
	I tried optimizing the models performance by dropping "noisy" variables, try various activation functions, and adding additional neurons and hidden layers.

## Summary

This neural network model was unable to achieve the targeted performance of 75% accuracy and is determined to be an unfit model for this situation. Adjustments were made to the code multiple times but resulted in less accurate results.

An alternative model I would recommend to solve this classification problem is the Random forest classifiers model. While the deep learning model used in this module required a couple minutes to train on the tens of thousands of data points, a random forest classifier can train a large dataset and predict values a lot less time, requiring less code.