# TitanicSurvival
Predict survival of Titanic passengers

![Titanic](https://github.com/ReinhardSellmair/TitanicSurvival/blob/master/Titanic.PNG)

This repository contains all R Markdown files I wrote for the Kaggle Titanic challenge https://www.kaggle.com/c/titanic.
Kaggle account: https://www.kaggle.com/reisel

## File descriptions

ReconstrucFamilies.Rmd 
Use name feature to extract family relations (parents/children, siblings, spouses) among passengers.

featureEngineering.Rmd 
Create features: SameTicketNumber, CabinSide, and Deck
Impute missing values to the features: Fare, Embarked, Age, and Deck                        

iterativePrediction.Rmd 
Include passengers' relatives survival feature in prediction - update this feature iteratively, 
applied predictors: logistic regression, KNN, SVM, random forest, Naive Bayes, decision tree, 
hyperparameter tuning via grid search

featureCorrelation.Rmd
Apply methods to reduce number of features: recursive feature elimination (RFE), Lasso regularisation, PCA
assess methods by predicting survival with SVM and random forest and compare scores

ValidationSetCreation.Rmd
Apply methods to create a validation data set which is representative for the test set. Assess results by comparing prediction accuracy on validation set with public score.
