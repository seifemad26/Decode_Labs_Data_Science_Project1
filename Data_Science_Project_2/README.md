# Credit Card Fraud Detection Project

## Project Overview
This project aims to build a robust machine learning pipeline to detect fraudulent credit card transactions. Given the highly imbalanced nature of the dataset (where fraud represents only 0.17% of transactions), the project focuses on handling class imbalance using various sampling techniques and evaluating models using precision-recall metrics.

## Key Features
- **Exploratory Data Analysis (EDA)**: Comprehensive visualization of class imbalance and feature distributions.
- **Data Preprocessing**: Standard scaling of numerical features and handling of time/amount columns.
- **Imbalance Handling**: Implementation of **SMOTE (Synthetic Minority Over-sampling Technique)**, Random Over-sampling, and Random Under-sampling.
- **Machine Learning Models**:
  - Logistic Regression (Baseline)
  - Random Forest Classifier
  - Dummy Classifier (for performance comparison)
- **Model Evaluation**: Focus on ROC-AUC, Precision-Recall curves, and Confusion Matrices to ensure high recall for the minority class.

## Dataset
The project uses the [Credit Card Fraud Detection dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud), which contains transactions made by credit cards in September 2013 by European cardholders.
- **Total Transactions**: 284,807
- **Fraudulent Transactions**: 492 (0.17%)
- **Features**: 30 numerical features (V1-V28 are PCA-transformed, plus Time and Amount).

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/credit-card-fraud-detection.git
   cd credit-card-fraud-detection
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Usage
Open the Jupyter notebook to view the analysis and model training:
```bash
jupyter notebook pasted_file_byosSP_DataScienceProject2.ipynb
```

## Results
The Random Forest model combined with SMOTE achieved significant performance in detecting fraudulent transactions while maintaining a low false-positive rate. Detailed metrics and confusion matrices are available within the notebook.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
