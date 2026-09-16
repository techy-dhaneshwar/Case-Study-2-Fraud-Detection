# Case Study 2: Credit Card Fraud Detection

## What is this project about?
When people use credit cards, a tiny fraction of transactions are fraudulent. Because fraud happens so rarely, datasets are hugely imbalanced—meaning almost all transactions are normal and only a few are fraud. This project uses machine learning to catch those rare fraudulent transactions accurately.

---

## What data are we using?
* **`amount`**: How much money was spent in the transaction.
* **`distance_from_home`**: How far away the transaction happened from the cardholder's home.
* **`is_online`**: Whether the purchase was made online or in a physical store (1 = Online, 0 = In-store).
* **`is_fraud`**: What we are trying to predict (1 = Fraudulent, 0 = Legitimate).

---

## Steps We Followed
1. **Created a Dataset**: Simulated 1,000 credit card transactions where only 5% were fraudulent.
2. **Balanced the Data (SMOTE)**: Since fraud is so rare, we used a technique called **SMOTE** to create synthetic examples of fraud so the model has enough data to learn from.
3. **Scaled the Numbers**: Adjusted the values so large numbers (like transaction amount) don't overpower smaller numbers.
4. **Trained Two Models**:
   * **Baseline Model**: Support Vector Machine (SVM)
   * **Main Model**: XGBoost Classifier
5. **Compared Results**: Checked which model did a better job catching fraud using ROC-AUC scores and saw which features mattered most for detecting fraud.
