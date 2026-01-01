# Fraud-detection-using-transaction-text-analysis-
# Fraud Detection Using XGBoost

## 📌 Overview
This project focuses on detecting fraudulent credit card transactions using machine learning techniques.  
The dataset represents real-world credit card transactions made by European cardholders over two days, with a highly imbalanced class distribution where fraud cases account for only **0.172%** of all transactions.

Due to this extreme imbalance, the project emphasizes **appropriate evaluation metrics** and **robust modeling techniques** rather than relying on misleading accuracy scores.

---

## 🎯 Objective
- Build an effective fraud detection model capable of identifying rare fraudulent transactions.
- Handle severe class imbalance using suitable evaluation strategies.
- Apply gradient boosting (XGBoost) to capture complex, non-linear patterns in transaction data.

---

## 📊 Dataset Description
- **Total Transactions:** 284,807  
- **Fraudulent Transactions:** 492  
- **Fraud Ratio:** 0.172%

### Features
- `V1` to `V28`: Numerical features obtained using **PCA transformation** (anonymized for confidentiality).
- `Time`: Seconds elapsed between the transaction and the first transaction in the dataset.
- `Amount`: Transaction amount (useful for cost-sensitive learning).
- `Class`: Target variable  
  - `1` → Fraud  
  - `0` → Legitimate transaction

⚠️ Original feature descriptions are unavailable due to privacy and confidentiality constraints.

---

## 🧠 Approach
1. **Data Exploration & Analysis**
   - Class distribution analysis
   - Transaction amount and time behavior

2. **Data Preprocessing**
   - Feature scaling
   - Train-test split with stratification
   - Handling extreme class imbalance

3. **Modeling**
   - Implemented **XGBoost Classifier**
   - Tuned hyperparameters for imbalanced classification

4. **Evaluation Strategy**
   - Accuracy and confusion matrix are avoided due to class imbalance
   - Primary metric used:
     - **Area Under the Precision-Recall Curve (AUPRC)**
   - Precision, Recall, and F1-score analyzed for fraud class

---

## 📈 Results & Insights
- The XGBoost model demonstrated strong capability in identifying rare fraud cases.
- Precision-Recall trade-offs were carefully analyzed to minimize false negatives.
- AUPRC provided a more reliable performance indicator compared to accuracy.

---

## 🛠 Tech Stack
- **Programming Language:** Python  
- **Libraries:**  
  - Pandas, NumPy  
  - Scikit-learn  
  - XGBoost  
  - Matplotlib / Seaborn  
- **Environment:** Jupyter Notebook  

---

## ▶️ How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/USERNAME/fraud-detection-xgboost.git
