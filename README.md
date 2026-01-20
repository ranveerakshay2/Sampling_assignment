
# Project Title

Sampling Assignment – Credit Card Fraud Detection


## Objective
The objective of this assignment is to analyze the importance of sampling techniques in handling a highly imbalanced dataset and to study how different sampling strategies affect the performance of various machine learning models.

Credit card fraud detection is a real-world problem where fraudulent transactions are very rare compared to legitimate ones. Without proper sampling, machine learning models tend to become biased toward the majority class.


## Dataset Description
Dataset: Creditcard_data.csv

## Methodology
Step 1: Data Loading and Preprocessing

The dataset is loaded using Pandas.
Features (X) and target (y) are separated.
Initial class distribution is analyzed to confirm imbalance.

Step 2: Dataset Balancing

SMOTE (Synthetic Minority Over-sampling Technique) is applied to balance the dataset.
SMOTE generates synthetic samples for the minority class instead of duplicating existing samples.
After SMOTE, both classes contain an equal number of samples.

Step 3: Creation of Five Samples

The balanced dataset is split into five different samples using different random states.
Each sample contains a training set and a test set.
Multiple samples ensurerobustness and reduce bias caused by a single train-test split.

Step 4: Sampling Techniques Applied
| Sampling ID | Technique             | Description                             |
| ----------- | --------------------- | --------------------------------------- |
| Sampling1   | Random Under Sampling | Reduces majority class samples          |
| Sampling2   | Random Over Sampling  | Duplicates minority class samples       |
| Sampling3   | SMOTE                 | Generates synthetic minority samples    |
| Sampling4   | SMOTE + Tomek Links   | Removes overlapping samples             |
| Sampling5   | SMOTE + ENN           | Removes noisy and misclassified samples |

Step 5: Machine Learning Models Used
| Model ID | Algorithm              |
| -------- | ---------------------- |
| M1       | Logistic Regression    |
| M2       | Decision Tree          |
| M3       | Random Forest          |
| M4       | K-Nearest Neighbors    |
| M5       | Support Vector Machine |

Step 6: Model Training and Evaluation

Each model is trained on the resampled training data.
Predictions are made on the test data.
Accuracy is used as the evaluation metric.
Final accuracy values are computed as the average accuracy across all five samples.


## Methodology
Step 1: Data Loading and Preprocessing

The dataset is loaded using Pandas.
Features (X) and target (y) are separated.
Initial class distribution is analyzed to confirm imbalance.

Step 2: Dataset Balancing

SMOTE (Synthetic Minority Over-sampling Technique) is applied to balance the dataset.
SMOTE generates synthetic samples for the minority class instead of duplicating existing samples.
After SMOTE, both classes contain an equal number of samples.

Step 3: Creation of Five Samples

The balanced dataset is split into five different samples using different random states.
Each sample contains a training set and a test set.
Multiple samples ensurerobustness and reduce bias caused by a single train-test split.

Step 4: Sampling Techniques Applied
| Sampling ID | Technique             | Description                             |
| ----------- | --------------------- | --------------------------------------- |
| Sampling1   | Random Under Sampling | Reduces majority class samples          |
| Sampling2   | Random Over Sampling  | Duplicates minority class samples       |
| Sampling3   | SMOTE                 | Generates synthetic minority samples    |
| Sampling4   | SMOTE + Tomek Links   | Removes overlapping samples             |
| Sampling5   | SMOTE + ENN           | Removes noisy and misclassified samples |

Step 5: Machine Learning Models Used
| Model ID | Algorithm              |
| -------- | ---------------------- |
| M1       | Logistic Regression    |
| M2       | Decision Tree          |
| M3       | Random Forest          |
| M4       | K-Nearest Neighbors    |
| M5       | Support Vector Machine |

Step 6: Model Training and Evaluation

Each model is trained on the resampled training data.
Predictions are made on the test data.
Accuracy is used as the evaluation metric.
Final accuracy values are computed as the average accuracy across all five samples.

| Model               | Sampling1 | Sampling2 | Sampling3 | Sampling4 | Sampling5 |
| ------------------- | --------- | --------- | --------- | --------- | --------- |
| Logistic Regression | 91.75    | 91.83     | 91.79     | 91.57     | 92..01     |
| Decision Tree       | 97.51   | 97.47     | 97.69     | 97.73     | 93.89     |
| Random Forest       | 99.52     | 99.61     | 99.61     | 99.04     | 97.16     |
| KNN                 | 84.67     | 84.59     | 84.63     | 84.15     | 81.09     |
| SVM                 | 67.99     | 68.03     | 67.99     | 67.73     |66.03     |


