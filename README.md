# Feedforward Neural Network from Scratch  
### Deep Learning Lab Assignment

---

## 📌 Assignment Overview

This project implements a **Feedforward Neural Network (FNN)** from scratch using Python without using any deep learning libraries such as TensorFlow, Keras, or PyTorch.

The implementation demonstrates:

- Forward Propagation  
- Backpropagation  
- Gradient Descent  
- Weight updates in each epoch  
- Loss visualization  

This assignment helps in understanding the mathematical foundation of neural networks.

---

## 🎯 Objective

To build and train a simple Feedforward Neural Network using:

- Sigmoid activation function  
- Mean Squared Error (MSE) loss  
- Gradient Descent optimization  

---

## 📊 Dataset Used

AND Gate Dataset:

| x1 | x2 | y |
|----|----|---|
| 0  | 0  | 0 |
| 0  | 1  | 0 |
| 1  | 0  | 0 |
| 1  | 1  | 1 |

This dataset is chosen because:
- It is simple and easy to verify.
- It clearly demonstrates learning behavior.
- It is suitable for understanding backpropagation.

---

## 🧠 Neural Network Architecture

- Input Layer: 2 Neurons  
- Hidden Layer: 1 Neuron  
- Output Layer: 1 Neuron  
- Activation Function: Sigmoid  
- Learning Rate: 0.5  
- Loss Function: Mean Squared Error  

---

## 🧮 Mathematical Concepts Used

### Sigmoid Function

σ(x) = 1 / (1 + e^(-x))

Derivative:

σ'(x) = σ(x)(1 − σ(x))

---

### Forward Propagation

Hidden Layer:

zh = x1w1 + x2w2 + b1  
h = sigmoid(zh)

Output Layer:

zo = hw3 + b2  
ŷ = sigmoid(zo)

---

### Backpropagation

Output Layer Gradient:

δo = (y − ŷ) * σ'(ŷ)

Hidden Layer Gradient:

δh = δo * w3 * σ'(h)

---

### Weight Update Rule

w = w + η * gradient

Where η is the learning rate.

---

## 📈 Output

During training:

- Weights are updated at each epoch.
- Loss decreases gradually.
- The network learns the AND gate mapping successfully.
- A Loss vs Epoch graph is plotted using matplotlib.

---

## ▶️ How to Run

1. Clone the repository  
2. Open Jupyter Notebook  
3. Run `DL_01.ipynb`

---

## 🛠 Requirements

- Python 3.x  
- Jupyter Notebook  
- matplotlib  

Install matplotlib using:

```
pip install matplotlib
```

---

## 📂 Project Structure

```
Feedforward-Neural-Network-From-Scratch/
│
├── FNN_Assignment.ipynb
├── README.md
├── dataset.txt
└── screenshots/
```

---

## 📚 Research Reference

Rumelhart, D. E., Hinton, G. E., & Williams, R. J. (1986).  
Learning representations by back-propagating errors.  
Nature, 323(6088), 533–536.

---

## 🌍 Applications of Feedforward Neural Networks

- Image Classification  
- Spam Detection  
- Credit Risk Prediction  
- Medical Diagnosis  
- Speech Recognition  

---

## 📌 Conclusion

The Feedforward Neural Network was successfully implemented from scratch.  
Forward propagation, backpropagation, and gradient descent were mathematically derived and implemented without using any deep learning libraries.

The model successfully learned the AND gate dataset.

---
