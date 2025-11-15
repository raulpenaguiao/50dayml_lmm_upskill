# Project 3: minGPT - Shakespeare Text Generation

## Overview
Build and train a GPT model from scratch following Andrej Karpathy's minGPT, trained on Shakespeare's works to generate Shakespearean text.

## Goals
- Implement GPT architecture from scratch
- Train on Shakespeare corpus
- Generate convincing Shakespearean text
- Achieve <2.0 perplexity
- Demonstrate Transformer mastery

## Requirements

### Model Architecture
- Multi-head self-attention
- Causal masking
- Layer normalization
- Residual connections
- Configurable size (6-12 layers)
- Position embeddings

### Training Pipeline
- Character-level tokenization
- Efficient data loading
- Learning rate warmup and cosine decay
- Gradient clipping
- Model checkpointing
- Mixed precision training (optional)

### Text Generation
- Multiple sampling strategies
- Temperature control
- Top-k and nucleus sampling
- Seed text support
- Diverse, high-quality examples

### Evaluation
- Training/validation loss curves
- Perplexity calculation
- Generation quality assessment
- Ablation studies
- Comparison with baseline

## Project Structure
```
project3-minGPT/
├── data/
│   └── shakespeare.txt       # Training data
├── models/
│   └── checkpoints/         # Model checkpoints
├── notebooks/
│   └── mingpt_shakespeare.ipynb
├── src/
│   ├── model.py             # GPT implementation
│   ├── trainer.py           # Training utilities
│   ├── config.py            # Configuration
│   ├── utils.py             # Utilities
│   └── generate.py          # Generation script
├── outputs/
│   └── generated_samples/   # Generated text
├── requirements.txt
└── README.md
```

## Model Configuration
```python
# Suggested configuration
model_config = {
    'n_layer': 6,          # Number of transformer blocks
    'n_head': 6,           # Number of attention heads
    'n_embd': 384,         # Embedding dimension
    'block_size': 256,     # Context length
    'dropout': 0.1,        # Dropout rate
    'vocab_size': 65       # Character vocabulary
}

training_config = {
    'batch_size': 64,
    'learning_rate': 3e-4,
    'warmup_steps': 500,
    'max_steps': 10000,
    'grad_clip': 1.0
}
```

## Success Criteria
- [ ] Complete GPT implementation from scratch
- [ ] Achieves <2.0 perplexity on Shakespeare
- [ ] Generates convincing Shakespearean text
- [ ] Clean, well-documented code
- [ ] Comprehensive evaluation
- [ ] Portfolio-ready presentation

## Sample Generations
After training, the model should generate text like:
```
ROMEO:
What light through yonder window breaks?
It is the east, and Juliet is the sun...
```

## Getting Started
1. Download Shakespeare data:
   ```bash
   wget https://raw.githubusercontent.com/karpathy/char-rnn/master/data/tinyshakespeare/input.txt -O data/shakespeare.txt
   ```
2. Install dependencies: `pip install -r requirements.txt`
3. Train model: `python src/train.py`
4. Generate text: `python src/generate.py --checkpoint models/best.pt`

## Reference
Based on Andrej Karpathy's minGPT: https://github.com/karpathy/minGPT

## Related Days
- Day 17: Introduction to Transformers
- Day 21-22: Transformer architecture
- Day 24-25: GPT architecture and training
- Day 27-28: minGPT study and implementation
- Day 30: Project completion
