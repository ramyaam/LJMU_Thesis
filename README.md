# Sequence-Aware Customer Lifetime Value Prediction Using Hybrid AI Models

## Overview

This repository contains the implementation developed as part of my master's thesis titled:

**Sequence-Aware Customer Lifetime Value Prediction Using Hybrid AI Models**

The project investigates how incorporating sequential customer transaction behavior alongside traditional customer-level features can improve Customer Lifetime Value (CLV) prediction. Multiple machine learning, deep learning, and hybrid AI models are developed and compared to evaluate their predictive performance.

---

## Research Objective

Traditional CLV prediction models primarily rely on aggregated customer features such as Recency, Frequency, and Monetary (RFM) values. While effective, these approaches often ignore the temporal order of customer transactions.

This research explores whether sequence-aware learning using Long Short-Term Memory (LSTM) networks, combined with ensemble machine learning algorithms, can improve CLV prediction accuracy.

---

## Models Implemented

### Machine Learning Models

* Linear Regression
* Decision Tree Regressor
* Random Forest Regressor
* XGBoost Regressor
* LightGBM Regressor

### Deep Learning Model

* LSTM Sequence Model

### Hybrid Models

* LSTM + XGBoost
* LSTM + LightGBM

The hybrid models combine learned sequential transaction embeddings from the LSTM with engineered customer-level features before training gradient boosting models.

---

## Dataset

The experiments use the **Online Retail** dataset containing customer transaction records.

Typical preprocessing includes:

* Data cleaning
* Removal of cancelled transactions
* Missing value handling
* Customer aggregation
* Feature engineering
* RFM feature creation
* Sequential transaction generation
* Log transformation of the target variable

---

## Project Workflow

1. Data preprocessing
2. Feature engineering
3. Customer sequence generation
4. Feature scaling
5. Train-test split
6. Baseline machine learning models
7. LSTM sequence model
8. Hybrid LSTM + Gradient Boosting models
9. Model evaluation
10. Feature importance analysis

---

## Evaluation Metrics

Models are evaluated using:

* Mean Absolute Error (MAE)
* Root Mean Squared Error (RMSE)
* R² Score

The target variable is log-transformed during training and converted back to the original scale before evaluation.

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
* Google Colab

---

## Repository Structure

```
├── data/
│   └── OnlineRetail.xlsx
│
├── notebooks/
│   └── CLV_Model_Building.ipynb
│
├── README.md
└── requirements.txt
```

(Modify the structure above to match your repository.)

---

## Installation

Clone the repository:

```bash
git clone https://github.com/your-username/your-repository.git
```

Install the required libraries:

```bash
pip install -r requirements.txt
```

Open the notebook and run the cells sequentially.

---

## Results

The study compares traditional machine learning models, sequence-based deep learning, and hybrid approaches to analyze the impact of sequential transaction information on Customer Lifetime Value prediction.

Performance comparisons are based on MAE, RMSE, and R² metrics.

---

## Future Work

Potential future improvements include:

* Transformer-based sequence models
* Attention mechanisms
* Temporal Graph Neural Networks
* Hyperparameter optimization
* Real-world customer datasets
* Deployment as a prediction API

---

## Academic Use

This repository was created for academic research purposes as part of a master's thesis.

If you use this work in your research, please provide appropriate citation.

---

## Author

**Ramya M**

Master's Thesis Research

**Research Title:**
*Sequence-Aware Customer Lifetime Value Prediction Using Hybrid AI Models*

---

## License

This project is intended for educational and research purposes.
