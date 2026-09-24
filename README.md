# 🦟 Machine Learning-Based Malaria Risk Prediction & Decision Support System for Nigeria

An end-to-end **data science and public health AI project** that integrates malaria survey data, climate data, machine learning, geospatial analysis, and interactive visualization to support malaria risk assessment and evidence-based decision-making in Nigeria.

**Status:** Completed MVP — continuously improving
**Author:** Olatunji Oluwaseun Abimbola
**Country:** Nigeria

---

## 📌 Project Overview

Malaria remains a major public health challenge in Nigeria. This project explores how **machine learning and data analytics** can be applied to individual-level malaria risk prediction and state-level risk mapping.

The system was designed to:

* Predict malaria infection risk
* Estimate malaria probability for individual children
* Identify important malaria risk factors
* Visualize predicted malaria risk across Nigerian states
* Provide an interactive public health dashboard
* Support evidence-based malaria intervention planning

---

## 🔄 End-to-End Data Science Workflow

**Data Sourcing → Data Integration → Data Cleaning → Exploratory Data Analysis → Feature Engineering → Data Preprocessing → Machine Learning → Model Evaluation → Geospatial Visualization → Interactive Dashboard**

---

## 📊 Data Sources & Integration

The project combines multiple data sources to create a machine-learning-ready dataset.

### Nigeria Malaria Indicator Survey (MIS)

Malaria survey data for **2010, 2015, and 2021** were obtained from the Demographic and Health Surveys (DHS) Program.

Variables included:

* Child age
* Malaria RDT result
* Mosquito net usage
* Household characteristics
* Wealth index
* Water source
* Toilet facilities
* Urban/rural residence
* State of residence

### NASA POWER Climate Data

Environmental predictors were obtained through the **NASA POWER API**, including:

* Average temperature
* Maximum temperature
* Minimum temperature
* Relative humidity
* Wind speed
* Precipitation

### Geospatial Data

Nigeria state boundary data were used for **interactive geospatial visualization and choropleth mapping**.

## The datasets were integrated using **state and survey year**, with state-name harmonization performed to resolve inconsistencies across sources.

## 🧹 Data Preparation

The data preparation workflow included:

* Missing value handling
* Duplicate removal
* Variable renaming
* Data type correction
* Categorical encoding
* State-name standardization
* Climate data integration
* Feature engineering

## The final integrated dataset contained **21,545 observations and 20 predictors**, with malaria test result used as the target variable.

## 🔬 Exploratory Data Analysis

Exploratory analysis examined:

* Age and climate-variable distributions
* Wealth and malaria relationships
* Residence and malaria relationships
* LLIN usage and malaria relationships
* Correlations between variables
* State-level malaria prevalence

These analyses were used to identify patterns and inform subsequent **feature engineering and predictive modelling**.

---

## 🤖 Machine Learning

Several classification algorithms were considered:

* Logistic Regression
* Random Forest
* XGBoost

The final model used **XGBoost**, selected based on the project's predictive-performance evaluation.

### Machine Learning Pipeline

```text
Missing Value Imputation
        ↓
Scaling
        ↓
One-Hot Encoding
        ↓
XGBoost Classifier
```

### Model Evaluation

The model was evaluated using:

* Accuracy
* Precision
* Recall
* F1-score
* ROC-AUC
* Confusion Matrix
* ROC Curve
* Feature Importance

---

## 🗺️ Interactive Public Health Dashboard

The model was integrated into a **Streamlit** application for interactive risk prediction and visualization.

### Prediction Dashboard

Users can provide information including:

* Age
* State
* Wealth
* Climate variables
* Household characteristics

The application returns:

* Predicted malaria outcome
* Probability
* Confidence
* Risk level

### Risk Visualization

The dashboard includes:

* Interactive risk gauge
* Risk-factor display
* Interpretation panel
* Public health recommendations
* Interactive Nigeria malaria risk map
* State-level predicted risk visualization

### Visualization & Application Tools

* Streamlit
* Plotly
* Folium
* GeoPandas
* Pandas
* Joblib
* XGBoost

---

## 🛠️ Technology Stack

**Programming:**
Python

**Data Analysis & Processing:**
Pandas, NumPy, Scikit-learn

**Machine Learning:**
XGBoost, Logistic Regression, Random Forest

**Visualization:**
Plotly, Folium, GeoPandas

**Dashboard:**
Streamlit

**Development:**
Jupyter Notebook, VS Code, Anaconda

**Deployment:**
Streamlit

---

## 🌍 Public Health Application

The project demonstrates how **machine learning, data integration, predictive analytics, and geospatial visualization** can be combined to support malaria surveillance and intervention planning.

Potential users include:

* Public health programmes
* Researchers
* Community health workers
* NGOs
* Health researchers
* Policy and programme stakeholders

---

## 💡 Key Skills Demonstrated

### Data Science

* Data Cleaning
* Data Preparation
* Data Integration
* Exploratory Data Analysis
* Feature Engineering
* Machine Learning
* Predictive Modelling
* Model Evaluation

### Data & Visualization

* Data Visualization
* Interactive Dashboards
* Geospatial Analysis
* Choropleth Mapping
* Data Quality & Validation

### Public Health Analytics

* Malaria Surveillance
* Climate & Health
* Risk Prediction
* Public Health Data Analysis
* Decision Support Systems

---

## 📁 Project Structure

```text
Malaria_Dashboard/
│
├── app.py
├── dashboard_data.csv
├── xgb_model.pkl
├── nigeria_states.geojson
│
├── pages/
│   ├── prediction.py
│   ├── malaria_map.py
│   └── about.py
│
├── notebooks/
│   ├── Data Cleaning.ipynb
│   ├── Feature Engineering.ipynb
│   ├── Model Training.ipynb
│   └── Evaluation.ipynb
│
├── models/
├── assets/
└── reports/
```

---

## 📈 Project Outcome

This project demonstrates an end-to-end workflow for taking a real-world public health problem from **multi-source data acquisition and integration through data preparation, exploratory analysis, machine learning, model evaluation, geospatial visualization, and interactive deployment**.

It showcases the application of data science to a practical health problem while keeping the focus on **predictive analytics, interpretability, visualization, and decision support**.

---

## 🚀 Future Improvements

Planned enhancements include:

* SHAP-based model explainability
* Individual feature-contribution analysis
* Time-series malaria forecasting
* Weather API integration
* Real-time climate prediction
* Mobile-friendly interface
* Health-facility recommendations
* REST API integration
* Docker containerization

---

## 👤 Author

**Olatunji Oluwaseun Abimbola**
Data Scientist

[GitHub](https://github.com/oaolatunji12)
