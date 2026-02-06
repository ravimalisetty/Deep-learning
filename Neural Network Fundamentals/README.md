# Neural Network Fundamentals

This section focuses on understanding the fundamental building blocks of neural networks
and how different architectures are constructed using these components. The goal is to
develop a strong conceptual foundation before moving on to advanced and applied deep
learning problems.

All architectures in this folder are implemented using PyTorch, primarily from scratch,
to clearly understand how neural networks learn from data and how modern architectures
evolved over time.

---

## Core Building Blocks of Neural Networks

Neural networks are composed of the following key components, which are common across
most architectures:

### 1. Neurons and Layers
A neural network consists of interconnected neurons organized into layers:
- Input layer
- Hidden layers
- Output layer

Each neuron performs a weighted sum of inputs followed by a non-linear transformation.

---

### 2. Weights and Biases
- **Weights** control the importance of input features.
- **Biases** allow the model to shift activation functions and improve learning flexibility.

During training, these parameters are updated to minimize prediction error.

---

### 3. Activation Functions
Activation functions introduce non-linearity into the network, allowing it to model
complex patterns.

Common activation functions include:
- ReLU
- Sigmoid
- Tanh
- Softmax (for classification outputs)

---

### 4. Loss Functions
Loss functions measure how far the model’s predictions are from the actual targets.

Examples:
- Mean Squared Error (MSE) for regression
- Cross-Entropy Loss for classification

The training objective is to minimize the loss.

---

### 5. Backpropagation
Backpropagation is the algorithm used to compute gradients of the loss with respect to
model parameters. These gradients indicate how parameters should be updated to improve
performance.

---

### 6. Optimization Algorithms
Optimizers update the model parameters based on computed gradients.

Common optimizers:
- Stochastic Gradient Descent (SGD)
- Adam
- RMSprop

---

### 7. Training Process
The general training loop involves:
1. Forward pass
2. Loss computation
3. Backward pass (gradient calculation)
4. Parameter update

This process is repeated over multiple epochs until convergence.

---

## Architectures Covered

This folder contains implementations of the following neural network architectures,
organized in a learning-oriented progression:

1. **Feed Forward Neural Networks**  
   Basic fully connected networks that form the foundation of deep learning.

2. **Recurrent Neural Networks (RNN)**  
   Designed to handle sequential data by maintaining hidden states across time steps.

3. **Long Short-Term Memory (LSTM)**  
   An extension of RNNs that introduces memory cells and gating mechanisms to capture
   long-term dependencies.

4. **Gated Recurrent Unit (GRU)**  
   A simplified alternative to LSTM with fewer parameters and similar performance.

5. **Convolutional Neural Networks (CNN)**  
   Specialized networks for learning spatial features, commonly used in image processing.

6. **Encoder–Decoder (Sequence-to-Sequence) Models**  
   Architectures designed for transforming one sequence into another, such as in
   machine translation.

7. **Transformers**  
   Attention-based architectures that replace recurrence with self-attention, enabling
   efficient parallel processing and improved performance on sequence tasks.

---

## Learning Objective

The purpose of this section is to:
- Understand how neural networks work internally
- Learn why new architectures were introduced
- Build intuition for choosing the right architecture for a given problem
- Establish a strong foundation for advanced deep learning and NLP projects

This section prioritizes clarity, correctness, and conceptual understanding ov
