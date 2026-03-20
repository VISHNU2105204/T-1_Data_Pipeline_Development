# TASK - 1
# DATA_PIPELINE_DEVELOPMENT

*COMPANY*: CODTECH IT SOLUTIONS

*NAME*: BADIMELA VISHNU VARDHAN

*INTERN ID*: CTIS1342

*DOMAIN*: DATA SCIENCE

*DURATION*: 12 WEEKS

*MENTOR*: NEELA SANTHOSH

## This project implements an end-to-end Machine Learning ETL (Extract, Transform, Load) pipeline designed to predict vehicle CO2 emissions based on various automotive specifications. As a Computer Science and Engineering student specializing in AI, this work demonstrates a structured approach to building reproducible data workflows and predictive models.

## Extraction: The process begins by ingesting vehicle data from a CSV source. The dataset contains information on 935 vehicle entries, focusing on features like engine size, fuel consumption, and smog levels.

## Transformation: To prepare the data for the model, a robust preprocessing strategy was implemented using ColumnTransformer.

## Numerical Features: Columns such as Engine_Size and Fuel_Consumption_comb(L/100km) undergo mean imputation to handle missing values and StandardScaler to normalize the data scales.

## Categorical Features: Variables like Make, Model, and Transmission are processed using most-frequent imputation and OneHotEncoder to convert text-based categories into a machine-readable format.

## Modeling: A Random Forest Regressor was integrated into the final pipeline. This ensemble method was chosen to capture non-linear relationships between engine characteristics and emission levels.

## Loading & Persistence: The fully trained pipeline including both the preprocessing steps and the model—is serialized and saved as a .joblib file. This ensures the model can be easily deployed or reloaded for future predictions without retraining.

## The model was evaluated on a test set (20% of the data) and achieved high accuracy:
## R^2 Score: 0.9742, indicating the model explains over 97% of the variance in $CO_2$ emissions.
## RMSE: 10.1898, representing the standard deviation of the prediction errors.
## MAE: 3.0989, showing that on average, predictions deviate by only about 3 units from the actual emission values.
