# Bronny James Jr. Draft & Career Value Analysis

### *Statistical & Machine Learning Evaluation of NBA Draft Outcomes*

**Author:** Logan Laszewski  
**Timeline:** Personal Project (2025)

---

## Executive Summary

**Problem Motivation:** Bronny James Jr.’s selection at **55th overall** in the 2024 NBA Draft sparked criticism questioning whether his draft position reflected performance or name recognition. However, very little of this discussion referenced real historical data on late-second-round picks.

**Solution:** Using NBA draft and performance data (1989–2022), this project evaluates Bronny’s rookie season using transparent statistical and machine learning methods. The analysis includes:

* A **Random Forest regression model** predicting where Bronny would have been drafted based solely on rookie-year performance
* **k-Nearest Neighbors (KNN)** to identify historically similar rookie seasons
* **Principal Component Analysis (PCA)** to compare long-term performance among early vs. late picks
* Descriptive analysis of historical outcomes for players drafted **50–60**

**Impact:** Findings show Bronny’s rookie performance aligns more closely with a **mid-second-round pick (~35th overall)**. This challenges the “wasted pick” narrative and provides a data-driven, historically grounded evaluation.

---

## Project Motivation

* Public debate around Bronny focused on narrative, not data.
* Late-second-round outcomes are widely misunderstood — few players drafted 50–60 become long-term contributors.
* Rookie stats matter more for evaluating value than media takes.
* Statistical models offer a fair, bias-free way to contextualize his draft position.
* This project asks: **Was Bronny’s draft position actually unreasonable?**

---

## Methods & Techniques

### **Data**

* NBA player performance and draft data (1989–2022)
* Rookie-season statistics only (drafted players)
* Career averages across multiple performance categories
* Physical metrics: age, height, weight

### **Modeling**

* **Random Forest Regressor**
  * Predicts draft position using rookie-year stats
  * Tuned using GridSearchCV
  * RMSE ≈ 9.5 picks
  * Bronny’s inputs → estimated draft position **35**

* **k-Nearest Neighbors (KNN)**
  * Identifies the closest historical rookie-season matches
  * Bronny’s top comps:
    * Josh Selby
    * Jaylen Nowell
    * DeShawn Stevenson

* **Principal Component Analysis (PCA)**
  * Reduces 11 career-related metrics to 2 dimensions
  * Shows that late picks share substantial overlap with early picks

### **Descriptive Statistics**

* Weighted rookie-season averages for picks 50–60
* Median career length: **3 seasons**
* Development patterns from rookie year to year 5

---

## Findings

* Players drafted 50–60 rarely have large statistical impacts.
* Bronny’s rookie-year performance fits squarely within historical norms.
* Random Forest results suggest he outperformed his draft slot by ~20 picks.
* KNN comps include players who formed multi-year NBA careers.
* PCA demonstrates that draft position is not a strong predictor of long-term success.

---

## Skills Demonstrated

* Python data cleaning and preprocessing (Pandas, NumPy)
* Exploratory data analysis and visualization
* Machine learning modeling (Random Forest, KNN, PCA)
* Model evaluation (RMSE, hyperparameter tuning, CV splits)
* Dimensionality reduction and multivariate analysis
* Sports analytics and performance trend analysis
* Explaining technical insights to a nontechnical audience

---

## Data Source

NBA Performance & Draft Dataset (Kaggle): https://www.kaggle.com/datasets/sumitrodatta/nba-aba-baa-stats

---

## Files

* **Bronny_James_Jr_Analysis.ipynb** — full code, models, and visualizations  
* **all_seasons.csv** — cleaned dataset used for modeling
