# Problem-Statement-Demographic-Data

## Domain
This problem is drawn from the analysis census demo graphic data. Similar analysis has been done when it come to the gender pay gap or when it comes to assessing demographic data by tax bracket. Sample source:
https://docs.microsoft.com/en-us/azure/machine-learning/preview/scenario-tdsp-classifying-us-incomes

## Problem Statement
For a person with a given set of demographic features were will use supervised learning to develop a classification model to predict whether a given person's wage is less/equal to 50k or higher than 50k. 

In Tom Mitchell's words of a machine learning problem:
'A computer program (in this case R) is said to learn from experience E(the census data set) with respect to some class of tasks T (the various demographic features in correlation with the target wage class) and performance measure P, if its performance at tasks T, as measured by P, improves with experience E.' 

In other words is it possible to predict the wage class by a combination of demographic features with more certainty than using the mean or most common class.

## Dataset and Inputs
The dataset to be examined contains the following features age, the work class, the education, the marital status, the occupation, race, sex, the hours worked per week, and the native country in connection with the target, the wage class.

The dataset has 32,560 rows and 15 columns and uses up 3.8M GB in memory.

## Solution Statement
A solution to this problem will be a classification model such as a logistic regression, decision tree, random forest, gradient-boosted tree, multilayer perceptron, one-vs-rest.

## Benchmark Model
Given that we seek a classification model a good naive benchmark would be to guess the most common class.

## Evaluation Metrics
The dataset is evenly distributed unevenly as the wage class =<50k is represented almost three times as often as the >50k wage class. We can use the success of the model measuring against the F-Score and determine if our model predicts the correct wage class more reliably than the F-Score.
