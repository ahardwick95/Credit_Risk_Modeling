# 🏦 Credit Risk Modeling with LendingClub Data

🚀 A full-stack machine learning project designed to predict loan default risk using real-world LendingClub data. This project simulates how data scientists in fintech build, explain, and deploy models for business-critical decisions — from SQL cleaning to deep learning to executive reporting.

---

## 📊 Project Overview

This project builds an end-to-end pipeline to:

- Clean and explore raw loan application data using **SQL** and **Pandas**
- Perform **EDA** and **feature engineering** to uncover key risk drivers
- Train and compare multiple models:
  - Logistic Regression (baseline)
  - XGBoost
  - LightGBM
  - PyTorch MLP
- **Deploy** the final model via:
  - 🚀 **FastAPI** for backend API
  - 🎯 **Streamlit** for interactive front-end UI
- 📈 **Power BI Dashboard** to simulate stakeholder reporting
- Analyze both **accepted** and **rejected** loan applications

---

## 🧠 Problem Statement

**Can we predict whether a loan applicant is likely to default, using only information available at the time of loan approval?**

✅ This problem is critical for lenders seeking to reduce risk exposure while maximizing loan volume.

---

## 🏗️ Architecture Workflow

```text
[Raw LendingClub CSVs]
        ↓
[SQL → Cleaning + Filtering]
        ↓
[Pandas/Seaborn → Deep EDA + Feature Engineering]
        ↓
[Modeling → Logistic | XGBoost | LightGBM | PyTorch]
        ↓
┌────────────┬────────────┐
│ FastAPI API│ Power BI   │
│ (Backend)  │ Dashboard  │
└────────────┴────────────┘
        ↓
[User Interface → Risk Score + Reports]
