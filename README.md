# Credit Card Fraud Detection System

## Overview

This is a credit card fraud detection system built using logistic regression. It helps in identifying fraudulent credit card transactions.

## Dataset Information
The dataset contains transactions made by credit cards in September 2013 by European cardholders. This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions.

It contains only numerical input variables which are the result of a PCA transformation. Unfortunately, due to confidentiality issues, we cannot provide the original features and more background information about the data. Features V1, V2, … V28 are the principal components obtained with PCA, the only features which have not been transformed with PCA are 'Time' and 'Amount'. Feature 'Time' contains the seconds elapsed between each transaction and the first transaction in the dataset. The feature 'Amount' is the transaction Amount, this feature can be used for example-dependant cost-sensitive learning. Feature 'Class' is the response variable and it takes value 1 in case of fraud and 0 otherwise.

Given the class imbalance ratio, we recommend measuring the accuracy using the Area Under the Precision-Recall Curve (AUPRC). Confusion matrix accuracy is not meaningful for unbalanced classification.

## Requirements

- Python 3.x
- scikit-learn
- pandas
- numpy
- matplotlib
- seaborn

## Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/your_username/credit-card-fraud-detection.git
    ```

2. Navigate to the project directory:

    ```bash
    cd credit-card-fraud-detection
    ```

3. Install the required dependencies:

    ```bash
    pip install -r pandas sklearn numpy seaborn matplotlib
    ```

## Usage

1. Open `credit_card_fraud_detection.ipynb` in a Jupyter Notebook environment.

2. Follow the instructions provided in the notebook to train the logistic regression model and evaluate its performance.

## Dataset

The dataset used for this project is the [Credit Card Fraud Detection dataset](https://www.kaggle.com/mlg-ulb/creditcardfraud) from Kaggle.

## Model

The model used for this project is logistic regression.

## Evaluation

The performance of the model is evaluated based on accuracy and F1-score.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
