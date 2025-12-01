# Day 25: Training GPT from Scratch - Further Reading

This day covers practical techniques for efficiently training language models including mixed precision training, gradient accumulation, and learning rate scheduling.

## References

1. **A Recipe for Training Neural Networks**
   - [Andrej Karpathy: Training Practices](http://karpathy.github.io/2019/04/25/recipe/)
   - Essential guide to training best practices including data pipeline, hyperparameter tuning, and debugging.

2. **Mixed Precision Training**
   - [Nvidia: Mixed Precision Training](https://docs.nvidia.com/deeplearning/performance/mixed-precision-training/)
   - Guide to fp16/bf16 training for efficient memory usage and faster computation on modern hardware.

3. **Gradient Accumulation and Large Batch Training**
   - [PyTorch Gradient Accumulation](https://towardsdatascience.com/what-is-gradient-accumulation-in-deep-learning-ec034122216f)
   - Explanation of gradient accumulation for simulating large batch sizes with limited memory.

4. **Learning Rate Scheduling for Language Models**
   - [WARM UP, PLATEAU, AND DECAY](https://arxiv.org/abs/1904.08779)
   - Paper analyzing learning rate schedules including warmup and decay phases critical for stable training.

5. **Scaling Laws for Neural Language Models**
   - [Kaplan et al.: Scaling Laws](https://arxiv.org/abs/2001.08361)
   - Important paper on how model/data size affect performance, guiding training decisions.

---

**Tip:** Start with reference #1 for general practices, #2-3 for efficiency techniques, #4 for learning rate scheduling, and #5 for understanding model scaling.
