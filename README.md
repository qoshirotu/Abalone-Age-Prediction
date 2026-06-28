# Abalone Age Prediction Using Gradient Descent

This project applies Simple Linear Regression with Gradient Descent to estimate abalone age indicators using physical measurement data from the UCI Abalone Dataset.

## Overview

The model uses **Diameter** as the input feature and **Rings** as the target variable. Ring count is commonly used as an indicator of abalone age.

The project evaluates how different learning rates affect Gradient Descent convergence and regression performance.

## Dataset

* **Dataset:** UCI Abalone Dataset
* **Instances:** 4,177
* **Features:** 8 physical measurements and 1 target variable
* **Target:** Rings
* **Selected Feature:** Diameter

## Workflow

1. Load the Abalone dataset from the UCI Machine Learning Repository.
2. Select `Diameter` as the predictor and `Rings` as the target.
3. Normalize the Diameter feature.
4. Split the data into 60% training and 40% testing sets.
5. Train a Simple Linear Regression model using Gradient Descent.
6. Compare learning rates of `0.01`, `0.1`, and `0.5`.
7. Evaluate model performance using SSE and MSE.
8. Visualize the cost function, parameter updates, regression line, and error comparison.

## Key Results

The final regression model produced approximately:

| Metric             | Training Data | Testing Data |
| ------------------ | ------------: | -----------: |
| Mean Squared Error |          7.30 |         6.46 |

The model identified a positive relationship between abalone diameter and ring count. The learning-rate experiment demonstrates the importance of selecting an appropriate optimization step size for stable and efficient convergence.

## Visualizations

The notebook includes:

* Cost Function vs. Epochs
* SSE Comparison for Training and Testing Data
* Weight and Bias Progression
* Regression Line Visualization
* Training and Testing Data Scatter Plot

## Technologies

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-learn
* UCI Machine Learning Repository

## Installation

```bash
pip install ucimlrepo pandas numpy matplotlib scikit-learn
```

## How to Run

1. Clone this repository.

```bash
git clone https://github.com/yourusername/abalone-age-prediction.git
cd abalone-age-prediction
```

2. Open the notebook.

```bash
jupyter notebook Abalone_Age.ipynb
```

3. Run the notebook cells sequentially.

> Make sure the `gradient_descent()` function is defined before running the learning-rate experiment and evaluation cells.

## Project Structure

```text
abalone-age-prediction/
│
├── Abalone_Age.ipynb
└── README.md
```

## Learning Outcomes

This project improved my understanding of feature normalization, train-test splitting, Simple Linear Regression, Gradient Descent optimization, learning-rate evaluation, SSE, MSE, and model visualization.


