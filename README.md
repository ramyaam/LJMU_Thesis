# Sequence-Aware Customer Lifetime Value Prediction Using Hybrid AI Models

## Overview

This repository contains the implementation developed for my master's thesis titled:

**Sequence-Aware Customer Lifetime Value Prediction Using Hybrid AI Models**

The project investigates Customer Lifetime Value (CLV) prediction by combining traditional customer-level features with sequential transaction behavior. The objective is to evaluate whether incorporating purchase sequences through an LSTM model can improve prediction accuracy over conventional machine learning approaches.

---

## Research Objective

Customer Lifetime Value is an important metric for customer relationship management and marketing decision-making. Traditional CLV prediction models typically rely on aggregated customer features such as Recency, Frequency, and Monetary (RFM) values.

This research extends the traditional approach by learning customer purchasing behavior from transaction sequences using an LSTM model. The learned sequence embeddings are combined with engineered customer features to build hybrid prediction models.

---

## Dataset

The implementation uses the **Online Retail** dataset.

The preprocessing pipeline includes:

* Data cleaning
* Missing value handling
* Removal of cancelled transactions
* Total purchase value calculation
* Customer-level aggregation

The dataset is divided into:

* **Observation Period** – used to generate customer features
* **Prediction Period** – used to calculate the target Customer Lifetime Value (CLV)

---

## Feature Engineering

Customer-level features include:

* Recency
* Frequency
* Monetary Value (RFM)
* Additional customer behavioral features derived from transaction history

The target variable (CLV) is log-transformed before model training.

---

## Sequence-Aware Learning

Customer purchase histories are converted into fixed-length transaction sequences.

An LSTM network is trained to learn sequential purchasing behavior. The hidden layer representations (sequence embeddings) are extracted and combined with customer-level features to construct hybrid datasets.

---

## Models Implemented

### Baseline Machine Learning Models

* Linear Regression
* Decision Tree Regressor
* Random Forest Regressor
* XGBoost Regressor
* LightGBM Regressor

### Deep Learning Model

* LSTM Sequence Model

### Hybrid Models

* LSTM Embeddings + XGBoost
* LSTM Embeddings + LightGBM

---

## Project Workflow

1. Install required libraries
2. Load and clean the Online Retail dataset
3. Create observation and prediction periods
4. Generate Customer Lifetime Value target
5. Perform RFM feature engineering
6. Prepare data for baseline models
7. Train and evaluate baseline machine learning models
8. Generate customer transaction sequences
9. Build and train the LSTM sequence model
10. Extract LSTM sequence embeddings
11. Create hybrid datasets by combining engineered features with sequence embeddings
12. Train Hybrid XGBoost and Hybrid LightGBM models
13. Compare model performance
14. Visualize prediction results and residual errors

---

## Evaluation Metrics

Model performance is evaluated using:

* Mean Absolute Error (MAE)
* Root Mean Squared Error (RMSE)
* R² Score

Predictions are converted back to the original CLV scale before evaluation.

---

## Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* TensorFlow / Keras
* XGBoost
* LightGBM
* Matplotlib
* Seaborn
* Google Colab

---

## Repository Contents

```text
SourceCode.ipynb        # Complete implementation
README.md               # Project documentation
```

---

## Key Outputs

The notebook includes:

* Performance comparison of all models
* Random Forest feature importance
* Actual vs Predicted CLV visualization
* Residual error analysis
* Hybrid model evaluation

---

## Research Purpose

This repository is intended for academic research and demonstrates the implementation of sequence-aware Customer Lifetime Value prediction using machine learning, deep learning, and hybrid AI models.

---

## Author

**Ramya M**

Master's Thesis

**Research Title:**
*Sequence-Aware Customer Lifetime Value Prediction Using Hybrid AI Models*
