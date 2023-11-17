<div align="center"><h1><strong>Credit Card Fraud Detection</strong></h1></div>
<div align="center"><h3><strong>Data Analytics Project</strong></h3></div>
<br>
<div align="center"><img style="margin: auto; padding: 0px 5px 0px 5px;" src="https://img.shields.io/badge/Made%20With%20Python-FFD43B?style=for-the-badge&logo=python&logoColor=darkgreen"><img style="margin: auto; padding: 0px 5px 0px 5px;" src="https://img.shields.io/badge/Jupyter%20Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white"><img style="margin: auto; padding: 0px 5px 0px 5px;" src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white"><img style="margin: auto; padding: 0px 5px 0px 5px;" src="https://img.shields.io/badge/Scikit_Learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white"></div>

---

## Context

Credit card companies must be able to recognize fraudulent credit card transactions to prevent customers from being charged for unauthorized purchases. This project focuses on identifying such fraudulent transactions using data analytics and machine learning.

## Dataset Overview

The dataset contains credit card transactions made by European cardholders in September 2013. It includes 284,807 transactions, with 492 instances of fraud, making it highly imbalanced. The features include PCA-transformed numerical variables, 'Time,' and 'Amount.'

### Inspiration

The primary goal is to identify fraudulent credit card transactions. Given the class imbalance, accuracy will be measured using the Area Under the Precision-Recall Curve (AUPRC).

## Project Structure

- **[Credit_Card_Fraud_Detection.ipynb](Credit_Card_Fraud_Detection.ipynb):** Jupyter Notebook containing the entire project code.
- **[creditcard.csv](creditcard.csv):** Dataset file.

## Exploratory Data Analysis (EDA)

The project begins with exploratory data analysis to understand the dataset and its distribution.

### Key EDA Visualizations

- Class distribution bar plot, pie chart, and donut chart.
- Histogram of transaction amount.
- Scatter plot of time vs. amount for fraud and normal transactions.

## Data Preprocessing

The dataset is analyzed and preprocessed, checking for missing values and exploring the distribution of features.

## Model Prediction

The following outlier detection algorithms are applied:

1. **Isolation Forest Algorithm:** Detects anomalies based on the isolation of observations using decision trees.

2. **Local Outlier Factor (LOF) Algorithm:** Computes the local density deviation of a given data point with respect to its neighbors.

3. **Support Vector Machine (SVM):** Uses a one-class SVM for anomaly detection.

### Model Evaluation

The models are evaluated based on accuracy, precision, recall, and classification reports. Isolation Forest outperforms the other algorithms in detecting fraud cases.

## Results

- Isolation Forest detected 73 errors, LOF detected 97 errors, and SVM detected 8516 errors.
- Isolation Forest achieved an accuracy of 99.74%, a precision of 30%, and a recall of 27% for fraud detection.

## Feature Analysis

Boxplots illustrate the reduction of outliers in key features (V14, V12, V10) after applying the outlier detection algorithms.

## Contributors

- [Your Name](Your GitHub Profile)
- [Collaborator 1](Collaborator 1 GitHub Profile)
- [Collaborator 2](Collaborator 2 GitHub Profile)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Mention any external libraries, datasets, or individuals whose work contributed to the project.


