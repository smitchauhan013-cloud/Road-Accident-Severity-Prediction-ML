# Road Accident Severity Prediction

This project predicts the severity of road accidents using Machine Learning models on the **US Accidents March 2023** dataset.

## Project Objective

The main objective of this project is to predict accident severity based on factors such as:

- Temperature
- Humidity
- Pressure
- Visibility
- Wind Speed
- Weather Condition
- Location features
- Time-related features

## Dataset

- **Dataset Name:** US_Accidents_March23.csv
- **Source:** Kaggle / US Accidents Dataset
- **Size:** Large-scale accident dataset with millions of records

## Workflow

The project follows a complete Machine Learning workflow:

1. Data Collection
2. Exploratory Data Analysis (EDA)
3. Data Preprocessing
4. Feature Selection
5. Data Splitting
6. Model Training
7. Model Evaluation
8. Hyperparameter Tuning
9. Model Saving / Deployment

## Data Preprocessing

The preprocessing steps include:

- Handling missing values
- Encoding categorical columns
- Feature engineering from date and time
- Weather condition simplification
- Scaling numerical features
- Feature selection

## Models Used

The following models were used in this project:

- Logistic Regression
- Decision Tree
- Random Forest
- LightGBM
- XGBoost

## Best Model

For the multiclass severity prediction task, **Decision Tree** gave strong accuracy in our experiments.

For the binary classification version (**Low vs High Severity**), advanced boosting models like **LightGBM** and **XGBoost** were also explored.

## Evaluation Metrics

The project uses the following evaluation metrics:

- Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC
- Confusion Matrix

## Features Used

Some important features used in the project:

- Temperature(F)
- Humidity(%)
- Pressure(in)
- Visibility(mi)
- Wind_Speed(mph)
- Weather_Condition
- Start_Lat
- Start_Lng
- Hour
- Weekday
- Duration_min
- Traffic-related indicator features

## Results

- Decision Tree performed well for direct severity prediction
- Binary classification improved separability between low and high severity classes
- Feature importance analysis helped identify the most influential factors

## Project Structure

```text
road-accident-severity-prediction/
│
├── US_Accidents_Project.ipynb
├── US_Accidents_Project.py
├── README.md
├── requirements.txt
├── .gitignore
└── images/
    ├── eda_overview.png
    ├── confusion_matrix.png
    ├── feature_importance.png
    └── roc_curve.png
