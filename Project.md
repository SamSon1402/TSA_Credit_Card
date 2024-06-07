# Credit Card Fraud Detection

## Overview
This project aims to detect fraudulent credit card transactions using machine learning techniques. The dataset consists of transactions made by European cardholders in September 2013. With the prevalence of credit card fraud, it is crucial for financial institutions to identify and prevent fraudulent activities to protect customers and minimize losses.

## Dataset Description
The dataset contains transactions over two days, including 492 fraudulent transactions out of a total of 284,807 transactions. Due to confidentiality issues, the original features are not provided; instead, the data has been transformed using Principal Component Analysis (PCA). The dataset includes the following features:

- `Time`: Seconds elapsed between each transaction and the first transaction in the dataset.
- `Amount`: The transaction amount, which can be used for cost-sensitive learning.
- `Class`: The response variable, where 1 indicates a fraudulent transaction and 0 indicates a non-fraudulent transaction.
- `V1`, `V2`, ..., `V28`: Principal components obtained via PCA.

The dataset is highly unbalanced, with the positive class (frauds) accounting for only 0.172% of all transactions.

## Recommended Evaluation Metric
Given the class imbalance, traditional accuracy metrics may not be informative. We recommend using the Area Under the Precision-Recall Curve (AUPRC) for evaluation. The confusion matrix accuracy is not meaningful for unbalanced classification.

## Getting Started

### Prerequisites
To run the project, you need to have the following software installed:
- Python 3.6 or higher
- Jupyter Notebook (optional, for interactive exploration)

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/credit-card-fraud-detection.git
   cd credit-card-fraud-detection
