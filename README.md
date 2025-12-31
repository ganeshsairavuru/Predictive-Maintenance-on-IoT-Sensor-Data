# IoT Predictive Maintenance using Sensor Telemetry and Machine Learning

## 📌 Project Summary
This project demonstrates an end-to-end predictive maintenance solution built on industrial IoT sensor telemetry data. The goal is to predict the **Remaining Useful Life (RUL)** of equipment using historical sensor readings, enabling proactive maintenance decisions and reducing unexpected failures.

The project mirrors real-world data engineering and machine learning workflows, including data ingestion, feature engineering, model training, evaluation, and visualization.

---

## 🎯 Business Problem
Industrial equipment failures are costly and often disruptive. Traditional reactive maintenance leads to downtime and operational risk. By analyzing time-series sensor telemetry, organizations can:
- Anticipate equipment degradation
- Schedule maintenance proactively
- Reduce operational costs and downtime

This project simulates how data engineers and ML practitioners build predictive maintenance pipelines at scale.

---

## 📊 Dataset
**NASA Turbofan Engine Degradation Dataset**

- Source: https://www.kaggle.com/datasets/behrad3d/nasa-cmaps
- Data Type: Multivariate time-series telemetry
- Records: ~20,000+ sensor readings
- Sensors: 21 continuous sensor measurements per engine
- Target: Remaining Useful Life (RUL)

Each engine operates until failure, making the dataset ideal for supervised regression modeling.

---


## 🧱 Architecture Overview

Raw Sensor Data
↓
Data Cleaning & Schema Standardization
↓
Feature Engineering (Rolling Windows, RUL)
↓
ML Training (Regression Model)
↓
Evaluation & Visualization


---

## 🔄 Data Engineering Workflow

### 1. Data Ingestion
- Loaded raw telemetry files
- Standardized schemas and column names
- Removed unused columns and validated data types

### 2. Feature Engineering
- Calculated Remaining Useful Life (RUL) per engine
- Generated rolling window statistics for key sensors
- Created ML-ready feature sets

These steps simulate batch processing commonly implemented in Spark or Databricks pipelines.

---

## 🤖 Machine Learning Approach

### Model Type
- Regression model to predict Remaining Useful Life
- Baseline model: Random Forest Regressor

### Features Used
- Raw sensor values
- Rolling mean features
- Time-based degradation signals

### Evaluation Metric
- Mean Absolute Error (MAE)

This approach prioritizes interpretability and reliability, which are critical for operational ML systems.

---

## 📈 Visualizations & Outputs

### Sensor Degradation Over Time
Visualizes sensor behavior across operational cycles for a single engine.

![Sensor Degradation](screenshots/sensor_degradation.png)

### Remaining Useful Life Distribution
Shows the distribution of RUL values used for training.

![RUL Distribution](screenshots/rul_distribution.png)

These visualizations help stakeholders understand degradation patterns and model inputs.

---

## 🛠️ Technology Stack
- Python
- Pandas & NumPy
- Scikit-learn
- Time-Series Feature Engineering
- Matplotlib
- Machine Learning for Predictive Analytics

---

## 🚀 Key Outcomes
- Built ML-ready datasets from raw IoT telemetry
- Engineered time-series and rolling features
- Trained and evaluated predictive maintenance models
- Delivered business-focused visual insights
- Simulated production-style ML pipeline design

---

## 🔍 Future Enhancements
- Implement Spark-based feature engineering
- Add streaming ingestion using Kafka or Pub/Sub
- Deploy model using batch inference pipelines
- Introduce model monitoring and drift detection

---

## 👤 Author
**Ganesh Sai Ravuru**  
Data Engineer | Analytics & Machine Learning Enthusiast  

---

## 📝 Notes
This project was designed to reflect real-world data engineering and ML workflows used in cloud environments such as Azure, AWS, and GCP.

