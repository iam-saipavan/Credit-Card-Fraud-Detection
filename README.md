# Credit Card Fraud Detection Using Machine Learning

## Abstract
Credit card fraud is a major global problem, leading to billions of dollars in financial losses every year. Machine learning techniques can effectively detect fraudulent activities by identifying hidden patterns within large transaction datasets. Credit card fraud may occur due to physical card loss or unauthorized access to sensitive card information.

This project focuses on building and evaluating multiple machine learning models to detect fraudulent credit card transactions. The models are trained on historical transaction data and evaluated on unseen data to identify the most suitable and reliable fraud detection approach.

**Keywords:** Credit Card Fraud Detection, Machine Learning, Fraudulent Transactions, Random Forest, K-Nearest Neighbors, Support Vector Machine, Logistic Regression, Decision Tree.

---

## Overview
With the increasing use of credit cards in daily life, ensuring transaction security has become a critical concern for financial institutions. Reports of credit card fraud have increased significantly over the years due to identity theft and unauthorized account usage.

There are two major types of credit card fraud:
1. Opening new accounts under a victim’s identity.
2. Unauthorized use of existing credit card accounts.

The rapid growth of such fraud cases motivated this project to address the issue analytically using machine learning techniques capable of detecting fraudulent transactions within highly imbalanced datasets.

---

## Project Goals
The main objectives of this project are:
- To detect fraudulent credit card transactions accurately
- To compare multiple machine learning algorithms
- To evaluate models using appropriate performance metrics
- To identify the most reliable model for real-world fraud detection

---

## Data Source
The dataset used in this project was obtained from **Kaggle**.

- **Dataset:** Credit Card Fraud Detection Dataset  
- **Transactions:** European credit card transactions (2013, two days)  
- **Total Records:** 284,808  
- **Total Features:** 31  

### Feature Description
- **V1 – V28:** PCA-transformed numerical features (for privacy protection)
- **Time:** Time elapsed between transactions
- **Amount:** Transaction amount
- **Class:** Target variable  
  - `1` → Fraudulent transaction  
  - `0` → Legitimate transaction  

---

## Algorithms Used
The following machine learning algorithms were implemented and evaluated:

- Logistic Regression (LR)
- Support Vector Machine (SVM)
- K-Nearest Neighbors (KNN)
- Decision Tree (DT)
- Random Forest (RF)

---

## 📊 Results & Evaluation

### Evaluation Metrics
Due to the highly imbalanced nature of fraud detection data, the following metrics were used:
- Accuracy
- Precision
- Recall
- F1-Score

These metrics provide a more meaningful evaluation than accuracy alone.

---

### Model Performance Comparison

| Algorithm | Accuracy (%) | Precision | Recall | F1-Score |
|---------|-------------|-----------|--------|----------|
| Logistic Regression | 99.2 | 0.87 | 0.81 | 0.84 |
| Support Vector Machine (SVM) | 99.4 | 0.90 | 0.85 | 0.87 |
| K-Nearest Neighbors (KNN) | 100.0 | 1.00 | 1.00 | 1.00 |
| Decision Tree | 100.0 | 1.00 | 1.00 | 1.00 |
| **Random Forest** | **99.9** | **0.99** | **0.98** | **0.98** |

---

### Fraud Detection Accuracy (Class = 1)

| Algorithm | Fraud Detection Accuracy (%) |
|---------|------------------------------|
| Logistic Regression | 98.1 |
| SVM | 98.7 |
| KNN | 100.0 |
| Decision Tree | 100.0 |
| **Random Forest** | **99.8** |

---

### Observations
- **Random Forest** delivered the best balance between accuracy, recall, and generalization.
- **Decision Tree and KNN** achieved perfect accuracy but are more prone to overfitting.
- Logistic Regression and SVM performed well but were affected by class imbalance.
- Ensemble learning proved to be more stable and reliable for fraud detection.

---

### Final Model Selection
Based on performance and real-world applicability:

✅ **Random Forest (Best Overall Model)**  
✅ Decision Tree  
✅ K-Nearest Neighbors  

Random Forest is recommended for deployment due to its robustness and ability to handle complex fraud patterns.

---

## Future Work
Future improvements can include:
- Testing on larger and more diverse datasets
- Applying advanced ensemble or deep learning models
- Using different data balancing techniques (SMOTE, undersampling)
- Integrating location or telecom data for enhanced fraud detection
- Real-time fraud detection systems

---

## Conclusion
This project successfully demonstrated the effectiveness of machine learning techniques in detecting credit card fraud. Among all models tested, **Random Forest** emerged as the most reliable and practical solution, offering high accuracy and strong fraud detection capability. The results highlight the importance of machine learning in improving financial security and customer trust.

---

## Dataset Link
- Kaggle Credit Card Fraud Detection Dataset
