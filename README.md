# Loan-Default-Prediction

The aim of this project is to mine actual bank transaction data to solve a problem of interest to your client which is a large Italian bank seeking to reduce bad loans. The goal is to produce estimates of probability of that firm defaulting on the loan within the next 12 months.

Following methodology was followed in this project:
1. Data Understanding
2. Data Preparation
3. Modeling 
4. Evaluation
5. Deployment

## Prerequisite to Run :

1. Kindly install imbalanced-learn
Eg. conda install -c conda-forge imbalanced-learn
2. We require python3.7 to run

## Execution

To get predictions on a dataset please use the test_harness() function in the python notebook:

Eg. predicted_probabilities = test_harness(test_data, data_path = “/path/to/data”)

The following parameters need to be provided to it:

1. test data
2. data path (where we store the pickled model, preprocessing parameters and the external data).

Return value: probability of default (our model predictions) for each record.

### Testing using Decision Tree Classifier

To train the Decision Tree Classifier please use estimator() function: 

The following parameters need to be provided to it:

1. cleaned_data (output of preprocessor)
2. fitting_algo
3. calibrator  (creation shown in notebook)
4. est_params (creation shown in notebook)

Return value: model
