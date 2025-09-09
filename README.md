# Lab Test  – Driving Behavior & Neural Networks

## 📌 Overview
This lab test uses the **Driving Behavior Dataset** to explore the application of **Artificial Neural Networks (ANNs)**. The goal is to understand how input data is processed through a network using the **forward pass**, how errors are measured with a **loss function**, and how the **backpropagation algorithm** updates weights to improve predictions.

---

## 📂 Dataset Information
- **File name**: `Driving Behavior Dataset.csv`
- **Columns**: `Acceleration`, `Speed`, `Steering`, `Class`
- **Target**: `Class` (Driving behavior category)

---

## 🔑 Key Concepts

### 1. Neuron Forward Pass
Formula:
```math
y = f(Σ(wᵢ ⋅ xᵢ) + b)
```
Where:
- `xᵢ` → input features (e.g., speed, acceleration)
- `wᵢ` → weights (importance of each feature)
- `b` → bias (adjustment term)
- `f()` → activation function (Sigmoid, ReLU, etc.)
- `y` → neuron output

👉 This step is called the **Forward Pass**.

---

### 2. Loss Function
The **loss function** measures the difference between predicted output and actual target.

Common loss:
```math
L = (y_true - y_pred)²   # Mean Squared Error
```
👉 This step happens **after forward pass**, to compute error.

---

### 3. Backpropagation Algorithm
Backpropagation is used to **train the neural network** by updating weights.
Steps:
1. Perform **forward pass** to calculate prediction.
2. Compute **loss function**.
3. Apply **chain rule** to compute gradients (derivatives).
4. Update weights using:
```math
w = w - η * (∂L/∂w)
```
Where `η` is the learning rate.

👉 This step is called the **Backward Pass**.

---


---


- **Forward Pass** → Compute neuron output.
- **Loss Function** → Calculate error.
- **Backward Pass (Backpropagation)** → Update weights to reduce error.

This cycle repeats until the network achieves good accuracy.

---
