# California Housing Price Prediction 🏠🤖

This repository contains my implementation and notes for the California Housing Prices project from the renowned book **"Hands-On Machine Learning with Scikit-Learn, Keras, and TensorFlow"** by Aurélien Géron. 

The goal of this project is to build a high-performance Machine Learning model to predict median housing prices in California districts using various demographic and geographic features.

---

## 🚀 Project Workflow & Progress

### 1. Data Ingestion & Setup
* Automated data downloading and extraction pipelines.
* Implemented robust data loading mechanisms using Pandas.
* Handled automated train/test splitting.

### 2. Stratified Sampling (Current Stage) 🎯
* Analyzed income distributions to identify potential data bias.
* Avoided pure random sampling limitations by leveraging **Stratified Sampling** via Scikit-Learn's `StratifiedShuffleSplit`.
* Created a temporary `income_cat` attribute to ensure the test set is thoroughly representative of the overall population, then cleanly dropped it to keep the dataset pristine.

### 3. Next Steps 🛠️
* Explored Data Analysis (EDA) and visualization (Scatter plots, correlations).
* Feature Engineering & Attribute Combinations.
* Data Cleaning (Handling missing values, Categorical Encoding, Feature Scaling).
* Training and fine-tuning Machine Learning Models.

---

## 🛠️ Tech Stack & Tools
* **Language:** Python 🐍
* **Libraries:** Pandas, NumPy, Scikit-Learn, Matplotlib
* **Environment:** Jupyter Notebook, Virtual Environments (`venv`)
