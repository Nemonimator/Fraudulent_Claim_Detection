# **Fraudulent Claim Detection 🚀**

## **🔹 Overview**
Fraudulent insurance claims lead to **significant financial losses** and **operational inefficiencies**. This project employs **machine learning models** to analyze historical claim data and improve fraud detection.

## **🔹 Data Processing**
- **Data Cleaning**: Removed **null values, illogical entries, and duplicate records**.
- **Feature Engineering**: Selected **key fraud indicators**, balanced classes using **RandomOversampling & SMOTE**, and applied **feature scaling**.
- **Exploratory Data Analysis (EDA)**: Investigated **fraud trends**, claim distributions, and feature correlations.

## **🔹 Models Tested**
### ✅ **Logistic Regression**
- **Accuracy**: `76.22%`
- **Recall (Fraud Detection)**: `2.94%` ❌ → Misses most fraud cases
- **Specificity**: `99.08%` ✅ → Correctly identifies legitimate claims
- **Precision**: `50%`
- **F1-Score**: `5.56%`

### ✅ **Random Forest**
- **Accuracy**: `69.23%`
- **Recall (Fraud Detection)**: `20.59%` ✅ → Detects more fraud
- **Specificity**: `44.95%`
- **Precision**: `29.17%`
- **F1-Score**: `24.14%`

## **🔹 Key Fraud Predictors**
📌 **Total Claim Amount** → Higher amounts are more suspicious  
📌 **Incident Severity (Total Loss & Minor Damage)** → Fraudulent claims cluster around extremes  
📌 **Policy Deductibles & Premiums** → Certain combinations indicate fraud risks  
📌 **Witness Count & Bodily Injuries** → No witnesses or exaggerated injuries may signal fraud  

## **🔹 Recommendations**
🚀 **Hybrid Model Approach** → Combine **Logistic Regression & Random Forest** for balanced fraud detection  
🚀 **Class Balancing Techniques** → Apply **SMOTE & Random Oversampling** to handle imbalance  
🚀 **Threshold Optimization** → Lower fraud detection threshold to **improve recall**  
🚀 **Advanced Models** → Experiment with **XGBoost & LightGBM** for **better fraud detection rates**  

## **🔹 Future Improvements**
🔹 Enhance feature selection to **reduce multicollinearity**  
🔹 Implement **real-time fraud scoring** for incoming claims  
🔹 Explore **fraud trend analysis over time**  
🔹 Improve model **generalization & reduce overfitting**  

## **🔹 Getting Started**
### **Installation**
```bash
git clone https://github.com/your-repo/fraud-detection.git
cd fraud-detection
pip install -r requirements.txt

python train_model.py

