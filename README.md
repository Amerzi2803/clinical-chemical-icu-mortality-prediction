# clinical-chemical-icu-mortality-prediction
Predict ICU mortality using clinical and chemical lab data with XGBoost and ML techniques for healthcare insights.

# Clinical & Chemical ICU Mortality Prediction

**Author:** Aamerzish Alvi  
**Domain:** Healthcare AI or Clinical & Chemical Lab Data  
**Frameworks & Tools:** Python, Pandas, NumPy, Scikit-learn, XGBoost, Matplotlib, Seaborn, Jupyter Notebook  

---

##  Project Overview
This project aims to predict **ICU mortality** using a blend of **clinical and chemical lab test data**.  
We leverage machine learning techniques to help hospitals identify high-risk patients and make data-driven clinical decisions.

**Dataset Highlights:**  
- 20,000 patient records  
- Clinical features: age, weight, gender, vital lab markers  
- Chemical features: glucose, creatinine, hemoglobin, WBC, platelets, sodium, potassium, lactate  
- Target: `icu_mortality` (binary: 0 = survived, 1 = deceased)  

---

##  Problem Statement
ICU mortality prediction is a critical task in healthcare analytics.  
By integrating chemical lab results with clinical patient data, hospitals can prioritize care for high-risk patients and optimize resource allocation.

---

##  Key Steps in Project
1. **Data Exploration & Preprocessing**
   - Handled missing values
   - Numeric scaling & one-hot encoding for categorical features
2. **Train-Test Split**
   - Ensured balanced target distribution
3. **Modeling**
   - Baseline: Logistic Regression
   - Advanced: XGBoost (Gradient Boosting)
4. **Evaluation**
   - Confusion Matrix, Classification Report, ROC-AUC
   - Tuned hyperparameters using GridSearchCV
5. **Insights**
   - ROC-AUC achieved: ~0.69
   - Recall for ICU mortality: ~0.75
   - Feature importance analyzed

---

##  Results (XGBoost)

**Confusion Matrix:**

[[ 881 822]
[ 565 1732]]


**Classification Report:**

| Class | Precision | Recall | F1-Score | Support |
|-------|-----------|--------|----------|---------|
| 0     | 0.61      | 0.52   | 0.56     | 1703    |
| 1     | 0.68      | 0.75   | 0.71     | 2297    |

**Accuracy:** 0.65  
**Macro Avg F1-Score:** 0.64  
**Weighted Avg F1-Score:** 0.65  
**ROC-AUC:** 0.6898
