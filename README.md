# Lending CLub
## Machine Learning CUNEF 2020
### Authors:
#### Hugo César Octavio del Sueldo `hugo.delsueldo@cunef.edu`
#### Jose López Galdón `jose.lopez@cunef.edu`

***

#### Objective
The objetive of this exercise is to classificate our current and old customers in order to predict if the new clientes will pay the loan or not.

#### Target

The target we want to predict is the `loan_status` variable.

#### Data

Initially we have 4 datasets with the information of our clients, to proceed with the data analysis we merged them into one dataset. The shape of this data is 884876 rows × 151 columns.

#### EDA

After performing an Exploratory Data Analysis and selecting the best variables we got a 425015 rows × 51 columns dataset.

#### Processing data

In order to perform the next algorithms, we processed the data (sclaing, one hot enconding...) and created our TRAIN, VALIDATION and TEST datasets.

#### Predictions

 Algorithms            |Accuracy|ROC-AUC
-----------------------|--------|--------
Logistic Regression    | 76.11 %| 0.72
Support Vector Machine | 58.89 %| 0.51
Random Forest          | 76.25 %| 0.73
XGBoost                | 76.58 %| 0.73
K-Nearest Neighbors    | 73.80 %| 0.59
XGBoost Tuned          | 73.42 %| 0.73

#### Conclusions

The best model is the XGboost tuned, beacause it has the best accuracy, precissions, recalls and f1-score. But as we can see the differences between the metrics are very low, so if we have to conclude which is the best one for production would be the Logistic Regression because it is clearly interpretable and faster than the XGboost or Random Forest Classifier.

***

#### Repository structure

- _README.md_ <- The top-level README for developers.

- _data_
  - 01_raw <- Immutable input data
  - 02_intermediate<- Cleaned version of raw
  - 03_processed <- Data used to develop models
  - 04_models <- trained models

- _html- <- html of the notebooks.

- _notebooks_ <- Jupyter notebooks.

- _references_ <- Data dictionaries, manuals, etc.

- _requirements.txt_ <- The requirements file for reproducing the analysis environment.

- _.gitignore_ <- Avoids uploading data, credentials, outputs, system files etc





