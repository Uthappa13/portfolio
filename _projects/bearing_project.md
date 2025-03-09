---
name: Predictive Maintenance for Rotating Machines using Machine Learning Models
tools: [Python, Scikit-learn, SVM, ANN]
image: /portfolio/images/bearing_project1.png
description: Predictive maintenance for rotating machines using machine learning models.
---

# Predictive Maintenance for Rotating Machines using Machine Learning Models

## Project Overview

This project is aimed at predictive maintenance for rotating machinery by classifying the health conditions of bearings using machine learning models.
By analyzing vibration data collected from bearings under different failure conditions, the project detects and classifies faults as:
- Roller failure
- Inner race failure
- Outer race failure
- Combinations of the above failures


## Languages & Tech stack

- **Python** for implementation.
- **NumPy** & **Pandas** for data handling.
- **Scikit-learn** for machine learning models.
- **Matplotlib** for data visualization.
- **SciPy** for signal processing.
- **Self-Organizing Maps (SOM)** for anomaly detection.
- **Support Vector Machines (SVM)** for classification.
- **Artificial Neural Networks (ANN - Multi-Layer Perceptron)** for deep learning-based classification.


## Methodology

- **Data Preprocessing**
    - Vibration signals are collected using accelerometers at 50 kHz.
    - Features are extracted from both time and frequency domains.
    - Dimensionality reduction is performed using Principal Component Analysis (PCA).
- **Machine Learning Models**
    - Self-Organizing Map (SOM-MQE) is used for anomaly detection.
    - Support Vector Machines (SVM-OvO & SVM-OvR) are used for classification.
    - Artificial Neural Network (ANN-MLP) is employed for deep learning-based classification.


## Project Snippets

- **Vibration Data Analysis**
    ![Vibration Data](/portfolio/images/bearing_project2.png)

- **Bearing Health Condition Visualization**
    ![Bearing Health](/portfolio/images/bearing_project3.png)

- **Bearing Fault Classification Visualization**
    ![Bearing Fault](/portfolio/images/bearing_project4.png)

- **Confusion Matrix Visualization**
    ![Confusion](/portfolio/images/bearing_project5.png)


## Detailed code on Github

<div class="left">
{% include elements/button.html link="https://github.com/Uthappa13/Bearing-health-diagnosis/tree/master" text="Code on Github" %}
</div>
