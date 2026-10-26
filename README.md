# Industrial Predictive Maintenance & Anomaly Detection Pipeline

An end-to-end data analytics and machine learning pipeline designed to monitor industrial water pump sensor readings, engineer rolling temporal features, and isolate operational anomalies using unsupervised machine learning.

## 📌 Project Overview
In industrial IoT (IIoT) systems, pump failures can cause critical downtimes and high operational costs. This project demonstrates how to analyze multi-sensor time-series data, handle missing values, engineer predictive features, and automatically detect anomalies to support preventive maintenance strategies.

## 🛠️ Tech Stack & Libraries
* **Language:** Python
* **Environment:** Google Colab, VS Code
* **Data Manipulation & Cleaning:** Pandas, NumPy
* **Machine Learning:** Scikit-learn (Isolation Forest)
* **Data Visualization:** Matplotlib, Seaborn

## 🔄 Pipeline Steps
1. **Data Wrangling & Cleaning:** Loaded industrial sensor datasets, handled missing values using forward-fill (`ffill`), and structured temporal data into proper datetime indices.
2. **Exploratory Data Analysis (EDA):** Analyzed sensor correlations and mapped historical `BROKEN` failure statuses against operational telemetry.
3. **Feature Engineering:** Generated 60-minute rolling means and rolling standard deviations (`rolling_mean`, `rolling_std`) to smooth out high-frequency sensor noise and capture underlying structural trends.
4. **Unsupervised Anomaly Detection:** Implemented an **Isolation Forest** model to isolate abnormal behavioral shifts and failure precursors without requiring large labeled failure datasets.
5. **Visualization:** Plotted multi-sensor time series overlaid with model-predicted anomaly markers for clear, non-technical stakeholder reporting.

## 📊 Results & Key Findings
* Successfully captured critical precursor drops and system instabilities in sensor metrics prior to failure events.
* Provided transparent, interpretable visual outputs suitable for both technical teams and operational management.

---
*Created by İbrahim Halil Aslan*
