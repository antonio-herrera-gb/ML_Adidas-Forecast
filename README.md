# 🤖 Sales Forecasting with Machine Learning - Adidas Retailers 📈

Welcome to my Machine Learning project focused on predicting sales for Adidas retail distributors in the United States! 🏪 We use supervised regression models to estimate store revenue and identify key trends by product, region, and seasonality.

## 🧠 **Project Overview**

- **PART I:**

The primary goal is to predict the total sales of distributor stores based on multiple factors such as product type, price, store location, and date. 

- **PART II:**

Understand which products and markets are growing or declining 📊

Estimate if stores will reach minimum revenue targets 💰

Analyze how sales behave across seasons and months 📆

Support strategic decisions in logistics and stock distribution 🚛

This project is fully based on supervised Machine Learning, and includes the construction of a robust baseline model, hyperparameter tuning, and model evaluation.

## 📦 **The Dataset**

The dataset contains detailed sales records of Adidas distributors across the U.S. between 2020 and 2021, including:

Store information: retailer, region, state, city

Product category: product

Pricing and quantity: price_per_unit, units_sold

Date of transaction: invoice_date

Calculated target: total_sales

🧼 After cleaning missing values, correcting inconsistencies, and engineering new features (like month, quarter, and cyclical encodings), the data was ready for model training.

## 🤖 **Models Used**

We tested several models and selected the top performers:

📉 Linear Regression (Baseline)

🌲 Random Forest Regressor

⚡ XGBoost Regressor

🐱 CatBoost Regressor (best balance between performance and generalization)

GridSearchCV and KFold cross-validation were used to ensure robust model evaluation.

## 📈 **Final Results (CatBoost)**

| Metric   | Train     | Validation | Test      |
|----------|-----------|------------|-----------|
| **RMSE** | 5080.57   | 5541.40    | 5356.21   |
| **MAE**  | 3134.64   | 3214.43    | 3136.05   |
| **R²**   | 0.8350    | 0.8032     | 0.8369    |

CatBoost was selected as the final model due to its stability, native categorical handling, and excellent test performance.

## 🛠️ **Technologies Used**

- **Language**: Python 🐍

- **Libraries**: Pandas, NumPy, Scikit-learn, XGBoost, CatBoost, Matplotlib, Seaborn, Scipy, Joblib

- **Environment**: Visual Studio Code, Jupyter Notebook

## 📁 **Project Structure**
```plaintext
📦 ML_Adidas-Forecast
|
|── 📂 src/
|   ├── 📂 data/                  # Raw and cleaned datasets
|   ├── 📂 imgs/                  # Graphs and visualizations
|   ├── 📂 models/                # Saved model (CatBoost)
|   ├── 📂 notebooks/             # Jupyter notebooks (EDA, modeling, tuning)
|   ├── 📂 results_notebook/      # Final notebook
|   ├── 📂 utils/                 # Funtions
|
├── 📄 README.md              # Documentation
└── 📄 presentacion.pdf       # Presentation/report
```


## 📬 **Contact**

If you have any questions or want to collaborate, feel free to reach out:

- **Email**: [antonio-baquero@proton.me](mailto:antonio-baquero@proton.me)
- **LinkedIn**: [Antonio Herrera](https://www.linkedin.com/in/antonioherreragarciabaquero/)

Thanks for reading this project! 🧠🚀Feel free to fork it, test it, or propose improvements!

