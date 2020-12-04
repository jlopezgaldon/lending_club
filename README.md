# Lending CLub
## Machine Learning CUNEF 2020
### Authors:
####Hugo César Octavio del Sueldo y Jose López Galdón

***

#### Objective
The objetive of this exercise is to classificate our current and old customers in order to predict if the new clientes will pay the loan or not.

#### Target

The target we want to predict is the `loan_status` variable.

#### Data

Initially we have 4 datasets with the information of our clients, to proceed with the data analysis we merged them into one dataset. The shape of this data is 884876 rows × 151 columns.

#### EDA

After performing an Exploratory Data Analysis and selecting the best variables we got a 407319 rows × 30 columns dataset.

#### Processing data

In order to perform the next algorithms, we processed the data (sclaing, one hot enconding...) and created our TRAIN, VALIDATION and TEST datasets.

#### Predictions

 Algorithms            |Accuracy
-----------------------|--------
Logistic Regression    | 80.32 %
Support Vector Machine | 67.23 %
Random Forest          | 80.41 %
XGBoost                | 80.22 %
K-Nearest Neighbors    | 76.89 %
XGBoost Tuned          | 80.49 %

#### Conclusions

The best model is the XGboost tuned, beacause it has the best accuracy, precissions, recalls and f1-score. But as we can see the differences between the metrics are very low, so if we have to conclude which is the best one for production would be the Logistic Regression because it is clearly interpretable and faster than the XGboost or Random Forest Classifier.




