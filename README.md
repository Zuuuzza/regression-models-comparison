# Regression-models-comparison

This project focuses on regression using probabilistic and optimization-based methods. The main goal was to analyze the impact of feature transformations, scaling techniques, and regularization on model performance.

## Methods
- Data preprocessing:
  - Handling formatting issues (decimal commas)
  - Feature scaling (MinMaxScaler and StandardScaler)
- Model training:
  - Stochastic Gradient Descent (SGD)
  - Various basis functions:
    - Sigmoid
    - Polynomial (degree 1–5)
    - ReLU / Leaky ReLU
- Dataset split:
  - 60% training
  - 20% validation
  - 20% testing

## Regularization
The following techniques were applied:
- L1 (Lasso)
- L2 (Ridge)
- Elastic Net

Hyperparameters were tuned using **Random Search** over:
- Learning rate
- Regularization strength (λ)
- Elastic Net mixing parameter (α)

## Results
- Best performance achieved with **polynomial features (degree 4)**
- Regularization significantly improved stability and reduced loss
- Best models reached MSE ≈ **20,000**

## Analytical Solution
An analytical solution for Ridge Regression was also implemented:

- Closed-form solution using pseudoinverse
- Best result: **MSE = 25,720**
