# 🚀 NASA Asteroid Hazard Prediction

A Machine Learning project that predicts whether a Near-Earth Object (NEO) is potentially hazardous based on its physical and orbital characteristics.

The project uses multiple classification algorithms, compares their performance, performs hyperparameter tuning using GridSearchCV, and provides an interactive prediction interface using Streamlit.

---

## 📌 Project Overview

Near-Earth Objects are asteroids and other objects whose orbits bring them relatively close to Earth.

This project uses NASA NEO dataset features to build a **binary classification model** that predicts:

- 🟢 `0` → Not Potentially Hazardous
- 🔴 `1` → Potentially Hazardous

The project demonstrates a complete Machine Learning workflow from data preprocessing to model deployment.

---

## 🎯 Objectives

- Analyze NASA Near-Earth Object data
- Perform data preprocessing and exploratory data analysis
- Identify useful features for prediction
- Train multiple Machine Learning classification models
- Compare model performance
- Perform hyperparameter tuning using GridSearchCV
- Save the trained model using Joblib
- Build an interactive Streamlit application
- Deploy the application for real-time predictions

---

## 📊 Dataset

The project uses a NASA Near-Earth Object dataset.

### Main Features

| Feature | Description |
|---|---|
| `absolute_magnitude` | Absolute magnitude of the asteroid |
| `estimated_diameter_min` | Minimum estimated diameter |
| `estimated_diameter_max` | Maximum estimated diameter |
| `relative_velocity` | Relative velocity of the asteroid |
| `miss_distance` | Distance by which the asteroid misses Earth |
| `is_hazardous` | Target variable indicating whether the asteroid is potentially hazardous |

> Note: The exact columns may vary depending on the version of the dataset being used.

---

## 🧠 Machine Learning Workflow

```text
NASA NEO Dataset
       ↓
Data Loading
       ↓
Data Cleaning
       ↓
Missing Value Handling
       ↓
Exploratory Data Analysis
       ↓
Feature Selection
       ↓
Train/Test Split
       ↓
Model Training
       ↓
Model Evaluation
       ↓
Cross Validation
       ↓
GridSearchCV
       ↓
Best Model
    
       ↓
Streamlit Application
       ↓
Deployment
