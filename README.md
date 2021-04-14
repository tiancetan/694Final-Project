# Final-Project
# Human Activity Recognition from Continuous Ambient Sensor Data

## Intro of the project

Data description:

Source: UCI 

https://archive.ics.uci.edu/ml/da![Uploading Screen Shot 2021-04-14 at 11.17.26 AM.png…]()
tasets/Human+Activity+Recognition+from+Continuous+Ambient+Sensor+Data

- Data are collected by sensors continuously while residents perform their normal routines.

- the dataset is about 54.34 GB

- 37 attributes

- Multi-classification(45 classes)

__Analytics Goal/Novelty:__

Compare ML models’ performance by f1 scores

- Random Forest
- Logistic Regression (OnevsRest)
- XGBoost
- Deeplearning
- Multi-Layer-Perception

Compare different hyperparameters’ performance

## Data Pipeline

__S3 -> EMR(preprocessing) -> S3(data storage) -> EMR(Modeling)__

## Data preprocessing algorithm details

- Dropped null/missing values
- Vectorized feature columns
- Clean misspelling category name in target column
- Encode target column
- Normalize data
- Apply PCA to reduce data dimensions

## Result

<img width="727" alt="Screen Shot 2021-04-14 at 11 15 53 AM" src="https://user-images.githubusercontent.com/69778068/114743947-c9782b00-9d12-11eb-867c-5ded86da2a60.png">

