# AutoLend-ML-Classifier
A predictive modeling project aimed at automating bank loan approval decisions. This repository compares Logistic Regression, K-Nearest Neighbors (KNN), and Support Vector Machines (SVM), featuring rigorous hyperparameter tuning and a critical analysis of algorithmic fairness and ethical lending practices.

# Automated Loan Approval Decision System

## 🏦 Project Overview
This project simulates the role of a Data Scientist at a regional bank. The objective is to automate the loan approval process by building and optimizing classification models. The project transitions from manual underwriting to an algorithmic approach, focusing on efficiency, accuracy, and ethical transparency.

## 📊 Dataset: `loan_approval.csv`
The model uses historical applicant data to predict the `approved` status. Key features include:
- **Financials**: Debt, Income, Years Employed, Credit Score.
- **Demographics**: Age, Gender, Ethnicity (used for ethical auditing).
- **History**: Prior Default, Employment status.

## 🤖 Modeling & Optimization
I implemented and compared three distinct classification algorithms:
1. **Logistic Regression**: Tuning the regularization strength (`C`) and solvers.
2. **K-Nearest Neighbors (KNN)**: Optimizing for the number of neighbors and distance weighting.
3. **Support Vector Machine (SVM)**: Tuning kernels (RBF vs. Sigmoid) and cost parameters.

### Performance Evaluation
Each model was evaluated using:
- **Grid Search / Hyperparameter Tuning** with visual scoring charts.
- **Confusion Matrices** & **Classification Reports** (Precision, Recall, F1-Score).
- **ROC/AUC Curves** to measure the trade-off between sensitivity and specificity.
- **K-Fold Cross-Validation** to ensure the models generalize well to new applicants.

## ⚖️ Ethical Considerations
A core component of this project is the discussion on **Fair Lending**. Since the dataset contains sensitive attributes (Age, Gender, Ethnicity), the project includes a critical reflection on:
- Algorithmic bias and historical discrimination.
- The use of "proxies" (like Zip Codes) in lending.
- The "Right to Explanation" for rejected applicants under financial regulations.

## 🚀 Installation & Usage
1. Clone the repository.
2. Install dependencies: `pandas`, `sklearn`, `seaborn`, `matplotlib`.
3. Open `AutoLend-ML-Classifier.ipynb` in Jupyter Notebook or Google Colab to view the analysis.
