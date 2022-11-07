# Predicting telecom client churn 
This is the final project of the Practicum DS course, combining all the sprints.

## Description
Here we have a dataset on telecom clients plans and contract information. We aim to predict if a client is likely to leave, so we could suggest them special plan options.

First, we should do some data preprocessing: clean the data, fill in the missing values (if any), change data types and merge the data. Next, we need to construct additional features, scale and encode the data. Afterward, we could proceed to model development.

## Conclusion
After preprocessing, we explored several models and picked the CatBoost model as it showed the best ROC-AUC score. Extracting feature importance from the model allowed us to exclude eight features that didn't decrease the impurity so our final model could train and predict faster. Our best model is **CatBoostClassifier** with a ROC-AUC score on the test data of 0.91.