# OBS - TFM
Trabajo de Fin de Máster

Este repositorio contiene el código que hemos desarrollado durante el máster de IA en OBS para:
Predecir el retraso de las salidas y llegadas de las líneas aéreas.

El ejercicio se base en un dataset que contiene más de 6M de filas, de USA y del año 2023 completo.
El código fuer realizado en python 3.12.10, utilizando visual studio code, el cual puede ser personalizado según se requiera.
Se han usado 13 modelos para verificar cúal es la mejor opción, lo cual ha resultado en que las salidas usa uno distinto al de las llegadas.
Las llegadas están supeditadas a las salidas.
La interfaz gráfica se ha realizado en GRADIO.

# ✈️ Flight Delay Prediction System

[![Hugging Face Spaces](https://img.shields.io/badge/Gradio-interface-blue?logo=gradio)](https://huggingface.co/spaces)
[![Python](https://img.shields.io/badge/Python-3.12.10-green?logo=python)](https://www.python.org/)
[![License](https://img.shields.io/badge/License-MIT-yellow)](LICENSE)

An intelligent machine learning system that predicts flight departure and arrival delays using various regression models.

# 🔢 General Information

## 📊 Dataset
- **📝 Description**: US 2023 Civil Flights, delays, meteo and aircrafts
- **📊 Dataset used**: 6,743,373 rows, 58 columns
- **📌 Features**: 58 features
- **📆 Date Range**: 2023-01-01 to 2023-12-31
- **✈️ Airlines**: 15
- **🧳 Airports**: 349
- **🛩️ Aircraft models**: 21
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
3. **Tree-based**:
     - Decision Tree (DT)
     - Random Forest (RF)
     - Extra Trees (ET)
5. **Boosting**:
     - AdaBoost
     - Gradient Boosting (GD)
     - XGBoost
     - LightGBM
     - CatBoost
7. **Other**:
     - K-Nearest Neighbors (KNN)

### Best Performing Models
- **🛫 Departure Model**: GB | MAE: 5.48 min | R²: 0.9782
- **🛬 Arrival Model**: KNN | MAE: 4.90 min | R²: 0.9838

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

## Los participantes de este proyecto hemos sido:
- Carlos
- Juan
- Nicolas
- Riccardo
