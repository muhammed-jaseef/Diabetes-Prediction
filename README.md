# 🩺 Diabetes Prediction Using Machine Learning

## 📘 Overview
This project focuses on predicting whether a person is diabetic or not based on various medical and personal attributes. The dataset is analyzed, preprocessed, and modeled using multiple machine learning algorithms to identify the best-performing model.

---

## 📂 Dataset
The dataset includes several health-related features such as:

- **Pregnancies**: Number of times pregnant  
- **Glucose**: Plasma glucose concentration  
- **BloodPressure**: Diastolic blood pressure (mm Hg)  
- **SkinThickness**: Triceps skinfold thickness (mm)  
- **Insulin**: 2-Hour serum insulin (mu U/ml)  
- **BMI**: Body mass index (weight in kg/(height in m)²)  
- **DiabetesPedigreeFunction**: Genetic influence of diabetes  
- **Age**: Age of the person (years)  
- **Outcome**: 1 = Diabetic, 0 = Non-diabetic  

---

## ⚙️ Project Workflow
1. **Data Preprocessing**
   - Handling missing values  
   - Feature scaling using `StandardScaler`  
   - Addressing class imbalance using **SMOTE**
   - Hyper parameter tuning using **GridSearchCV**

2. **Model Training**
   Models trained with different preprocessing setups:
   - Scaled only  
   - Scaled + SMOTE  
   - Scaled + SMOTE + Hyperparameter Tuning  

3. **Model Evaluation**
   Metrics used for evaluation:
   - Accuracy  
   - Precision  
   - Recall  
   - F1-Score  

---

## 📊 Model Performance Summary

| Model | Accuracy | Precision | Recall | F1-Score | Setup |
|--------|-----------|------------|----------|-----------|--------|
| **Random Forest** | 0.76 | 0.75 | 0.76 | 0.75 | Scaled only |
| **Logistic Regression** | 0.76 | 0.75 | 0.76 | 0.75 | Scaled only |
| Logistic Regression | 0.75 | 0.75 | 0.75 | 0.75 | Scaled + SMOTE + Hyperparam |
| **XGBoost** | 0.75 | 0.74 | 0.75 | 0.74 | Scaled only |
| Random Forest | 0.73 | 0.73 | 0.73 | 0.73 | Scaled + SMOTE + Hyperparam |
| SVM | 0.73 | 0.72 | 0.73 | 0.71 | Scaled only |
| XGBoost | 0.70 | 0.71 | 0.70 | 0.70 | Scaled + SMOTE + Hyperparam |
| SVM | 0.68 | 0.67 | 0.68 | 0.67 | Scaled + SMOTE + Hyperparam |
| Logistic Regression | 0.75 | 0.63 | 0.67 | 0.65 | Scaled + SMOTE |
| Random Forest | 0.75 | 0.65 | 0.61 | 0.63 | Scaled + SMOTE |
| XGBoost | 0.72 | 0.60 | 0.63 | 0.61 | Scaled + SMOTE |
| SVM | 0.71 | 0.59 | 0.59 | 0.59 | Scaled + SMOTE |

---

## 🏆 Best Performing Models
- **Random Forest (Scaled only)** and **Logistic Regression (Scaled only)** both achieved:
  - **Accuracy:** 0.76  
  - **Precision:** ~0.75  
  - **F1-Score:** ~0.75  

These models performed best in balancing accuracy and stability.

---

## 🧠 Key Learnings
- Proper scaling significantly improves model performance.  
- SMOTE helps address imbalance but may introduce slight overfitting if not tuned carefully.  
- Logistic Regression and Random Forest were the most robust models for this dataset.  

---

## 📈 Tools & Libraries Used
- Python  
- Pandas, NumPy  
- Scikit-learn  
- XGBoost  
- Imbalanced-learn (SMOTE)
- Standard scalar
- GridSearchCV 
- Matplotlib, Seaborn  

---

## 🚀 Future Work
- Implement **feature selection** to identify the most influential variables  
- Experiment with deep learning models for comparison    
- Model deployment using **Flask** or **Streamlit**

---


