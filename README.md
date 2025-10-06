# Titanic Feature Engineering

This repository contains a **feature engineering pipeline** for the classic [Titanic dataset](tested.csv). The notebook demonstrates how to transform raw passenger records into a **machine-learning-ready dataset** through data cleaning, enrichment, and encoding.

---

## **Project Overview**

The Titanic dataset is one of the most popular benchmarks for data science. The challenge is to predict passenger survival based on features such as age, gender, ticket class, and family connections.

This notebook focuses on **feature engineering**, a critical step that often determines model performance.

---

## **Steps in the Notebook**

### **1.  Data Loading & Exploration**

* Import Titanic dataset with Pandas.
* Inspect data types, missing values, and survival distribution.
* Quick exploratory statistics and visualizations.

### **2.  Data Cleaning**

* Handle missing values for `Age`, `Cabin`, and `Embarked`.
* Standardize formats and drop irrelevant identifiers.

### **3.  Feature Engineering**

* **Title Extraction** from names (Mr, Miss, Mrs, etc.).
* **Family Size** (`SibSp` + `Parch` + 1).
* **IsAlone** flag for passengers traveling without family.
* **Cabin Deck** extracted from cabin numbers.
* **Age Groups** (Child, Teen, Adult, Senior).
* **Fare Bins** to reduce skewness.

### **4.  Encoding & Transformation**

* Convert categorical variables (Sex, Embarked, Title, Cabin Deck) into numerical form via Label or One-Hot Encoding.
* Normalize continuous features where useful.

### **5.  Final Dataset Preparation**

* Drop unnecessary columns (e.g., PassengerId, Ticket, Name).
* Return a clean DataFrame ready for training ML models.

---

## **Key Outcomes**

* A **reproducible pipeline** for feature engineering.
* Demonstrates techniques like **categorical encoding, binning, imputation, and feature extraction**.
* Produces a dataset optimized for **classification models** (Logistic Regression, Random Forest, Gradient Boosting, etc.).

---

## **Next Steps**

* Train baseline models with engineered features.
* Compare model performance with and without feature engineering.
* Extend to ensemble methods (XGBoost, LightGBM).

