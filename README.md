# Geographic Classification of UK Electric Vehicle Infrastructure
**Module:** Data Mining (CSO7021)  
**Student ID:** 2418010  
**Artifact:** Replicable Machine Learning Pipeline & Analytics Repository  

---

## 📌 Project Overview
This repository contains a self-contained, reproducible Python machine learning pipeline designed to classify UK Local Authority areas into **Low, Medium, or High** public EV charging infrastructure density zones. 

By utilizing regional economic and demographic datasets from the **Office for National Statistics (ONS)** and the **Department for Transport (DfT)**, this project investigates whether regional characteristics—such as localized population scales and individual disposable income—can reliably indicate levels of public infrastructure investment.

## 🎯 The Strategic Challenge
The statutory transition from Internal Combustion Engine (ICE) vehicles to Electric Vehicles (EVs) introduces a significant geographic risk: the emergence of localized 'infrastructure deserts.' This project builds an empirical framework to help policymakers identify vulnerable areas and distribute development budgets efficiently, moving beyond the limitations of standard linear tracking.

---

## 🛠️ Pipeline Architecture (The "Big Four")
The methodology strictly complies with the module's Week 1–6 boundary constraints, evaluating and comparing the core classification paradigms:

1. **Support Vector Classifier (RBF Kernel):** Attempting non-linear boundary resolution to map structural distribution shifts.
2. **Decision Tree Classifier (`max_depth=4`):** Utilizing hierarchical, axis-aligned feature partitioning to mitigate majority-class collapse.
3. **k-Nearest Neighbours ($k=21$):** Implementing algorithmic hyperparameter tuning ($k=1$ to $21$) to identify optimal spatial neighborhoods.
4. **Gaussian Naive Bayes:** Assessing the impact of feature correlation and strict probabilistic independence on minority-class classification.

---

## 📁 Repository Structure
```text
├── 2418010_A3_Notebook.ipynb   # Unified Jupyter Notebook (Ingestion to Evaluation)
├── dft_ev_charging_raw.xlsx    # Department for Transport raw charging infrastructure dataset
├── ons_gdhi_per_head_raw.xlsx  # ONS raw Gross Disposable Household Income dataset
├── ons_population_raw.xlsx     # ONS raw regional population estimates dataset
├── README.md                   # Project documentation and replication guide
└── requirements.txt            # Python environment dependencies