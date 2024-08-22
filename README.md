# Time Series Forecasting Project

## Project Objective

The objective of this project is to predict future samples of a multivariate time series using advanced deep learning techniques. The goal is to design and implement models that can effectively leverage past observations in the input sequence to accurately forecast future values. This project explores different model architectures, including autoregressive models, encoder-decoder structures, and ensemble methods, to achieve the best possible forecasting performance.

## What Has Been Done

1. **Data Loading and Pre-processing**:
    - The dataset was loaded and explored using custom functions.
    - Anomalies were identified but deemed to have minimal impact on model performance.
    - The data was split using a hold-out cross-validation method (90% training, 10% validation), ensuring that the most recent data was used for validation.

2. **Model Development**:
    - **Autoregression**:
        - An autoregressive model was developed, where predictions were made iteratively with a shifting window. This model achieved a CodaLab score of 3.912.
    - **Encoder-Decoder**:
        - An encoder-decoder architecture was implemented, incorporating Gaussian Noise layers for robustness. The model achieved a slightly better CodaLab score of 3.892.
    - **Ensemble Methods**:
        - Several ensemble strategies were applied, including simple averaging, weighted averaging, and feature replacement. The best-performing ensemble method achieved a CodaLab score of 3.364, indicating significant improvement over individual models.

3. **Hyper-parameter Tuning**:
    - Hyper-parameters were tuned using Bayesian Optimization, particularly focusing on significant model changes. This approach ensured that the best possible model configurations were used.

4. **Conclusions**:
    - The project successfully applied multiple advanced deep learning techniques to time series forecasting, resulting in models that improved progressively. Despite attempts to implement additional mechanisms like attention or transformers, challenges such as computational limitations were encountered. The project reflects a thorough learning process with promising results and a clear direction for future work.

## Results

- **Best Autoregressive Model**: CodaLab score of 3.912.
- **Best Encoder-Decoder Model**: CodaLab score of 3.892.
- **Best Ensemble Model**: CodaLab score of 3.364.

This project demonstrates a robust application of time series forecasting methods, culminating in a model that significantly improves upon the initial baseline.

