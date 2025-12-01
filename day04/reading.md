# Day 04: Advanced Optimization and Gradient Dynamics - Further Reading

This day builds graduate-level understanding of optimization algorithms, gradient flow in deep networks, and numerical stability considerations that are critical for training modern deep learning models.

## References

1. **An Overview of Gradient Descent Optimization Algorithms**
   - [Sebastian Ruder's Blog](https://ruder.io/optimizers/)
   - Comprehensive review of optimization algorithms (SGD, Momentum, Adam, etc.) with intuitive explanations and comparisons.

2. **The Adam Paper: A Method for Stochastic Optimization**
   - [Adam: A Method for Stochastic Optimization](https://arxiv.org/abs/1412.6980)
   - Original paper introducing Adam optimizer with convergence analysis and adaptive learning rates explained mathematically.

3. **Understanding the Difficulty of Training Deep Feedforward Networks**
   - [Glorot & Bengio: Initialization Paper](https://proceedings.mlr.press/v9/glorot10a)
   - Foundational paper on weight initialization and vanishing/exploding gradients with mathematical analysis.

4. **3Blue1Brown - Backpropagation Calculus**
   - [3Blue1Brown: Backpropagation](https://www.youtube.com/watch?v=tIeHLnjs5U8)
   - Visual explanation of how gradients flow backward through neural networks and why the chain rule matters.

5. **Mixed Precision Training with Automatic Loss Scaling**
   - [NVIDIA Mixed Precision Training](https://docs.nvidia.com/deeplearning/performance/mixed-precision-training/)
   - Guide to numerical stability with lower precision (FP16) training and automatic loss scaling techniques.

---

**Tip:** Start with reference #4 for visual intuition, then #1 for practical optimizer understanding, and #2-3 for mathematical rigor.
