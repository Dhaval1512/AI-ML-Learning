# Machine Learning Basics 🚀
This repository contains my learning journey in AI & Machine Learning — from foundational theory to hands-on projects.

## 📚 Topics Covered
- Classification vs Regression
- Train/Test Split (Manual vs Sklearn)
- Bias-Variance Tradeoff
- Decision Tree Classifier
- Large Language Models (LLMs) — Theory & Concepts
- Exploratory Data Analysis (EDA)
- Data Preprocessing & Feature Engineering

---

## 🗂️ Projects & Notes

### 🤖 Large Language Models — Concepts & Notes
> `notes/llm_basics.md` (or `notebooks/llm_basics.ipynb`)

A structured breakdown of how Large Language Models work under the hood.

**Topics Covered:**
- What are LLMs and how they work
- Pre-training — learning from massive text corpora, next token prediction
- Post-training — fine-tuning, instruction tuning, aligning to human intent
- RLHF (Reinforcement Learning from Human Feedback)
- Key concepts: tokenization, embeddings, attention mechanism

---

### 🏥 Medical Insurance Charges — EDA & Preprocessing
> `notebooks/insurance_data_preprocessing.ipynb`

End-to-end EDA and preprocessing on a medical insurance dataset to prepare it for ML modelling.

**Key EDA Findings:**
- Smoking status is the single strongest predictor of insurance charges (3–4x higher for smokers)
- BMI × Smoker interaction reveals a distinct high-cost cluster not visible in either variable alone
- Charges are heavily right-skewed (skewness ~1.7) — log transformation applied

**Preprocessing Pipeline:**
- Removed duplicate records
- Median imputation for missing `age` and `bmi` values
- Log1p transformation on `charges` to reduce skewness
- IQR-based outlier capping for `bmi` and `charges`
- Label Encoding for binary categoricals (`sex`, `smoker`)
- One-Hot Encoding for `region`
- Feature engineered `bmi_smoker` interaction term
- StandardScaler normalization
- Train/Test split — dataset ready for modelling

**Tech used:** Python, Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn

---

## 🛠️ Tech Stack
- Python
- NumPy
- Pandas
- Scikit-learn
- Matplotlib
- Seaborn

## 📂 Repository Structure
```
├── notebooks/          → Jupyter notebooks with experiments & projects
├── notes/              → Learning resources and references
```

## ✍️ Author
**Dhaval Patel**
