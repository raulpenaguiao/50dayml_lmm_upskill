# Project 1: MNIST Neural Network Classification

## Overview
Build a comprehensive MNIST digit classification system demonstrating deep learning fundamentals.

## Goals
- Design custom CNN architecture
- Implement training pipeline with best practices
- Achieve >98% test accuracy
- Create professional, reproducible code

## Requirements

### Model Architecture
- Custom CNN with residual connections
- Batch normalization
- Dropout for regularization
- Configurable hyperparameters

### Training Pipeline
- Data augmentation
- Learning rate scheduling
- Model checkpointing
- Early stopping
- Metrics tracking (loss, accuracy)

### Evaluation
- Comprehensive test set evaluation
- Confusion matrix
- Per-class metrics
- Error analysis with visualizations

### Documentation
- Clean, well-commented code
- Results summary
- Architecture diagram
- Performance comparison table

## Project Structure
```
project1-mnist-nn/
├── data/               # MNIST dataset (auto-downloaded)
├── models/            # Saved model checkpoints
├── notebooks/         # Jupyter notebooks
│   └── mnist_classification.ipynb
├── src/               # Source code
│   ├── model.py       # Model architecture
│   ├── train.py       # Training script
│   ├── evaluate.py    # Evaluation script
│   └── utils.py       # Utility functions
├── results/           # Plots, metrics, visualizations
├── requirements.txt   # Dependencies
└── README.md         # This file
```

## Success Criteria
- [ ] Achieve >98% test accuracy
- [ ] Clean, documented code
- [ ] Comprehensive evaluation with visualizations
- [ ] Professional presentation
- [ ] Demonstrates all Phase 1 concepts

## Getting Started
1. Install dependencies: `pip install -r requirements.txt`
2. Run training: `python src/train.py`
3. Evaluate model: `python src/evaluate.py`
4. Explore notebook: `jupyter notebook notebooks/mnist_classification.ipynb`

## Related Days
- Day 1: Basic Neural Networks
- Day 2: CNNs
- Day 3-9: Advanced techniques
- Day 10: Project completion
