# Day 08: Hyperparameter Tuning and Experimentation - Further Reading

This day covers systematic approaches to hyperparameter tuning—the process of finding optimal model configurations. Good tuning practices dramatically impact model performance and training efficiency.

## References

1. **Hyperparameter Optimization: Foundations, Algorithms, and Applications**
   - [Bergstra et al.: Random Search Paper](https://jmlr.org/papers/v13/bergstra12a.html)
   - Foundational paper comparing random search vs grid search, showing random search's efficiency for high-dimensional spaces.

2. **Learning Rate Finder: A Practical Guide**
   - [Leslie Smith: A Disciplined Approach to Neural Network Training](https://arxiv.org/abs/1506.01186)
   - Paper introducing the learning rate range test (LR finder) to efficiently discover good learning rates.

3. **Experiment Tracking and Reproducibility**
   - [Weights & Biases: MLOps Fundamentals](https://docs.wandb.ai/)
   - Modern tools and best practices for tracking experiments, hyperparameters, metrics, and ensuring reproducibility.

4. **Bayesian Optimization for Hyperparameter Tuning**
   - [Hyperopt Documentation](http://hyperopt.github.io/hyperopt/)
   - Practical guide to Bayesian optimization for hyperparameter search with working implementations in Python.

5. **Early Stopping and Model Selection**
   - [PyTorch Lightning Early Stopping](https://pytorch-lightning.readthedocs.io/en/stable/common/early_stopping.html)
   - Best practices for early stopping to prevent overfitting and efficiently stop training when no improvement occurs.

---

**Tip:** Start with reference #2 for the learning rate finder, then #1 for search strategies, and #3 for experiment tracking tools.
