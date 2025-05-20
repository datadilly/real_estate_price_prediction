# 🏠 House Price Prediction

## Overview

This project explores various machine learning approaches to predict housing prices and analyze the profitability of an iBuyer business model. The objective was to optimize model performance while maintaining realistic generalization, and to evaluate strategies that affect profitability under certain decision-making rules.

## 📊 Project Structure

This project is built around the following core components:

- **Modeling Approaches**  
  - Baseline and advanced multilayer perceptron (MLP) models with different numbers of hidden layers and regularization strategies.
  - Progressive training with evaluation across epochs to assess model generalization and potential overfitting.

- **Regularization Techniques**  
  - L2 norm regularization and dropout were used to combat overfitting and improve validation performance.

- **Hyperparameter Tuning**  
  - Explored variations in learning rates, number of hidden layers, and layer sizes.
  - Presented validation errors for each configuration.

## 📈 Key Findings

- Overfitting was a key issue, particularly in deeper models without regularization.
- Norm regularization and dropout successfully improved generalization by stabilizing validation errors.
- Validation error divergence helped identify early stopping points and model tuning needs.

## 💸 iBuyer Profitability Analysis

Analyzed the effectiveness of the iBuyer pricing strategy using predicted house prices.

### Profit Insights

- **Bias of Prediction Errors**: +0.0457 (slight overestimation)
- **Average Profit if All Offers Accepted**: +12.28%, slightly above the target margin of 12%
- **Profit on Accepted Offers Only**: -3.17%, indicating a 15% gap below the target
- **Bias on Accepted Offers**: +0.1986, indicating substantial overestimation

These findings suggest that model overestimation combined with lenient acceptance criteria contributed to a lower than expected profit margin.

## 📁 Files

- Training/validation error plots
- Hyperparameter performance tables
- Histograms of prediction errors
- Profitability analysis write-up


## 📌 Conclusion

The models demonstrate the classic trade-off between complexity and generalization. While regularization helped improve performance, the profitability strategy still requires refinement. Future work could involve optimizing acceptance thresholds and retraining with more robust pricing data.

