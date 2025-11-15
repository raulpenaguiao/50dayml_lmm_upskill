# Day 5: Neural Networks from First Principles (NumPy Implementation)

## 🎯 Goal
Implement a complete neural network library from scratch using only NumPy, leveraging your linear algebra and calculus knowledge to build a deep understanding of autodifferentiation and backpropagation.

**Prerequisites:** Strong linear algebra (matrix multiplication, Jacobians) and calculus (chain rule, gradients). You'll implement the mathematical formulas you already understand.

**Time estimate:** 4-5 hours (this is a substantial implementation day)

---

## 📚 Topics Covered
- Computational graphs and autodifferentiation
- Efficient matrix-based forward propagation
- Reverse-mode automatic differentiation (backprop)
- Modular layer design
- Numerical gradient checking

---

## 📝 Syllabus

### 1. Mathematical Foundations Review
- **Matrix calculus**: Jacobians, vector-Jacobian products
- **Chain rule for vector functions**: Composition of linear and nonlinear layers
- **Computational graphs**: DAG representation of neural networks
- **Reverse-mode autodiff**: Why it's O(n) instead of O(n²)

### 2. Modular Layer Design
- **Abstract Layer class**: forward() and backward() methods
- **Linear layer**: Y = XW + b, deriving ∂L/∂W, ∂L/∂b, ∂L/∂X
- **Activation functions**:
  - ReLU and its gradient (handling x=0)
  - Sigmoid, Tanh (numerical stability considerations)
  - Softmax with log-sum-exp trick
- **Loss functions**: Cross-entropy (numerical stable implementation)

### 3. Backpropagation Engine
- **Forward pass**: Caching activations for backprop
- **Backward pass**: Computing and propagating gradients
- **Gradient accumulation**: Handling branches in computation graph
- **Numerical gradient checking**: Finite differences validation

### 4. Optimization and Training
- **Mini-batch SGD implementation**: Efficient matrix operations
- **Weight initialization**: Xavier/He initialization (mathematical justification)
- **Training loop**: Epoch, batch iteration, gradient updates
- **Monitoring**: Loss, accuracy, gradient norms

### 5. Advanced Considerations
- **Vectorization**: Broadcasting and efficient NumPy operations
- **Memory efficiency**: In-place operations where possible
- **Numerical stability**: Avoiding overflow/underflow

---

## ✅ Tasks

1. **Build Layer Abstraction**
   - Design abstract Layer base class
   - Implement Linear layer with proper gradient computation
   - Implement ReLU, Sigmoid, Tanh activation layers
   - Implement Softmax + Cross-Entropy loss (numerically stable)

2. **Implement Backpropagation**
   - Code forward pass with activation caching
   - Implement backward pass for each layer type
   - Chain gradients through multiple layers
   - **Validate with numerical gradients** (essential step!)

3. **Training on MNIST**
   - Implement mini-batch SGD
   - Train 2-3 layer network
   - Achieve >90% accuracy
   - Monitor gradient norms to detect vanishing/exploding gradients

4. **Analysis and Comparison**
   - Compare speed: NumPy implementation vs PyTorch
   - Verify gradient correctness (numerical vs analytical)
   - Profile bottlenecks (matrix mult, activation, backprop)
   - Understand why frameworks are faster (BLAS, GPU, etc.)

---

## 💡 Stretch Goals (Optional)
- Implement convolutional layer using im2col trick
- Add batch normalization with proper train/test mode handling
- Build momentum and Adam optimizers from scratch
- Implement automatic differentiation using computational graphs
- Add L2 regularization and dropout
- Compare numerical stability of different loss formulations
