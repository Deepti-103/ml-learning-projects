# Price vs Material Quality – Linear Regression Experiments

This mini-project explores the relationship between a product's **material quality score** and its **price** using simple linear regression. The goal is to understand how different implementation techniques affect model results and to build foundational intuition for linear regression.

## 📌 Objective

To predict product prices based on material quality scores using three different linear regression approaches:
1. **Using Scikit-learn's built-in Linear Regression**
2. **Implementing Gradient Descent from scratch**
3. **Using the Closed-form solution (Normal Equation)**

## 🧠 Dataset

For simplicity, a small synthetic dataset is used:
- `X`: Material quality score (e.g., 1 to 5)
- `y`: Product price (in arbitrary units)

You can later replace this with a real dataset from manufacturing, e-commerce, or product review data.

## 🛠️ Methods

### 1. Scikit-learn
- Utilizes the `LinearRegression` class from `sklearn.linear_model`.
- Quick and efficient for baseline results.

### 2. Manual Gradient Descent
- Implements linear regression from scratch using Python and NumPy.
- Helps understand how model parameters (weights and bias) are updated through optimization.

### 3. Closed-form Solution (Normal Equation)
- Uses the formula:
  
  \[
  w = \frac{\sum{(x - \bar{x})(y - \bar{y})}}{\sum{(x - \bar{x})^2}}, \quad b = \bar{y} - w\bar{x}
  \]
  
- No iterations or learning rate required.
- Works well for small datasets with one feature.

## 📈 Results

All three approaches produce similar weights (slope) and bias (intercept), confirming the correctness of the manual methods compared to Scikit-learn’s implementation.

## 📂 Project Structure

