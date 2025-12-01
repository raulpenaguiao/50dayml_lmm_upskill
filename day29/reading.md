# Day 29: Advanced Training Techniques for LLMs - Further Reading

This day covers advanced techniques essential for efficiently training large language models, including regularization, learning rate scheduling, gradient management, and proper initialization strategies.

## References

1. **An Overview of Gradient Descent Optimization Algorithms**
   - [Ruder: Optimizers](https://ruder.io/optimizers/)
   - Comprehensive overview of optimization algorithms and techniques for deep learning.

2. **SGDR: Stochastic Gradient Descent with Warm Restarts**
   - [Loshchilov & Hutter: SGDR](https://arxiv.org/abs/1608.03983)
   - Paper on cosine annealing schedules that improve generalization in neural networks.

3. **Decoupled Weight Decay Regularization (AdamW)**
   - [Loshchilov & Hutter: AdamW](https://arxiv.org/abs/1711.05101)
   - Important paper on properly decoupling weight decay from adaptive methods for better regularization.

4. **Understanding the Difficulty of Training Deep Feedforward Networks**
   - [Glorot & Bengio: Initialization](https://proceedings.mlr.press/v9/glorot10a)
   - Foundational paper on weight initialization addressing vanishing/exploding gradients.

5. **Gradient Checkpointing and Memory Optimization**
   - [Training ImageNet in 1 Hour](https://arxiv.org/abs/1709.05011)
   - Techniques for memory-efficient training including gradient checkpointing critical for large models.

---

**Tip:** Start with reference #2 for learning rate scheduling, #3 for AdamW, #4 for initialization, and #5 for memory efficiency techniques.
