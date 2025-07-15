# 🧹 Cleaned Datasets (SQL-Preprocessed)

This folder contains the intermediate, **SQL-cleaned datasets** used for early-stage analysis and modeling in the credit risk modeling project. These files were cleaned and exported after performing initial preprocessing using SQL (SQLite).

Further transformations, visualizations, and feature engineering will occur in Python/Pandas notebooks during the EDA and modeling phases.

---

## 📁 Files

### `accepted_loans_cleaned.csv`
> Accepted loan applications from LendingClub (2007–2018), cleaned using SQL for downstream supervised machine learning.

- ✅ Removed rows with excessive nulls or inconsistent records
- ✅ Selected relevant columns for analysis
- ⚠️ Further preprocessing (e.g., one-hot encoding, scaling, imputing) still pending in Pandas

---

### `rejected_loans_cleaned.csv`
> Loan applications that were rejected by LendingClub (2007–2018). No loan was issued, so these records have no outcome labels.

- ✅ Cleaned with SQL to remove malformed entries and irrelevant columns
- ✅ Retains useful features for exploratory analysis
- ❌ Not used for modeling (no target variable available)

---

## 📝 Usage in Project

- `accepted_loans_cleaned.csv`:  
  → Input for EDA, feature engineering, and model training in Python notebooks.

- `rejected_loans_cleaned.csv`:  
  → Used in exploratory dashboards (e.g., Power BI) to compare approved vs denied applications.

---

## 📂 Source

These cleaned files are derived from the raw LendingClub datasets (not included in this repo):

- `accepted_2007_to_2018Q4.csv`
- `rejected_2007_to_2018.csv`

📥 Available on [Kaggle](https://www.kaggle.com/datasets/wordsforthewise/lending-club)

---

## 🔜 Next Steps

- Perform Pandas-based EDA and feature engineering in `/notebooks/02_eda_feature_eng.ipynb`
- Prepare final ML-ready datasets for training and model evaluation

