# Credit Card Approval Prediction
## Project Description
This project aims to predict the likelihood of a credit card application being approved based on applicant data. By analyzing various demographic and financial features, we can build a model to help financial institutions improve the accuracy of their credit approval decisions.

The primary goal is to explore, train, and compare three different machine learning models:
1. K-Nearest Neighbors (KNN)

2. Random Forest

3. Neural Network (NN)

We will evaluate these models based on performance metrics like Accuracy, Precision, Recall, and F1-score to determine the most effective approach for this dataset, paying close attention to the significant class imbalance.

## Dataset
The dataset is sourced from the "Credit Card Approval Prediction" dataset found on Kaggle. It consists of two main files: 
1. `application_record.csv ` that contains applicant demographic, income, and other personal information.
2. `credit_record.csv` that contains historical monthly credit status data for applicants.

A key part of the project involves cleaning, merging, and engineering these two datasets to create a unified dataset (clean_merged.csv) with a suitable target variable (label) derived from the applicant's payment history.

## Project Structure
```plaintext
.
│
├── .gitignore          # Specifies files and folders for Git to ignore
├── README.md           # This file, explaining the project
├── requirements.txt    # A list of all Python package dependencies
│
├── data/
│   ├── application_record.csv  # Raw applicant data
│   ├── credit_record.csv       # Raw credit history data
│   └── clean_merged.csv        # The final, cleaned dataset (output of data_cleaning.ipynb)
│   └── to be updated
│
├── drafts/
│   └── (Notebooks and scripts for experimentation, ignored by .gitignore)
│
├── src/
│   ├── data_cleaning.ipynb     # Notebook for all cleaning, merging, and EDA
│   ├── data_processing.ipynb   # Notebook for processing and smote
│   ├── knn_model.ipynb         # Notebook for KNN modeling
│   ├── random_forest_model.ipynb # Notebook for Random Forest modeling
│   └── neural_network_model.ipynb # Notebook for NN modeling
│
└── models/
    └── (Saved model files, e.g., .pkl or .h5, can be saved here)
```