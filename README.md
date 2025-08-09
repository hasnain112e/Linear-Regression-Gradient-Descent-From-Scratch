# Linear-Regression-Gradient-Descent-From-Scratch
# 📉 Linear Regression with Gradient Descent - From Scratch

## 📌 Project Overview
This project demonstrates how to implement **Linear Regression** with **Gradient Descent** from scratch in Python using synthetic data.  
The goal is to understand the mathematics behind gradient descent, how parameters are updated iteratively, and how the model learns to fit data over time.

## 📊 Data Generation
- Equation: **y = 3x + 4 + noise**
- 100 random `x` values between 0 and 2
- Gaussian noise added for realistic variation

## ⚙️ Gradient Descent Implementation
- Parameters:
  - Initial slope (`m`) = 0
  - Initial intercept (`b`) = 0
- Hyperparameters:
  - Learning rate = 0.05
  - Epochs = 1000
- Steps:
  1. Compute predictions: `y_pred = m * X + b`
  2. Calculate error: `y_pred - y_true`
  3. Compute gradients:
     - `dm = (2/n) * sum(error * X)`
     - `db = (2/n) * sum(error)`
  4. Update parameters:
     - `m -= learning_rate * dm`
     - `b -= learning_rate * db`
  5. Track Mean Squared Error (MSE) over time
  6. Print progress every 100 epochs

## 📈 Visualizations
- **Fitted Line Plot:** Original data points vs final regression line
- **Loss Curve:** Loss reduction over training epochs

## 🛠 Technologies Used
- Python
- NumPy
- Matplotlib

## 🔧 How to Run
```bash
# Clone the repository
git clone https://github.com/yourusername/Linear-Regression-Gradient-Descent-From-Scratch.git
cd Linear-Regression-Gradient-Descent-From-Scratch

# Install dependencies
pip install numpy matplotlib

# Run the notebook
jupyter notebook gradient_descent_linear_regression.ipynb
