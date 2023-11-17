# Credit Analysis using Support Vector Machines (SVM)

## Overview
This repository is dedicated to credit analysis utilizing Support Vector Machines (SVM) on the German Credit dataset. The project's primary objective is to apply SVM models to predict credit risks based on various features.

## Project Structure
The project structure is organized into notebooks and datasets:
- `notebooks/`: Contains Jupyter notebooks for analysis and modeling.
- `dataset/`: Stores the German Credit dataset (`german_credit_data.csv`).

## Data Dictionary
The German Credit dataset comprises the following variables:

| Variable           | Description                             | Type      |
|--------------------|-----------------------------------------|-----------|
| Age                | Age of the individual in years           | Numerical |
| Sex                | Gender of the individual                | Categorical |
| Job                | Job category                            | Categorical |
| Housing            | Housing status                          | Categorical |
| Saving accounts    | Savings account balance                 | Categorical |
| Checking account   | Checking account balance                | Categorical |
| Credit amount      | Credit amount in Deutsche Mark          | Numerical |
| Duration           | Duration of the credit in months        | Numerical |
| Purpose            | Purpose for the credit                   | Categorical |
| Risk               | Risk associated with the credit ('good' or 'bad') | Categorical |

## Challenge and Results
The main challenge was to apply SVM and achieve a precision score higher than 0.74. The achieved results are as follows:

### SVM Parameters:
- Best Parameters: {'C': 1, 'degree': 2, 'gamma': 'scale', 'kernel': 'rbf'}
- Test Model Precision: 0.686
- Model Accuracy: 0.686

### Evaluation Metrics:

## Training Evaluation Metrics

| Precision | Recall | F1-Score | Support |
|-----------|--------|----------|---------|
| 0         | 0.98   | 0.20     | 0.34    | 210     |
| 1         | 0.75   | 1.00     | 0.85    | 490     |
|-----------|--------|----------|---------|
| Accuracy  |        |          | 0.76    | 700     |
| Macro avg | 0.86   | 0.60     | 0.60    | 700     |
| Weighted avg | 0.81 | 0.76  | 0.70    | 700     |

## Test Evaluation Metrics

| Precision | Recall | F1-Score | Support |
|-----------|--------|----------|---------|
| 0         | 0.36   | 0.06     | 0.10    | 90      |
| 1         | 0.70   | 0.96     | 0.81    | 210     |
|-----------|--------|----------|---------|
| Accuracy  |        |          | 0.69    | 300     |
| Macro avg | 0.53   | 0.51     | 0.45    | 300     |
| Weighted avg | 0.60 | 0.69  | 0.60    | 300     |


# Support Vector Machine (SVM)

Support Vector Machine (SVM) is a powerful supervised machine learning algorithm used primarily for classification tasks. Its primary objective is to find the best possible decision boundary that separates data points into different classes.

## Key Features:
- **Classification:** SVM is mainly used for classification tasks where it classifies data into different categories or classes.
- **Regression:** It can also perform regression tasks by estimating continuous values.
- **Effective in High-Dimensional Spaces:** SVM is effective even in cases where the number of dimensions is greater than the number of samples.
- **Kernel Trick:** SVM uses the kernel trick to transform data into higher dimensions, allowing for better separation of data points.

## How SVM Works:
- SVM works by finding the hyperplane that best divides a dataset into classes. This hyperplane is the one with the maximum margin or distance between the classes.
- It aims to minimize classification errors and maximize the margin, which is the distance between the hyperplane and the nearest data points from each class (support vectors).
- SVM can handle both linear and non-linear data through the use of different kernel functions such as linear, polynomial, radial basis function (RBF), and sigmoid.

## Applications:
- **Image Classification:** SVMs have been used in image classification tasks like face detection and object recognition.
- **Bioinformatics:** In genetics and biology, SVMs are used for protein classification and gene expression analysis.
- **Text and Hypertext Categorization:** SVMs are used in text and hypertext categorization, such as spam email detection and sentiment analysis.

Support Vector Machines are versatile and effective algorithms that excel in classification tasks by finding the best decision boundary between different classes in a dataset.

## Open Collaborations

Contributions to the project are welcome! If you have suggestions for improving the models, or if you have performed additional analyses that could provide further insights, please feel free to open an issue or submit a pull request.


## Getting Started

To get started with this project, clone the repository and navigate to the respective directories to access the Jupyter notebooks and the dataset:

```bash
git clone https://github.com/julioclerio/ml-svm
# Run the Jupyter notebooks
cd ml-svm/notebooks

# Access the dataset for your analyses
repository/german_credit_data.csv

