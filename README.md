# Loan-Default-Prediction

## Prerequisite :

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
