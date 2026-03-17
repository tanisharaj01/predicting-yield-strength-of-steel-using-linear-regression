# Predicting Yield Strength of Steel Alloys using Linear Regression

## Project Overview

This repository contains a Python implementation of linear regression for predicting steel strength based on the composition of metal alloys. The code utilizes the gradient descent algorithm and includes a dataset of chemical elements and their influence on alloy strength.

## Dataset

Dataset Source: Machine Learning Foundry Steel Strength Dataset Argonne National Laboratory

**steel_strength.csv**

It contains alloy composition features and measured mechanical properties.

Example columns:
* formula
* alloy composition features
* yield strength
* tensile strength
* elongation

The model currently predicts **Yield Strength** using the feature columns.

---

## Project Structure

```
project-folder
│
├── data
│   └── steel_strength.csv
│
├── golden_section_search.py
├── linear_regression.py
├── README.md
```

---

## Methodology

The project implements **Linear Regression** using **Gradient Descent optimization**.

Model equation:

y = WX + b

Where:

* X = input features
* W = model weights
* b = bias
* y = predicted output

Loss function used:

Mean Squared Error (MSE)

Loss = Σ(y - y_pred)^2 / N

Gradient Descent updates the weights iteratively to minimize the loss.

---

## Features

* Custom Linear Regression implementation
* Gradient Descent optimization
* Golden Section Search for adaptive step size
* Feature normalization
* Train/Test split
* Comparison with Scikit-Learn regression
* Loss visualization
* Scatter plot with regression line

---
## Model Visualization & Training Analysis
<img width="640" height="480" alt="Figure_2" src="https://github.com/user-attachments/assets/b15e08b4-5310-46d6-a4df-5f346df8496b" />

* The regression plot illustrates the relationship between the input features and the target variable, along with the fitted linear model.

* The model successfully captures the overall trend in the data, showing a consistent positive relationship between the features and the target. The fitted line provides a clear   approximation of how the target variable changes with respect to the input.

* While the data exhibits natural variability, the regression line effectively represents the central tendency of the dataset. This demonstrates that the model is able to learn   meaningful patterns and general trends from the data.

* Overall, the regression fit highlights the capability of a simple linear model to provide interpretable and stable predictions, serving as a strong baseline for further          improvements.


## Installation

Clone the repository:

```
git clone https://github.com/your-username/steel-strength-prediction.git
cd steel-strength-prediction
```

Install dependencies:

```
pip install numpy matplotlib scikit-learn
```

---

## Running the Project

Run the training script:

```
python linear_regression.py
```

The program will:

1. Load and preprocess the dataset
2. Train the model using Gradient Descent
3. Display training loss during iterations
4. Compare results with Scikit-Learn regression
5. Plot regression results

---

## Output

The program generates:

* Loss values during training
* Scatter plot of predictions
* Regression line
* Mean Squared Error comparison

---

## Example Visualization

The regression line shows the relationship between input features and predicted yield strength.

---

## Technologies Used

* Python
* NumPy
* Matplotlib
* Scikit-Learn

---





