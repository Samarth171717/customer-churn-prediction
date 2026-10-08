# Customer Churn Prediction

A machine learning project that predicts whether a customer is likely to churn based on customer attributes such as monthly charges, tenure, and support calls.

## 📌 Project Overview

Customer churn is an important business problem because losing customers can directly affect revenue.

In this project, a **Logistic Regression** model is trained to classify customers into two categories:

* `0` → No Churn
* `1` → Churn

The project demonstrates a complete beginner-friendly machine learning workflow using Python and Scikit-learn.

## 🎯 Problem Statement

Given information about a customer, predict whether the customer is likely to leave the service.

The model uses the following features:

* Age
* Monthly Charges
* Tenure
* Support Calls

## 🛠️ Technologies Used

* Python
* NumPy
* Pandas
* Scikit-learn
* Jupyter Notebook

## 📊 Dataset

A synthetic customer dataset containing 1,000 customer records was generated using NumPy.

The dataset contains:

* **1,000 customers**
* **4 input features**
* **1 target variable — Churn**

The churn target was generated based on combinations of monthly charges, tenure, and support calls.

> Note: Since the dataset is synthetic and the target was generated using predefined rules, the model's results should not be interpreted as real-world customer churn performance.

## 🔄 Machine Learning Workflow

The project follows these steps:

1. Generate the dataset
2. Explore the data using Pandas
3. Analyze churn patterns
4. Separate features (`X`) and target (`y`)
5. Split the data into training and testing sets
6. Train a Logistic Regression model
7. Generate predictions
8. Evaluate the model
9. Make predictions for new customers
10. Examine prediction probabilities

## 🤖 Machine Learning Model

### Logistic Regression

Logistic Regression was used as the classification algorithm because the target variable has two possible outcomes:

```text
0 → No Churn
1 → Churn
```

The dataset was divided into:

* **80% training data**
* **20% testing data**

## 📈 Model Evaluation

The model was evaluated using multiple classification metrics.

| Metric    | Score |
| --------- | ----: |
| Accuracy  |   98% |
| Precision |   80% |
| Recall    |   67% |
| F1 Score  |   73% |

### Confusion Matrix

```text
[[193   1]
 [  2   4]]
```

This corresponds to:

* True Negatives: 193
* False Positives: 1
* False Negatives: 2
* True Positives: 4

### Why multiple metrics?

Accuracy alone can be misleading when the classes are imbalanced.

Therefore, precision, recall, and F1 score were also considered to better understand how well the model identifies customers who churn.

## 🔮 Example Predictions

The trained model was tested with new customer information.

### Customer 1

```text
Age: 30
Monthly Charges: 130
Tenure: 10 months
Support Calls: 8
```

Prediction:

```text
Churn
```

The model estimated approximately **83.42% probability of churn**.

### Customer 2

```text
Age: 30
Monthly Charges: 50
Tenure: 60 months
Support Calls: 1
```

Prediction:

```text
No Churn
```

The model estimated an extremely low probability of churn for this customer.

## 📁 Project Structure

```text
customer-churn-prediction/
│
├── notebook/
│   └── churn_prediction.ipynb
│
├── .gitignore
├── README.md
└── requirements.txt
```

## ▶️ How to Run

### 1. Clone the repository

```bash
git clone <your-repository-url>
```

### 2. Navigate into the project

```bash
cd customer-churn-prediction
```

### 3. Install the required libraries

```bash
pip install -r requirements.txt
```

### 4. Open the notebook

Open:

```text
notebook/churn_prediction.ipynb
```

Run the notebook cells sequentially to reproduce the analysis and predictions.

## 📚 What I Learned

Through this project, I practiced:

* Creating and manipulating datasets with Pandas and NumPy
* Feature and target separation
* Train-test splitting
* Logistic Regression
* Model training with Scikit-learn
* Classification predictions
* Confusion matrices
* Accuracy, precision, recall, and F1 score
* Probability predictions using `predict_proba()`
* Understanding class imbalance
* Building a complete machine learning workflow



---

### Author

**Samarth S Bhat**
