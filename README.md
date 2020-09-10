# Exoplanet Exploration

## Background

Over a period of nine years in deep space, the NASA Kepler space telescope has been out on a planet-hunting mission to discover hidden planets outside of our solar system.
To help process this data, machine learning models were created capable of classifying candidate exoplanets from the raw dataset.

## Models

* Support Vector Machine
* Random Forest
* Logistic Regression

## Resources

https://www.kaggle.com/nasa/kepler-exoplanet-search-results

## Steps:

### Preprocess the Data

* Preprocessed the dataset prior to fitting the model.
* Performed feature selection and remove unnecessary features.
* Use MinMaxScaler to scale the numerical data.
* Separated the data into training and testing data.


### Tune Model Parameters

* Used GridSearch to tune model parameters.

## Analysis 

|Model                 |Training Data Score|Testing Data Score|
|:--------------------:|:-----------------:|:----------------:|
|Support Vector Machine|0.8916             |0.8947            |
|Random Forest         |1.0                |0.8993            |
|Logistic Regression   |0.8811             |0.8815            |   

When comparing the three models created, it appears Support Vector Machine is the best model to predict an exoplanet. The SVM model has a training date score of .8916 and a testing data score of .8947, which are higher than the Logistic Regression scores (.811 & .8815). The Random Forest model has the highest score, however, there is wide gap between the training data (1.0), and the testing data score (.8993), which indicates the model may be overfitted.
