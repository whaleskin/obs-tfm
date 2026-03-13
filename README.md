# OBS - Trabajo de Fin de Máster
<img src="https://i.ibb.co/F4tpB7ZZ/Screenshot-2025-12-16-115230.png" alt="main-windows" border="0" width="500">
Este repositorio contiene el código que hemos desarrollado durante el máster de IA en OBS para:
Predecir el retraso de las salidas y llegadas de las líneas aéreas.

**Sistema de Predicción de Retrasos de Vuelos**

El proyecto desarrolla un sistema basado en Machine Learning para predecir retrasos en vuelos comerciales en Estados Unidos utilizando un dataset de 6,7 millones de registros combinados con datos operacionales y meteorológicos. Se evaluaron 13 modelos de regresión y 4 redes neuronales, siendo LightGBM el más preciso, con un error medio de 5 minutos en salidas y 3,72 minutos en llegadas. El sistema incluye una arquitectura escalable y una interfaz en Gradio para predicciones en tiempo real con análisis SHAP para interpretabilidad. Además, permite identificar los factores que generan retrasos, optimizando la gestión operativa de aerolíneas y mejorando la planificación de viajes para los pasajeros.

# ✈️ Flight Delay Prediction System

[![GRADIO](https://img.shields.io/badge/Gradio-interface-blue?logo=gradio)](https://www.gradio.app/guides/quickstart)
[![Python](https://img.shields.io/badge/Python-3.12.10-green?logo=python&labelColor=red)](https://www.python.org/)
[![License](https://img.shields.io/badge/License-MIT-yellow)]([LICENSE](https://creativecommons.org/publicdomain/zero/1.0/))

An intelligent machine learning system that predicts flight departure and arrival delays using various regression models.

# 🔢 General Information

## 📊 Dataset
- **📝 Description**: US 2023 Civil Flights, delays, meteo and aircrafts
- **📊 Dataset used**:
    - **Rows**: 6,743,373
    - **Cols**: 58
- **📊 Data Split**:
    - **Training set**: 5,394,698 samples
    - **Test set**: 1,348,675 samples
- **📌 Features**: 58
- **📆 Date Range**: 2023-01-01 to 2023-12-31
- **📆 Days of the week**: from Monday to Sunday
- **✈️ Airlines**: 15
- **🧳 Airports**: 349
- **🛩️ Aircraft models**: 21
- **🛩️ Aircraft manufacturer**: 5
- **💾 Source**: <a href='https://www.kaggle.com/datasets/bordanova/2023-us-civil-flights-delay-meteo-and-aircraft'>Dataset</a>
- **🌐 License**: <a href='https://creativecommons.org/publicdomain/zero/1.0/'>CC0: Public Domain</a>
- **💻 Files**: <a href='https://github.com/whaleskin/obs-tfm.git'>GitHub Repository</a>
- 🌐 Website: <a href='https://i.ibb.co/F4tpB7ZZ/Screenshot-2025-12-16-115230.png'>Flight Prediction</a>
- 📬 Contact: obstfmgrupo1@gmail.com

## 📋 Features

- **🛫 Dual Prediction**: Predicts both departure and arrival delays
- **🤖 Multiple ML Models**: Compares 13 algorithms
- **🎯 Intelligent Filtering**: Dynamic dropdowns based on real airline data
- **📊 Performance Metrics**: MAE, RMSE, R², MAPE scores for model comparison
- **🌐 Web Interface**: User-friendly Gradio interface

## 🏗️ Model Architecture

### Models Evaluated
1. **Linear Models**:
    - Linear Regression (LR)
    - Ridge
    - Lasso
    - ElasticNet
2. **Tree-based**:
     - Decision Tree (DT)
     - Random Forest (RF)
     - Extra Trees (ET)
3. **Boosting**:
     - AdaBoost
     - Gradient Boosting (GD)
     - XGBoost
     - LightGBM
     - CatBoost
4. **Other**:
     - K-Nearest Neighbors (KNN)
5. **Neural Networks**:
     - Original Neural Network
     - Wide & Deep Network
     - Residual Network
     - Transformer-Style Network

### Best Performing Models
- **🛫 Departure Model**: lightGBM | MAE: 5.00 min | R²: 0.9782
- **🛬 Arrival Model**: lightGBM | MAE: 3.70 min | R²: 0.9838

## Requirements
### Core Data Science Libraries
  - numpy>=1.24.0
  - pandas>=2.0.0
  - scipy>=1.10.0

### Machine Learning Libraries
  - scikit-learn>=1.3.0
  - xgboost>=1.7.0
  - lightgbm>=4.0.0
  - catboost>=1.2.0

### Visualization & Utilities
  - matplotlib>=3.7.0
  - seaborn>=0.12.0
  - networkx>=3.0
  - haversine>=2.8.0
  - joblib>=1.2.0

### Statistics
  - statsmodels>=0.14.0

### Web Framework
  - gradio>=4.0.0

### Hugging Face Integration
  - huggingface-hub>=0.20.0

### Optional: For data loading
  - requests>=2.31.0

## 🎮 How to Use
Once the Gradio interface is up and running, the easiest way is clicking on any of the example, and then click on the prediction button.
Otherwise, select from the dropdown lists any avilabel value and combination, and the click on the prediction button.
The results will be displayed on top of the screen. For more details see the details down below.

## 🚀 Live Demo

To try the live application, please be in touch with the developers.

**GUI**
**Main Window**
<br>
<img src="https://i.ibb.co/MkwX5mTH/main-windows.png" alt="main-windows" border="0">

**GUI**
<br>
<img src="https://i.ibb.co/wN90pr67/gradio-1.png" alt="gradio 1" border="0">

## Los participantes de este proyecto hemos sido:
- Juan
- Riccardo
