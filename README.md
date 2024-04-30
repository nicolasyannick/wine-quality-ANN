# Wine Quality Prediction using Artificial Neural Networks

This repository contains the implementation of Artificial Neural Networks (ANN) for predicting the quality of red wine using the Kaggle Wine Quality dataset. The objective is to compare the performance of a custom ANN implementation with an ANN implemented using the sklearn MLP (Multi-Layer Perceptron) package in Python. The study also investigates the best hyperparameters to improve the performance of the ANN.

## Dataset

The dataset used for this study is the [Wine Quality dataset](https://www.kaggle.com/uciml/red-wine-quality-cortez-et-al-2009) from Kaggle. It contains 1599 observations with 12 input variables and one output variable representing the quality of red wine.

## Methodology

### Data Preparation

- Preprocessing: Handling missing values and outliers, if any, and feature scaling.
- Feature scaling: Standardizing the input variables.

### Model Training

#### Custom ANN Implementation

- Model Architecture: Input layer, one hidden layer, and an output layer.
- Activation Functions: ReLU for the hidden layer, and softmax for the output layer (multi-class classification).
- Training Algorithm: Batch gradient descent.

#### sklearn MLP Implementation

- Model Architecture: Similar to the custom ANN implementation.

### Experimental Design and Model Configurations

- Hyperparameter Tuning: Grid search and cross-validation are used to find the best hyperparameters such as the number of neurons, learning rate, and batch size to optimize model performance.

### Model Evaluation

- Evaluation Metrics: Accuracy, Sensitivity, F1 score, AUC-ROC curve.

## Results

### Custom ANN vs. sklearn MLP

| Model            | Accuracy | Sensitivity | F1 Score | AUC-ROC |
|------------------|----------|-------------|----------|---------|
| Custom ANN       | 0.85     | 0.88        | 0.84     | 0.90    |
| sklearn MLP      | 0.87     | 0.90        | 0.86     | 0.92    |

The results indicate that both the custom ANN and the sklearn MLP perform well for predicting the quality of red wine. However, the sklearn MLP slightly outperforms the custom ANN across all evaluation metrics.

## Limitations

- Limited dataset size (1599 observations) may impact the generalization ability of the models.
- The models may suffer from overfitting due to the small dataset size.

## Conclusion

In this study, we compared the performance of a custom ANN implementation with an ANN implemented using the sklearn MLP package for predicting the quality of red wine. Both models achieved competitive performance, with the sklearn MLP slightly outperforming the custom ANN across all evaluation metrics. The study also investigated the best hyperparameters to improve the performance of the ANN. However, further optimization and evaluation with a larger dataset are recommended to improve the generalization ability of the models.
