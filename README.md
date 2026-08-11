# 🏠 House Price Prediction

A Machine Learning project that predicts house prices using the **Ames Housing Dataset**. The project follows an end-to-end machine learning workflow including **Exploratory Data Analysis (EDA), data cleaning, feature engineering, preprocessing, model building, and model evaluation**.

## 📌 Project Overview

House prices depend on several factors such as living area, overall quality, number of rooms, garage capacity, basement area, year built, and neighborhood.

This project uses machine learning regression techniques to learn the relationship between these features and house sale prices and generate price predictions.

## ✨ Features

* Exploratory Data Analysis (EDA)
* Missing-value handling
* Categorical feature encoding
* Feature engineering
* Data preprocessing
* Machine learning model training
* Model evaluation using regression metrics
* Cross-validation
* Actual vs Predicted visualization
* Residual analysis
* Model comparison

## 🗂️ Project Structure

```text
House-Prediction/
│
├── data/
│   └── train.csv
│   └── house_price_clean.csv
├── 01_eda.ipynb
├── 02_data_cleaning.ipynb
├── 03_model_building.ipynb
├── utils.py
├── requirements.txt
└── README.md
```

## 🔄 Machine Learning Workflow

```text
Raw Dataset
     ↓
Exploratory Data Analysis
     ↓
Data Cleaning
     ↓
Missing Value Treatment
     ↓
Feature Engineering
     ↓
Categorical Encoding
     ↓
Train/Test Preparation
     ↓
Model Training
     ↓
Model Evaluation
     ↓
House Price Prediction
```

## 🧹 Data Preprocessing

The project handles missing values using appropriate techniques:

* Numerical features → median imputation
* Categorical features → mode or `"None"` where missing values represent absence of a feature
* Categorical variables → One-Hot Encoding

The project also removes the unnecessary `Id` column before modelling.

## 🛠️ Feature Engineering

Additional features are created to improve the model's ability to capture useful relationships:

* `HouseAge` – age of the house at the time of sale
* `RemodelAge` – years since the last remodeling
* `TotalSF` – total basement and floor area
* `TotalBathrooms` – combined bathroom score
* `TotalPorchSF` – total porch area
* `HasPool` – whether the property has a pool
* `HasGarage` – whether the property has a garage
* `HasFireplace` – whether the property has a fireplace

## 📊 Model Evaluation

The models can be evaluated using:

| Metric | Description                    |
| ------ | ------------------------------ |
| MAE    | Mean Absolute Error            |
| RMSE   | Root Mean Squared Error        |
| R²     | Coefficient of Determination   |
| MAPE   | Mean Absolute Percentage Error |

Cross-validation is also used to obtain a more reliable estimate of model performance.

## 📈 Visualizations

The project includes visual analysis such as:

* Distribution plots
* Feature relationships
* Correlation analysis
* Predicted vs Actual plots
* Residual plots
* Residual distribution

## 💻 Tech Stack

* **Python**
* **Pandas**
* **NumPy**
* **Matplotlib**
* **Seaborn**
* **Scikit-learn**
* **Jupyter Notebook**

## ⚙️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/abhishek00912/House-Prediction.git
cd House-Prediction
```

### 2. Create a virtual environment

```bash
python -m venv venv
```

### 3. Activate the environment

**Windows:**

```bash
venv\Scripts\activate
```

**Linux/macOS:**

```bash
source venv/bin/activate
```

### 4. Install dependencies

```bash
pip install -r requirements.txt
```

### 5. Start Jupyter Notebook

```bash
jupyter notebook
```

Then run the notebooks in the following order:

```text
01_eda.ipynb
      ↓
02_data_cleaning.ipynb
      ↓
03_model_building.ipynb
```

## 📚 Dataset

The project uses the **Ames Housing Dataset**, a commonly used dataset for house-price regression problems. The dataset contains numerous features describing residential properties, including quality, size, location-related attributes, construction information, and other property characteristics.

## 🎯 Project Goals

The main objectives of this project are:

1. Understand the factors affecting house prices.
2. Perform effective exploratory data analysis.
3. Handle missing and categorical data.
4. Create meaningful features.
5. Train regression models.
6. Compare model performance.
7. Evaluate predictions using appropriate regression metrics.

## 🚀 Future Improvements

* Hyperparameter tuning using GridSearchCV/RandomizedSearchCV
* Experiment with XGBoost and LightGBM
* Add SHAP-based model explainability
* Build a Streamlit web application
* Deploy the prediction model
* Add interactive prediction functionality

## 👨‍💻 Author

**Abhishek Kumar Yadav**

B.Tech CSE (AI)

---

⭐ If you found this project useful, consider giving it a star!
