# 🧭 IoT Sensor Anomaly Detection

### 🔍 Project Overview
This project develops an **end-to-end anomaly detection system** for IoT sensor data, designed to identify unusual readings that may signal equipment malfunction or maintenance needs.  

It demonstrates both **traditional unsupervised learning** (Isolation Forest) and **deep learning** (Autoencoder) approaches applied to time series data.

Dataset used: [`art_daily_jumpsup.csv`]

---

## ⚙️ Project Structure
├── anomaly-detection-work.ipynb # Main Jupyter notebook
├── art_daily_jumpsup.csv # Dataset used
├── IoT_Anomaly_Detection_Summary.pdf # Project summary report (2–3 pages)
├── README.md # This file


---

## 🧩 Requirements

Install dependencies using pip:

pip install pandas numpy matplotlib seaborn scikit-learn tensorflow


How to Run

Open the notebook

Load anomaly-detection-work.ipynb in Jupyter, Google Colab, or Kaggle.

Load the dataset

Ensure the file art_daily_jumpsup.csv is in the same working directory.

Run all cells sequentially

Steps are organized in the notebook:

Data Preparation & Exploration

Feature Engineering

Anomaly Detection using Isolation Forest

Anomaly Detection using Autoencoder

Model Evaluation & Visualization

View the results

Outputs include:

Raw time series and rolling mean plots

Distribution and boxplots of sensor values

Highlighted anomaly points

Autoencoder reconstruction error visualization

Model comparison table

📊 Key Features
Handles missing values and outliers

Creates rolling window & difference-based time series features

Normalizes data for better model performance

Implements two anomaly detection models:

Isolation Forest (unsupervised statistical)

Autoencoder (deep learning reconstruction)

Compares models and visualizes anomalies in context


Results Summary

| Model                | Total Anomalies | Mean (Anomalies) | Mean (Normal) | Key Trait                             |
| -------------------- | --------------- | ---------------- | ------------- | ------------------------------------- |
| **Isolation Forest** | 120             | 2.52             | -0.078        | High sensitivity, quick deployment    |
| **Autoencoder**      | 40              | 1.98             | -0.02         | High precision, fewer false positives |


Limitations & Future Work
Synthetic dataset — needs testing on real IoT sensor data.

No labeled anomalies; validation done visually and statistically.

Future versions may include:

LSTM Autoencoders for temporal learning

Streaming anomaly detection for live monitoring

Dashboard visualization for operators


👨‍💻 Author

Hemachandran M
Machine Learning Engineer | Data Science Enthusiast

