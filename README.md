# Credit Card Fraud Detection

## Project Overview
This project involves detecting fraudulent credit card transactions using machine learning techniques. The dataset used contains transactions made by European cardholders in September 2013. It includes 284,807 transactions, out of which 492 are classified as frauds, representing an imbalance where frauds account for only 0.172% of all transactions.

### Dataset Information
The dataset consists entirely of numerical variables, most of which are the result of a PCA (Principal Component Analysis) transformation. Features `V1, V2, ..., V28` are the principal components obtained through PCA. Two features, `Time` and `Amount`, were not transformed by PCA:
- **Time**: Seconds elapsed between each transaction and the first transaction in the dataset.
- **Amount**: The transaction amount, which could be used for example-dependent cost-sensitive learning.
- **Class**: The response variable, where `1` indicates fraud and `0` indicates non-fraud.

### Key Challenge
The primary challenge in this dataset is the extreme class imbalance, as frauds make up only a small fraction of the overall transactions. This makes evaluating model accuracy using traditional metrics like accuracy less meaningful. Instead, metrics such as the Area Under the Precision-Recall Curve (AUPRC) are more appropriate.

### Objective
The goal of the project is to build a machine learning model that accurately identifies fraudulent transactions while addressing the class imbalance issue.

## Getting Started

### Prerequisites
To run this project, ensure you have the following installed:
- Python 3.x
- Required libraries (install them using the `requirements.txt` file)
