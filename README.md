# Heart Disease Metrics Evaluation 🫀

This project implements a supervised classification model to predict the presence of heart disease, evaluating performance through key metrics, ROC/PR curves, and cost–benefit analysis.

## 🎯 Objective
Maximize **recall (sensitivity)** to minimize false negatives — ensuring that patients with actual disease are not missed.

## 🧠 Models Evaluated
- Logistic Regression  
- Random Forest  
- XGBoost  
- Support Vector Machine (SVM) — *final selected model*

## 📊 Evaluation Metrics
- Accuracy  
- Precision  
- Recall (primary metric)  
- F1 Score  
- ROC AUC  

## ⚙️ Additional Analysis
- Confusion Matrix  
- ROC and Precision–Recall Curves  
- Threshold tuning  
- Cost–Benefit analysis with simulated clinical costs  

## 🧩 Key Results (SVM Model at Threshold 0.40)
| Metric | Value |
|--------|--------|
| Precision | 0.878 |
| Recall | 0.961 |
| F1 Score | 0.917 |
| ROC AUC | 0.949 |
| Review Rate | 0.604 (≈60%) |

## 🧾 Interpretation
High recall ensures nearly all true cases are flagged, while acceptable precision limits excessive false alarms. The model operates in a clinically safe regime with a balanced trade-off between risk and workload.

## 🧮 Cost–Benefit Summary
At the chosen threshold (0.40):
- False Negatives (FN) cost = \$7,500  
- False Positives (FP) cost = \$1,000  
- Expected total cost per patient = \$236.96  
This configuration balances clinical safety and operational feasibility.

## 📦 Requirements
```bash
pip install numpy pandas matplotlib seaborn scikit-learn xgboost
