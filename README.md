# Microsoft: Classifying Cybersecurity Incidents with Machine Learning

**Project Title:** Microsoft: Classifying Cybersecurity Incidents with Machine Learning

## Table of Contents

- [Project Overview](#project-overview)
- [Skills Developed](#skills-developed)
- [Domain](#domain)
- [Problem Statement](#problem-statement)
- [Business Use Cases](#business-use-cases)
- [Dataset Overview](#dataset-overview)
- [Approach](#approach)
  - [1. Data Exploration and Understanding](#1-data-exploration-and-understanding)
  - [2. Data Preprocessing](#2-data-preprocessing)
  - [3. Model Selection and Training](#3-model-selection-and-training)
  - [4. Model Evaluation and Tuning](#4-model-evaluation-and-tuning)
  - [5. Model Interpretation](#5-model-interpretation)
  - [6. Final Evaluation on Test Set](#6-final-evaluation-on-test-set)
  - [7. Documentation and Reporting](#7-documentation-and-reporting)
- [Results](#results)
- [Project Deliverables](#project-deliverables)
- [Evaluation Metrics](#evaluation-metrics)
- [Technical Tags](#technical-tags)

---

## Project Overview

This project focuses on developing a machine learning model to classify cybersecurity incidents as **True Positive (TP)**, **Benign Positive (BP)**, or **False Positive (FP)** using the GUIDE dataset. The objective is to improve the efficiency of Security Operation Centers (SOCs) by automating the triage process and providing analysts with accurate, context-rich insights.

## Skills Developed

- Data Preprocessing and Feature Engineering
- Machine Learning Classification Techniques
- Model Evaluation Metrics (Macro-F1 Score, Precision, Recall)
- Cybersecurity Concepts (MITRE ATT&CK Framework)
- Handling Imbalanced Datasets
- Model Benchmarking and Optimization

## Domain

**Cybersecurity and Machine Learning**

## Problem Statement

As a data scientist at Microsoft, your task is to develop a machine learning model that predicts the triage grade of cybersecurity incidents based on historical evidence and customer responses. The model should:

- Classify incidents as **TP (True Positive)**, **BP (Benign Positive)**, or **FP (False Positive)**.
- Improve guided response systems by providing accurate recommendations.
- Be evaluated using **Macro-F1 Score**, **Precision**, and **Recall** on the test dataset.

## Business Use Cases

1. **Security Operation Centers (SOCs)**: Automating incident triage to help analysts prioritize threats.
2. **Incident Response Automation**: Providing guided response actions based on incident classifications.
3. **Threat Intelligence**: Enhancing threat detection accuracy by incorporating historical data.
4. **Enterprise Security Management**: Reducing false positives and addressing threats promptly.

## Dataset Overview

The **GUIDE dataset** consists of three levels of data:

1. **Evidence Level**: Metadata supporting an alert (IP address, user details, etc.).
2. **Alert Level**: Aggregates evidence into potential security incidents.
3. **Incident Level**: Represents security breaches or threat scenarios.

- **Training Set**: 70% of data, stratified by triage grade, OrgId, and DetectorId.
- **Test Set**: 30% of data, stratified similarly.

The dataset contains **45 features** and **1 million triage-annotated incidents**.

## Approach

### 1. Data Exploration and Understanding

- **Initial Inspection**: Analyze the train.csv structure (features, data types, target distribution).
- **Exploratory Data Analysis (EDA)**: Visualize patterns, correlations, and class imbalances.

### 2. Data Preprocessing

- **Handling Missing Data**: Imputation or removal based on analysis.
- **Feature Engineering**: Creating new features (e.g., timestamp-derived features).
- **Encoding Categorical Variables**: One-hot encoding, label encoding, or target encoding.
- **Data Splitting**: Train-validation split (e.g., 80-20) with stratification.

### 3. Model Selection and Training

- **Baseline Model**: Start with Logistic Regression or Decision Tree.
- **Advanced Models**: Random Forest, XGBoost, LightGBM, Neural Networks.
- **Cross-Validation**: k-Fold Cross-Validation to reduce overfitting.

### 4. Model Evaluation and Tuning

- **Metrics**: Macro-F1 Score, Precision, Recall.
- **Hyperparameter Tuning**: Grid Search or Random Search.
- **Handling Imbalance**: SMOTE, class weights, or ensemble methods.

### 5. Model Interpretation

- **Feature Importance**: SHAP values, permutation importance.
- **Error Analysis**: Identify common misclassifications for improvements.

### 6. Final Evaluation on Test Set

- **Testing**: Evaluate model on test.csv.
- **Compare to Baseline**: Ensure consistency and improvement.

### 7. Documentation and Reporting

- **Document Process**: Data preprocessing, model selection, and evaluation.
- **Recommendations**: Integration into SOC workflows and future improvements.

## Results

By the end of this project, the outcomes will include:

- A machine learning model that accurately classifies cybersecurity incidents (TP, BP, FP).
- High **Macro-F1 Score**, **Precision**, and **Recall**.
- Insights into feature importance and model performance.
- Comprehensive documentation and deployment recommendations.

## Project Deliverables

1. **Source Code**: Well-documented code covering all steps.
2. **Model File**: Trained model ready for deployment.
3. **Documentation**: Report detailing the approach, challenges, and findings.
4. **Presentation**: Summary of project outcomes and business impact.

## Evaluation Metrics

- **Macro-F1 Score**: Balanced performance across TP, BP, and FP classes.
- **Precision**: Accuracy of positive predictions.
- **Recall**: Model's ability to detect true positives.

## Technical Tags

- **Machine Learning**
- **Classification**
- **Cybersecurity**
- **Data Science**
- **Model Evaluation**
- **Feature Engineering**
- **SOC**
- **Threat Detection**


**Author:** PraveeN R  
