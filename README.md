## This is an implementation of test task for JetBrains internship, reaction predicting project
Here's a plan for notebook `test_task.ipynb`
Common approach for text analysis without pretrained models is using Tfidf + linear model.
### At first, try to implement straightforward
Classifiers from `xgboost` and `lightgbm` libraries are used, performance on `train_test_split` is about 81%.
### Then try to do the same with basic preprocessing
Using stemmer lowers the accuracy, but removing non-alphabet characters slightly improves accuracy for `xgboost` model.
### Also try using scikit-learn LogReg
It has about 77% accuracy, which is less than classifiers.
### Build regressor, try using 2 tresholds and classifier.
Both have lower accuracy than initial classifiers.
