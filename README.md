
# California Housing Price Prediction 🏡📊

This repository contains my implementation and notes for the California Housing Prices project from the renowned book **"Hands-On Machine Learning with Scikit-Learn, Keras, and TensorFlow"** by Aurélien Géron. 

The goal of this project is to build a high-performance Machine Learning model to predict median housing prices in California districts using various demographic and geographic features.

---

## 🚀 Project Workflow & Progress

### 1. Data Ingestion & Setup
* Automated data downloading and extraction pipelines.
* Implemented robust data loading mechanisms using Pandas.

### 2. Stratified Sampling 🎯
* Analyzed income distributions to avoid pure random sampling bias.
* Leveraged Scikit-Learn's `StratifiedShuffleSplit` based on income categories to ensure the test set thoroughly represents the overall population.

### 3. Data Exploration & Feature Engineering 🔍
* Investigated data correlations using the Pearson correlation coefficient matrix.
* Separated predictors from target labels (`housing_labels`) to prepare for ML pipelines.

### 4. Data Preprocessing & Automation Pipelines 🛠️
* **Data Cleaning:** Handled missing values dynamically across all numerical attributes using Scikit-Learn's `SimpleImputer` (median strategy).
* **Categorical Encoding:** Processed the text attribute `ocean_proximity` into binary vectors using `OneHotEncoder`.
* **Custom Transformers:** Created a custom standalone class `CombinedAttributesAdder` (inheriting from `BaseEstimator` and `TransformerMixin`) to automate feature scaling and mathematical feature combinations cleanly.
* **Feature Scaling:** Applied `StandardScaler` to bring all numerical features to a uniform variance, minimizing outlier impact.
* **Full Preprocessing Pipeline (Current Stage):** Unified both numerical pipelines and categorical encoders into a single, robust `ColumnTransformer` (`full_pipeline`) that outputs an optimized dense NumPy array ready for training.

### 5. Next Steps (Current Stage) 🔀
* Select and train baseline Machine Learning Models (Linear Regression, Decision Tree, Random Forest).
* Evaluate models using Cross-Validation and Root Mean Squared Error (RMSE).
* Fine-tune hyperparameters via Grid Search / Randomized Search.

---

## 🛠️ Tech Stack & Tools
* **Language:** Python 🐍
* **Libraries:** Pandas, NumPy, Scikit-Learn, Matplotlib
* **Environment:** Jupyter Notebook, Git

