# Telco Customer Churn Prediction 📊🔮

An end-to-end Machine Learning project designed to identify customers who are at a high risk of churning from a telecommunications service provider. By analyzing historical client demographics, signed contracts, account parameters, and subscription behavior, the repository builds and trains predictive models to guide business retention strategies.

---

## 🚀 Key Features Built into the Pipeline
* **Complete Preprocessing Lifecycle**: Automatic drop of non-predictive attributes (`customerID`), robust conversion of financial boundaries (`TotalCharges` forced to numeric format), and explicit median/mode missing value imputation strategies.
* **Categorical Feature Encoding**: Full deployment of Scikit-Learn `LabelEncoder` pipelines across object columns to format strings seamlessly into numeric data representations ready for model utilization.
* **Dual-Model Classifiers Evaluation**: Parallel execution, tuning, and rigorous performance comparisons of both **Logistic Regression** and **Random Forest Classifiers**.
* **Serialized Pipelines**: Comprehensive preservation of trained tracking frameworks (`label_encoders.pkl`) and the absolute best production-ready iteration (`churn_model.pkl`).
* **Automated Result Outputs**: Real-time logging of prediction outputs mapped directly alongside actual labels in an exported validation sheet (`prediction_results.csv`).

---

## 📁 Repository Structure
```text
├── customer_churn.csv        # Primary customer database used for training/testing
├── customer_churn_notebook.ipynb # Comprehensive development notebook containing standard cells
├── requirements.txt          # Python dependency libraries list
├── label_encoders.pkl        # Serialized LabelEncoder mapping configurations 
├── churn_model.pkl           # Exported production-grade classification model
└── prediction_results.csv    # Evaluated test splits including Actual vs Inferred vectors
