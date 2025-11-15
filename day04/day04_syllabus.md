# Day 4: Advanced Optimization and Gradient Dynamics

## 🎯 Goal
Build on your graduate-level understanding of optimization to master practical aspects of training deep neural networks. Focus on modern optimizers, gradient pathologies, and numerical considerations.

**Prerequisites:** You already understand gradient descent, the chain rule, and basic optimization theory. This day covers practical deep learning-specific challenges.

**Time estimate:** 3-4 hours

---

## 📚 Topics Covered
- Modern optimization algorithms beyond vanilla SGD
- Adaptive learning rate methods (theoretical foundations)
- Gradient pathologies in deep networks
- Numerical stability and implementation details
- Second-order optimization methods (overview)

---

## 📝 Syllabus

### 1. Advanced First-Order Optimizers
- **Momentum**: Polyak momentum, Nesterov accelerated gradient
- **Adaptive methods**: AdaGrad, RMSprop (connection to diagonal preconditioning)
- **Adam and variants**: Adam, AdamW, RAdam, Lookahead
- **Convergence analysis**: Understanding why adaptive methods work
- **Mathematical insight**: Connection to preconditioned gradient descent

### 2. Gradient Flow in Deep Networks
- **Backpropagation efficiency**: Computational graph and reverse-mode autodiff
- **Jacobian structure**: Understanding gradient flow through layers
- **Vanishing/exploding gradients**: Eigenvalue analysis of Jacobians
- **Skip connections**: Mathematical motivation from ResNets
- **Batch normalization**: Effect on loss landscape smoothness

### 3. Numerical Considerations
- **Floating-point arithmetic**: Understanding precision limitations
- **Gradient clipping**: Norm-based vs value-based clipping
- **Loss scaling**: Mixed precision training considerations
- **Catastrophic cancellation**: Numerical stability in loss computation

### 4. Advanced Topics (Overview)
- **Second-order methods**: Newton's method, L-BFGS (why they're rarely used in deep learning)
- **Natural gradient descent**: Fisher information matrix perspective
- **Hessian-free optimization**: Conjugate gradient methods
- **Why first-order methods dominate**: Computational complexity analysis

---

## ✅ Tasks

1. **Implement Advanced Optimizers**
   - Code SGD with Nesterov momentum from scratch
   - Implement RMSprop and Adam
   - Understand the mathematical intuition behind each

2. **Convergence Analysis**
   - Train same network with SGD, SGD+Momentum, RMSprop, Adam
   - Plot loss landscapes (2D projections)
   - Analyze convergence rates and final performance
   - Study learning rate sensitivity for each optimizer

3. **Gradient Flow Analysis**
   - Implement gradient norm monitoring across layers
   - Detect vanishing/exploding gradients
   - Experiment with different weight initialization schemes
   - Compare gradient flow with/without batch normalization

4. **Numerical Experiments**
   - Test mixed precision training (FP16)
   - Implement and test gradient clipping strategies
   - Analyze numerical stability issues

---

## 💡 Stretch Goals (Optional)
- Implement simple autograd using computational graphs
- Code L-BFGS optimizer and compare with first-order methods
- Derive Adam update rules from first principles
- Analyze Hessian eigenvalue spectrum of your loss landscape
- Implement learning rate warmup and cosine annealing schedules
