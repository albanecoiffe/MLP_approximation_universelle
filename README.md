# 🌐 Study of Universal Approximation in Neural Networks

[Notebook](https://albanecoiffe.github.io/MLP_approximation_universelle/)

## 🧠 Objective
The goal of this lab is to study a fundamental property of static (non-recurrent) neural networks: the universal approximation theorem. This property states that neural networks, even with just one hidden layer, can approximate any continuous function given sufficient neurons.

In this lab, we train a Multi-Layer Perceptron (MLP) with a single hidden layer on a piecewise-defined function and analyze how well the network approximates it.

## 📊 Lab Steps
### 1. Data Generation
The function f(x) is defined as follows:      
𝑓(𝑥)={     
sin(𝜋𝑥) si 𝑥∈[−1,1[       
0 si 𝑥∈[−2,−1]∪[1,2]       
-Adding Gaussian noise (0,0.2) to the generated data.
- Generating multiple training and test samples from this function.

### 2. mplementing MLP with TensorFlow

- Using a simple MLP with one hidden layer to approximate the generated function.
- Exploring different architectures by varying the number of hidden neurons (e.g., 1, 3, 5, 7 neurons).      
  
### Recommendations
- Analyzing results: Start with a small number of neurons and observe how the function approximation evolves.
- Testing variations: Experiment with different hidden layer sizes to see how the approximation becomes more or less "sparse" depending on the model's capacity.
- Evaluating performance: Assess the generalization of the model by testing it on a separate test set.      

## 🛠️ Technologies Used
- Python: Main programming language for implementation.
- TensorFlow: Framework for building and training the MLP neural network.
- NumPy: For generating and manipulating data.
- Matplotlib: For visualizing function approximations.
