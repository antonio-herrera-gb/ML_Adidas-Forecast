# 🤖 Sales Forecasting with Machine Learning - Adidas Retailers 📈

Welcome to my Machine Learning project focused on predicting sales for Adidas retail distributors in the United States! 🏪 We use supervised regression models to estimate store revenue and identify key trends by product, region, and seasonality.

## 🧠 **Project Overview**

**PART I:**

- The primary goal is to predict the total sales of distributor stores based on multiple factors such as product type, price, store location, and date. 

**PART II:**

- Understand which products and markets are growing or declining 📊

- Estimate if stores will reach minimum revenue targets 💰

- Analyze how sales behave across seasons and months 📆

- Support strategic decisions in logistics and stock distribution 🚛

This project is fully based on supervised Machine Learning, and includes the construction of a robust baseline model, hyperparameter tuning, and model evaluation.

## 📦 **The Dataset**

The dataset [kaggle](https://www.kaggle.com/datasets/ahmedabbas757/dataset?resource=download) contains detailed sales records of Adidas distributors across the U.S. between 2020 and 2021 (9641 entries and 12 columns), including:

- Store information: retailer, region, state, city

- Product category: product

- Pricing and quantity: price_per_unit, units_sold

- Date of transaction: invoice_date

- Calculated target: total_sales

🧼 After cleaning missing values, correcting inconsistencies, and engineering new features (like month, quarter, and cyclical encodings), the data was ready for model training.

## 🤖 **Models Used**

We tested several models and selected the top performers:

- 📉 Linear Regression

- 🌲 Random Forest Regressor

- ⚡ XGBoost Regressor

- 🐱 CatBoost Regressor (best balance between performance and generalization)

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
|   ├── 📂 utils/                 # Functions
|
├── 📄 README.md              # Documentation
└── 📄 presentacion.pdf       # Presentation/report
```


## 📬 **Contact**

If you have any questions or want to collaborate, feel free to reach out:

- **Email**: [antonio-baquero@proton.me](mailto:antonio-baquero@proton.me)
- **LinkedIn**: [Antonio Herrera](https://www.linkedin.com/in/antonioherreragarciabaquero/)

Thanks for reading this project! 🧠🚀Feel free to fork it, test it, or propose improvements!

---------
# 🤖 Predicción de Ventas con Machine Learning - Distribuidores de Adidas 📈

¡Bienvenido a mi proyecto de Machine Learning enfocado en predecir las ventas para los distribuidores de Adidas en los Estados Unidos! 🏪 Utilizamos modelos de regresión supervisada para estimar los ingresos de las tiendas e identificar tendencias clave por producto, región y estacionalidad.

## 🧠 **Descripción del Proyecto**

**PARTE I:**

El objetivo principal es predecir las ventas totales de las tiendas distribuidoras basándose en múltiples factores, tales como el tipo de producto, precio, ubicación de la tienda y fecha.

**PARTE II:**

- Comprender qué productos y mercados están en crecimiento o en declive 📊  
- Estimar si las tiendas alcanzarán los objetivos mínimos de ingresos 💰  
- Analizar el comportamiento de las ventas a lo largo de las temporadas y los meses 📆  
- Apoyar decisiones estratégicas en logística y distribución de inventario 🚛

Este proyecto se basa completamente en Machine Learning supervisado e incluye la construcción de un modelo base robusto, ajuste de hiperparámetros y evaluación del modelo.

## 📦 **Dataset**

El dataset [kaggle](https://www.kaggle.com/datasets/ahmedabbas757/dataset?resource=download) contiene registros detallados de ventas de distribuidores de Adidas en todo EE.UU. entre 2020 y 2021 (9641 entradas y 12 columnas), incluyendo:

- Información de la tienda: retailer, region, state, city  
- Categoría del producto: product  
- Precio y cantidad: price_per_unit, units_sold  
- Fecha de la transacción: invoice_date  
- Objetivo calculado: total_sales  

🧼 Tras limpiar los valores faltantes, corregir inconsistencias e incorporar nuevas variables (como mes, trimestre y codificaciones cíclicas), los datos estuvieron listos para el entrenamiento del modelo.

## 🤖 **Modelos Utilizados**

Se probaron varios modelos y se seleccionaron los de mejor desempeño:

- 📉 Regresión Lineal  
- 🌲 Random Forest Regressor  
- ⚡ XGBoost Regressor  
- 🐱 CatBoost Regressor (mejor balance entre rendimiento y generalización)

Se utilizaron GridSearchCV y validación cruzada con KFold para asegurar una evaluación robusta del modelo.

## 📈 **Resultados Finales (CatBoost)**

| Métrica  | Entrenamiento | Validación | Test      |
|----------|---------------|------------|-----------|
| **RMSE** | 5080.57       | 5541.40    | 5356.21   |
| **MAE**  | 3134.64       | 3214.43    | 3136.05   |
| **R²**   | 0.8350        | 0.8032     | 0.8369    |

CatBoost fue seleccionado como modelo final debido a su estabilidad, manejo nativo de variables categóricas y excelente desempeño en el conjunto de test.

## 🛠️ **Tecnologías Utilizadas**

- **Lenguaje**: Python 🐍  
- **Librerías**: Pandas, NumPy, Scikit-learn, XGBoost, CatBoost, Matplotlib, Seaborn, Scipy, Joblib  
- **Entorno**: Visual Studio Code, Jupyter Notebook

## 📁 **Estructura del Proyecto**
```plaintext
📦 ML_Adidas-Forecast
|
|── 📂 src/
|   ├── 📂 data/                  # Conjuntos de datos sin procesar y limpiados
|   ├── 📂 imgs/                  # Gráficos y visualizaciones
|   ├── 📂 models/                # Modelo guardado (CatBoost)
|   ├── 📂 notebooks/             # Jupyter notebooks (EDA, modelado, ajuste)
|   ├── 📂 results_notebook/      # Notebook final
|   ├── 📂 utils/                 # Funciones
|
├── 📄 README.md              # Documentación
└── 📄 presentacion.pdf       # Presentación/informe
```

## 📬 **Contacto**

Si tienes alguna sugerencia o quieres compartir algo acerca del proyecto, aquí puedes contactarme:

- **Email**: [antonio-baquero@proton.me](mailto:antonio-baquero@proton.me)
- **LinkedIn**: [Antonio Herrera](https://www.linkedin.com/in/antonioherreragarciabaquero/)

Gracias por leer este proyecto 🧠🚀