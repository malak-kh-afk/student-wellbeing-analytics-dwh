
# ✅ **Student Burnout Data Warehouse & Analytics Project**

## 🎓 **1. Overview**

This project aims to analyze academic burnout and stress among university students using a fully structured **Data Warehouse**, advanced **data preprocessing**, and **interactive analytics dashboards**.

The study is based on a **simulated dataset of 5,000 records** representing student wellbeing variables across **four semesters**.

The project includes:

* Data collection & cleaning (Python: Pandas & NumPy)
* Data transformation & encoding
* Star-schema Data Warehouse design
* SQL storage model
* KPI dashboard & visual analytics (Power BI)
* Data mining predictions: Logistic Regression, Random Forest, K-Means

---

## 🚨 **2. Problem Statement**

**To what extent do academic, socio-demographic, and behavioral factors contribute to increased stress, anxiety, and burnout among students?**
And how can a data warehouse help centralize and analyze these indicators to reveal risk patterns and guide preventive measures?

---

## 🧰 **3. Tools & Technologies**

| Category           | Tools                                                     |
| ------------------ | --------------------------------------------------------- |
| Data Cleaning      | Python, Pandas, NumPy                                     |
| Storage            | SQL, Star Schema Modeling                                 |
| BI & Visualization | Power BI                                                  |
| Data Mining        | Scikit-learn, Logistic Regression, Random Forest, K-Means |
| Data Parsing       | One-hot encoding, StandardScaler                          |

---

## 📦 **4. Dataset Description**

The dataset includes **demographic**, **academic**, **lifestyle**, and **psychological** indicators:

### 🔹 **Demographics**

* student_id
* age
* gender (M, F)
* city_type (Urban, Rural)
* faculty (Sciences, Engineering, Medicine, Law, etc.)
* level (Bac, L1, L2, L3, Master)

### 🔹 **Lifestyle**

* sleep_hours
* study_hours
* screen_hours_academic
* screen_hours_leisure
* physical_activity_hours

### 🔹 **Pressure Indicators**

* academic_pressure (1–5)
* financial_stress (1–5)
* social_support (1–5)
* exam_period (0/1)

### 🔹 **Psychological Scores**

* stress_level
* anxiety_score
* depressive_symptoms
* burnout_risk (Low, Medium, High)

---

## 🧹 **5. Data Cleaning & Transformation**

Performed using Python:

* Duplicate removal
* Missing value handling (median/mode)
* Optional outlier detection (z-score)
* One-hot encoding for categorical variables
* StandardScaler normalization for numerics
* Export as `student_wellbeing_clean_for_model.csv`

---

## 🏗️ **6. Data Warehouse – Star Schema**

The DWH model includes:

### ⭐ **Fact Table**

`fact_student_wellbeing`

* stress_level
* anxiety_score
* depressive_symptoms
* burnout_risk
* FK_student
* FK_time
* FK_academic
* FK_wellbeing

### 📘 **Dimensions**

* **dim_student** (gender, age, level, faculty…)
* **dim_time** (semester, exam_period…)
* **dim_academic** (gpa, pressure indicators…)
* **dim_wellbeing** (screen_hours, sleep_hours, physical activity…)

This structure centralizes all student wellbeing metrics for analysis.

---

## 📊 **7. BI Dashboard Insights (Power BI)**

Key findings:

* Burnout risk is **extremely high** across semesters, especially 2024S1–2024S2.
* Anxiety levels are **higher than stress levels**, indicating internal pressure.
* Faculties most affected: **Sciences, Engineering, Medicine**.
* Stress peaks during **exam periods**.
* Lifestyle variables (sleep hours, study hours) influence wellbeing.

---

## 🤖 **8. Data Mining & Prediction**

Models used:

### ✔️ Logistic Regression

Burnout probability: **≈ 99%**

### ✔️ Random Forest

Accuracy: **≈ 88%**
Most important feature: **anxiety_score (0.43)**

### ✔️ K-Means

Clear cluster:
**High Stress + High Anxiety** → students at maximum risk.

---

## 🧭 **9. Recommendations**

Based on insights:

* Stress-management workshops
* Psychological support during exam periods
* Monitor students with high anxiety scores
* Reduce academic overload in high-pressure faculties
* Create an early-warning detection system

---

## 📁 **10. Project Structure**

```
/data
    student_wellbeing_raw.csv
    student_wellbeing_clean_for_model.csv

/notebooks
    preprocessing.ipynb
    modeling.ipynb

/sql
    star_schema.sql

/dashboard
    burnout_dashboard.pbix

/docs
    presentation.pdf
    README.md
```

---

## 🚀 **11. How to Run**

### 1. Clone the repository

```
git clone https://github.com/<your-username>/burnout-datawarehouse.git
```

### 2. Install dependencies

```
pip install pandas numpy scikit-learn
```

### 3. Run preprocessing

```
python preprocessing.py
```

### 4. Import SQL star schema

Load tables into your SQL server.

### 5. Open the Power BI dashboard

Load `burnout_dashboard.pbix`.

---

## 📌 **12. Deliverables**

* ✔️ Cleaned dataset
* ✔️ Star schema SQL model
* ✔️ KPIs & visual dashboard
* ✔️ Data mining predictions
* ✔️ Full PDF presentation

---

## 🎯 **13. Authors**

* **Malak Kharbech**
