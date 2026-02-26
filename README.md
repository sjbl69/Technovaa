# Employee Turnover Prediction

## Project Objective

The goal of this project is to predict employee turnover using machine learning techniques and provide interpretable insights for business decision-making.

The project includes:
- Exploratory Data Analysis (EDA)
- Data preprocessing
- Baseline and advanced models
- Handling class imbalance
- Model comparison
- SHAP interpretability

---

## 📁 Dataset

The dataset is composed of three sources:
- HR information (SIRH)
- Performance evaluation data
- Employee survey data

After merging and cleaning, the final dataset contains:
- 1470 employees
- 34 features
- Target variable: `has_left`

The dataset is imbalanced:
- ~84% stayed
- ~16% left

---

## Exploratory Data Analysis

Key steps:
- Data cleaning and column normalization
- Missing value verification
- Descriptive statistics
- Correlation analysis
- Detection of redundant features
- Feature engineering

Main observations:
- Employee satisfaction and tenure are strongly related to turnover.
- Distance from home appears influential.
- No missing values detected.

---

##  Modeling

Three models were evaluated:

| Model | Accuracy | Precision | Recall | F1-score |
|-------|----------|----------|--------|----------|
| Dummy | Baseline | Baseline | 0 | 0 |
| Logistic Regression | Balanced | Good interpretability | Improved recall | Stable |
| Random Forest + SMOTE | Best overall | Best recall | Best F1 | Selected model |

### 🔹 Why Random Forest?

- Handles non-linear relationships
- Works well with mixed feature types
- Performs better on imbalanced data with SMOTE
- Provides feature importance

---

##  Model Evaluation

Evaluation metrics used:
- Accuracy
- Precision
- Recall
- F1-score
- Confusion matrix
- Stratified cross-validation

Recall was prioritized due to business importance:
Detecting employees at risk of leaving is more critical than overall accuracy.

---

##  Model Interpretability (SHAP)

SHAP was used to:
- Identify global feature importance
- Explain individual employee predictions

Key drivers of turnover:
- Satisfaction level
- Years in company
- Distance from home
- Work-life balance

---

##  Business Impact

This model can help HR teams:
- Identify at-risk employees early
- Improve retention strategies
- Optimize engagement policies
- Reduce turnover costs

---

## 🛠 Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Imbalanced-learn (SMOTE)
- Matplotlib / Seaborn
- SHAP

---

##  How to Run

```bash
pip install -r requirements.txt
