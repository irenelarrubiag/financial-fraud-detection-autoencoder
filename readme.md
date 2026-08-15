# Financial Fraud Detection Using Autoencoders

> **Work in Progress** — This project is currently under development. 
> The anomaly detection evaluation and final results are still being developed.

## Overview

This project explores the use of deep learning for unsupervised anomaly
detection in financial transactions.

The main objective is to investigate whether an autoencoder trained on
legitimate transactions can learn normal transaction behaviour and identify
unusual transactions through reconstruction error

## Dataset

The project uses the Credit Card Fraud Detection dataset from the Machine Learning Group at Université Libre de Bruxelles.

The dataset contains:

284,807 transactions
492 fraudulent transactions
31 variables
Transaction time and amount
28 anonymized numerical variables (V1–V28)
A binary Class variable indicating legitimate (0) or fraudulent (1) transactions

The dataset is highly imbalanced, with fraudulent transactions representing only 0.1727% of all observations.

## Autoencoder Architecture

The initial architecture compresses the input into a lower-dimensional latent representation.
The model is trained using Mean Squared Error (MSE) as the reconstruction loss.

The underlying idea is:

Low reconstruction error → transaction resembles learned normal behaviour
High reconstruction error → transaction differs from learned normal behaviour

A transaction is considered anomalous when its reconstruction error exceeds a selected threshold.

Technologies
Python
Pandas
NumPy
Matplotlib
Scikit-learn
TensorFlow / Keras
Jupyter Notebook

## Current Progress

The project currently includes:

- Exploratory data analysis
- Analysis of class imbalance
- Feature engineering and preprocessing
- Train/validation/test split
- Data standardization
- Autoencoder architecture design
- Model training
- Reconstruction error methodology

### Next Steps

- Calculate reconstruction errors on the test data
- Analyse the distribution of anomaly scores
- Select and evaluate different anomaly thresholds
- Evaluate fraud detection performance
- Draw final conclusions

