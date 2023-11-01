# KNN-ML-project

# iPhone Purchase Prediction with K-Nearest Neighbors (KNN)

This project utilizes the K-Nearest Neighbors algorithm to predict whether a person will purchase an iPhone based on their gender, age, and salary. The dataset contains information about individuals, and the goal is to build a model that accurately predicts iPhone purchases.

## Dataset Overview

The dataset 'iphone.csv' includes columns for Gender, Age, Salary, and the target variable 'Purchase Iphone'. Initial exploration shows no missing values.

## Data Preprocessing

- **Handling Categorical Data**: Gender information is converted into numerical values using LabelEncoder.
- **Feature Scaling**: StandardScaler is used to standardize the independent variables for the KNN algorithm.

## Model Building

- **K-NN Classifier**: A K-Neighbors Classifier is trained with n_neighbors set to 5.
- **Training Accuracy**: Achieves an accuracy of 91.67%.

## Model Evaluation

### Confusion Matrix Metrics

- **True Negatives (TN)**: 64
- **False Positives (FP)**: 4
- **False Negatives (FN)**: 3
- **True Positives (TP)**: 29

### Performance Metrics

- **Accuracy Score**: 93%
- **Precision Score**: 87.88%
- **Recall Score**: 90.62%

## Prediction

The model predicts whether a 'Female' aged 47 with a salary of 30000 will purchase an iPhone as '1' (indicating purchase).

## Determining Optimal n_neighbors

- Plotting training and testing accuracy against varying n_neighbors (1-20).
- Observed overfitting for lower n_neighbors (1,2) and achieved convergence at n_neighbors = 3.
- Optimal n_neighbors found at 3, as both training and testing accuracy stabilize around 93%.

## Conclusion

The model best operates with n_neighbors = 3 for this dataset, providing a stable prediction accuracy of 93% without overfitting.
