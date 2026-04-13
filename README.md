# 🧠 Customer Churn Prediction (End-to-End Machine Learning Project)

## 📌 Overview

This project predicts whether a customer will churn (leave the service) using machine learning models.
It includes complete steps from data preprocessing to model deployment-ready pipeline.

---

## 🎯 Objective

To identify customers who are likely to churn and help businesses take proactive actions to retain them.

---

## ⚙️ Tech Stack

* **Programming:** Python
* **Libraries:** Pandas, NumPy
* **Visualization:** Matplotlib, Seaborn
* **Machine Learning:** Scikit-learn
* **Model Saving:** Joblib

---

## 📊 Project Workflow

### 1. Data Preprocessing

* Handled missing values
* Encoded categorical features
* Feature scaling using StandardScaler

### 2. Feature Engineering

* Created new features like:

  * Balance per product
  * Salary balance ratio
  * Age groups
  * Tenure buckets
* Added business-driven flags (e.g., high balance customers)

### 3. Model Building

Trained multiple models:

* Logistic Regression
* Random Forest
* Gradient Boosting
* AdaBoost
* Support Vector Machine (SVM)

---

### 4. Model Evaluation

* Used **Stratified K-Fold Cross Validation**
* Compared models using:

  * ROC-AUC Score
  * Accuracy
  * Precision
  * Recall
  * F1 Score

---

### 5. Best Model Selection

* Selected the best model based on **highest ROC-AUC score**
* Built a complete **pipeline (preprocessing + model)**

---

### 6. Model Saving

* Saved trained pipeline using:

```python
joblib.dump(best_pipeline, "best_churn_pipeline.pkl")
```

---

### 7. Prediction on New Data

* Created sample customer input
* Applied same feature engineering
* Predicted:

  * Churn (0/1)
  * Probability of churn

---

## 📁 Project Structure

```
CUSTOMER CHURN PREDICTION/
│
├── Analysis.ipynb
├── customer_data.csv
├── best_churn_pipeline.pkl
├── .gitignore
└── README.md
```

---

## 📈 Results

* Achieved strong performance using Gradient Boosting / Random Forest (based on run)
* Model effectively identifies high-risk customers

---

## 🔥 Key Highlights

* End-to-end ML pipeline
* Real-world feature engineering
* Model comparison with cross-validation
* Clean and reusable pipeline
* Production-ready approach

---

## 🚀 How to Run

```bash
# Clone repo
git clone https://github.com/your-username/customer-churn-prediction.git

# Install dependencies
pip install pandas numpy matplotlib seaborn scikit-learn joblib

# Run notebook
jupyter notebook
```

---

## 💼 Use Case

This project can be used by:

* Banks
* Telecom companies
* Subscription-based businesses

to reduce customer churn and improve retention.

---

## 📌 Future Improvements

* Hyperparameter tuning
* Deployment using Flask/Streamlit
* Real-time prediction API
* Dashboard visualization

---

## 👩‍💻 Author

**Shreya Raghav**

---

## ⭐ If you like this project

Give it a ⭐ on GitHub!
