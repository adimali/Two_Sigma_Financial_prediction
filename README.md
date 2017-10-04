# Two Sigma Financial modeling project

This is the Readme for my Two Sigma Financial modeling project.
dataset used in this project can be found at Kaggle 2sigma competition [website](https://www.kaggle.com/c/two-sigma-financial-modeling/data)

## Initial_EDA.ipynb
This notebook contains exploratory data analysis of the dataset. In this notebook outliers and cutoff points for all the feature columns were  identified using histograms.

## Data_Preprocessing_1-3
These notebooks contain the Preprocessing steps used in removing outliers or transforming the original data.
 - Data_Preprocessing_1
   - Remove outliers according to predefined limits from Initial EDA notebook.
   - Apply nonlinear transformation using [QuantileTransformer](http://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.QuantileTransformer.html): uniform distribution.
 - Data_Preprocessing_2
   - Apply nonlinear transformation using [RobustScaler](http://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.RobustScaler.html).
   - Apply nonlinear transformation using [QuantileTransformer](http://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.QuantileTransformer.html): normal distribution.
 - Data_Preprocessing_3
   - clip each feature at predefined values obtained from Initial EDA notebook.

## Feature_selection_1-4
These notebooks contain the feature selection steps used in selecting the best features for preprocessed datasets. correlation with target variable 'y', [SelectKBest](http://scikit-learn.org/stable/modules/generated/sklearn.feature_selection.SelectKBest.html#sklearn.feature_selection.SelectKBest) and feature_importances_ in [ExtraTreesRegressor](http://scikit-learn.org/stable/modules/generated/sklearn.ensemble.ExtraTreesRegressor.html) were used to score the feature importance.

## Implementation* notebooks
These notebooks contain different models fit to the training data.
 - multiple linear regression
 - multiple Ridge regression
 - random forest regressor
 - AdaBoost regressor
 - ExtraTrees Regressor
 - SVR
Models were validated and evaluated using cross validation and held out test set. 


## Creators

* Adimali Piyadasa
    - [https://adimali.github.io/](https://adimali.github.io/)
