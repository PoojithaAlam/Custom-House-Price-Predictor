# 🏠 Custom House Price Predictor

This Web app allows you to **upload your own housing dataset** (CSV format), select the target and feature columns, and predict house prices using **Linear Regression**.

---

## 🚀 Features

- 📂 Upload any custom housing CSV file
- 🎯 Select your target price column
- 📌 Choose relevant feature columns for training
- ✏️ Input your own feature values to predict price
- 📈 View a scatter plot (1st feature vs price)
- Built with **Python**, **Streamlit**, **scikit-learn**, and **Plotly**

---

## 📸 Demo Screenshot

![App Screenshot](https://github.com/PoojithaAlam/Custom-House-Price-Predictor/blob/75e1ac2d30d3f902564149a9e457b8dbcf263416/Custom%20House.png)


![App Screenshot](https://github.com/PoojithaAlam/Custom-House-Price-Predictor/blob/75e1ac2d30d3f902564149a9e457b8dbcf263416/Custom%20House1.png)


![App Screenshot](https://github.com/PoojithaAlam/Custom-House-Price-Predictor/blob/75e1ac2d30d3f902564149a9e457b8dbcf263416/Custom%20House2.png)

---
# Website Link:

<p align="left">
  <a href="https://custom-house-price-predictor-a.streamlit.app/" target="_blank">
    <img src="https://img.shields.io/badge/Open%20Predictor-brightgreen" alt="Open Predictor">
  </a>
</p>

## 🧠 How It Works

1. Upload a CSV file with numeric columns (e.g., `GrLivArea`, `YearBuilt`, `SalePrice`, etc.)
2. Choose which column to predict (e.g., `SalePrice`)
3. Select feature columns that influence the price
4. The app trains a **Linear Regression** model on the fly
5. You can input values and get an estimated price prediction instantly

---

## 🧪 Test Cases

Use the following test cases to verify the app behavior:

### ✅ Test Case 1: Basic Prediction

- **Dataset:** Ames Housing CSV
- **Target:** `SalePrice`
- **Features:** `GrLivArea`
- **Input:** `GrLivArea = 1500`
- **Expected:** Reasonable price between $100,000 and $250,000

---

### ✅ Test Case 2: Multi-feature Prediction

- **Target:** `SalePrice`
- **Features:** `GrLivArea`, `OverallQual`, `YearBuilt`
- **Input:**  
  - `GrLivArea = 1800`  
  - `OverallQual = 7`  
  - `YearBuilt = 2005`
- **Expected:** Higher predicted price (e.g., > $200,000)

---

### ✅ Test Case 3: Invalid CSV Upload

- **Input:** Upload a non-CSV file or empty CSV
- **Expected:** App should show an error or validation warning

---

### ✅ Test Case 4: Missing Feature Values

- **Dataset:** Column has missing values (e.g., NaNs)
- **Expected:** App should either fail gracefully or prompt cleanup

---

### ✅ Test Case 5: Scatter Plot Visibility

- **Condition:** Select more than 1 feature
- **Expected:** Plot shows relationship between 1st selected feature and target column

---



## Dataset

[Dataset](https://github.com/PoojithaAlam/Custom-House-Price-Predictor/tree/75e1ac2d30d3f902564149a9e457b8dbcf263416/Dataset)

or 

Upload your own housing dataset with numerical columns like square footage, year built, etc.


## 💡 Ideas for Future Improvements
Add support for more models (e.g., Decision Trees, Random Forest)

Handle categorical features with encoding

Show model performance metrics (R², RMSE)

Enable saving and loading trained models

Add data preprocessing options (e.g., missing value handling)


## ▶️ How to Run

streamlit run app.py
## Authors

Made with ❤️ by Poojitha

