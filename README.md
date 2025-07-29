# 🌍 Novel Model to Find an Optimal Location for a Sustainable Energy Power Plant

## 🔍 Overview

This project implements a **machine learning-based suitability model** to identify optimal locations for setting up sustainable energy power plants. It integrates environmental and spatial datasets accessed via **Google Earth Engine (GEE)** and employs an **XGBoost** model with advanced preprocessing and tuning techniques.

**Key Highlights:**
- Remote sensing datasets via GEE  
- XGBoost-based ML model  
- Polynomial features & feature importance  
- Flask-based web interface

---

## 📊 Data Sources

The following satellite and spatial datasets were used:

| Dataset                   | Source                | Description               |
|--------------------------|-----------------------|---------------------------|
| `MODIS/061/MCD12Q1`      | Google Earth Engine   | Vegetation land cover     |
| `ECMWF/ERA5/DAILY`       | Google Earth Engine   | Daily wind speed          |
| `ESA/WorldCover/v100`    | Google Earth Engine   | Urbanization data         |
| `NASA/GEOS-5/MERRA2`     | Google Earth Engine   | Solar radiation levels    |

---

## ⚙️ Features and Methodology

### 📌 Data Processing
- Spatial feature extraction using GEE APIs  
- Normalization with `MinMaxScaler`

### 🧠 Feature Engineering
- Polynomial feature expansion for interaction terms

### 🤖 Machine Learning
- **XGBoost Regressor**  
- Hyperparameter tuning via `GridSearchCV`  
- Model evaluation using **R² score**

### 📈 Model Evaluation
- Feature importance analysis  
- Visualizations to interpret model decisions

<img width="1600" height="1001" alt="image" src="https://github.com/user-attachments/assets/c26bb242-2d15-472b-bd53-13b60729b055" />
<img width="1600" height="1001" alt="image" src="https://github.com/user-attachments/assets/4244fccc-b1b3-4af6-aec4-911dd7a30df2" />


---

## 🚀 Installation

Clone the repository and install the required packages:

```bash
pip install pandas numpy scikit-learn xgboost flask geopandas osmnx geopy
