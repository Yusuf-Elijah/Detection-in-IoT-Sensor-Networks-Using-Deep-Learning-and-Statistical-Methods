# Detection-in-IoT-Sensor-Networks-Using-Deep-Learning-and-Statistical-Methods
This study presents a comparative analysis of three anomaly detection algorithms: Isolation Forest, One-Class Support Vector Machine (OCSVM) and a Deep Learning Autoencoder.
IoT Sensor Anomaly Detection: Comparative Analysis 
This repository contains the official implementation of the research paper: "Comparative Analysis of Anomaly Detection in IoT Sensor Networks Using Deep Learning and Statistical Methods".

This project evaluates and benchmarks three distinct algorithmic approaches—Deep Autoencoders, Isolation Forest, and One-Class SVM—to detect irregularities in industrial sensor streams (Temperature, Humidity, and Vibration).
Project Overview
In Industrial IoT (IIoT), early detection of sensor anomalies is critical for predictive maintenance and system security. This project implements an unsupervised learning pipeline that establishes a "baseline of normalcy" and flags deviations without requiring labeled historical failure data.

Key Features:
Unsupervised Pipeline: Trained exclusively on normal operational data.

Deep Autoencoder: A 5-layer bottleneck neural network for non-linear reconstruction.

Statistical Baselines: Comparative implementation of Isolation Forest and OCSVM.

Extensive Visualization: Automated generation of ROC curves, Confusion Matrices, and Error Distributions.
Experimental Results
Our findings demonstrate that the Deep Autoencoder is the most robust model for capturing complex, non-linear relationships between sensors.

Model,Accuracy,F1-Score,ROC-AUC
Deep Autoencoder,95.8%,0.94,0.98
Isolation Forest,88.5%,0.85,0.89
One-Class SVM,81.2%,0.77,0.81

Repository Structure
├── models/                   # Saved model files (.h5 and .pkl)
│   ├── autoencoder_best.h5   # Trained Deep Learning model
│   ├── isolation_forest.pkl  # Trained Statistical model
│   └── scaler.pkl            # Preprocessing parameters
├── data/                     # Dataset (CSV)
├── figures/                  # Generated plots and visualizations
│   ├── confusion_matrices.png
│   └── roc_curves.png
├── results/                  # Performance logs and CSV reports
├── iot-anomaly-detection.ipynb # Main research notebook
└── README.md

Installation & Usage
1. Prerequisites
Python 3.11+

TensorFlow 2.12+

Scikit-learn, Pandas, Matplotlib

2. Setup
git clone https://github.com/your-username/iot-anomaly-detection.git
cd iot-anomaly-detection
pip install -r requirements.txt

3. Run the Analysis
Open the Jupyter Notebook to replicate the experiments:
Bash
jupyter notebook iot-data-anomaly-detection.ipynb

Authors
Yusuf Elijah - Lead Researcher

Team Members: Ojumu Oluwasetemi, Okoye Chukwuemeka, EreborSamuel

Supervisors: Ayuba Muhammad, Olusanya Olamide O., Kamorudeen Amuda

Affiliation: Bells University of Technology, Ota, Nigeria.
