# Final-Project
# Human Activity Recognition from Continuous Ambient Sensor Data

## Intro of the project

Data description:
- Source: [UCI](https://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+from+Continuous+Ambient+Sensor+Data) 
- Data Set Characteristics: Multivariate, Sequential, Time-Series
- This dataset represents ambient data collected in homes with volunteer residents.
Data are collected continuously while residents perform their normal routines.
Ambient PIR motion sensors, door/temperature sensors, and light switch sensors
are placed throughout the home of the volunteer. The sensors are placed in locations
throughout the home that are related to specific activites of daily living that we
wish to capture.
- The classification task is to predict the activity that is occurring in the smart
home and being observed by the ambient sensors. The sensors communicate using the
ZigBee Pro protocol, forming a mesh network with all battery powered sensors as leaf
nodes and always-on devices (light switches and ZigBee relays) forming the branches
that connect back to the USB gateway on our local SHiB server.

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

