# Churn Prediction using Neural Networks

## Overview
This project focuses on predicting customer churn using a neural network model built with TensorFlow and Keras. The dataset contains various customer attributes, and the goal is to classify whether a customer will churn or not.

## Dataset
The dataset used is `churn-bigml-20.csv`. The preprocessing steps include:
- Removing unnecessary features (`State`, `Account length`, `Area code`).
- Encoding categorical variables (`International plan`, `Voice mail plan`).
- Standardizing numerical features using `StandardScaler`.
- Handling class imbalance using `SMOTE`.

## Model Architecture
The model is a sequential neural network with:
- Input layer matching the feature size.
- Three hidden layers with ReLU activation and dropout for regularization.
- Output layer with a sigmoid activation for binary classification.

## Training
- The dataset is split into training and test sets (75%-25%).
- Early stopping is used to prevent overfitting.
- The model is trained with `adam` optimizer and `binary_crossentropy` loss function.

## Evaluation
- The model's accuracy on the test set is printed.
- A confusion matrix and classification report are generated.
- Training history is plotted (loss and accuracy trends).
- An ROC curve is plotted to visualize model performance.

## Dependencies
To run this project, install the following:
```bash
pip install pandas numpy seaborn matplotlib scikit-learn imbalanced-learn tensorflow keras
```

## Running the Project
1. Load the dataset.
2. Preprocess the data.
3. Train the neural network.
4. Evaluate the model.

 Results
The model provides insights into customer churn patterns and helps businesses take proactive measures to retain customers.

