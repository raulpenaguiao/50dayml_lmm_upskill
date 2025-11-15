# Project 2: Character-Level RNN for Text Generation

## Overview
Build a character-level language model using LSTM/GRU to generate coherent text in a specific style.

## Goals
- Implement character-level RNN from scratch
- Train on interesting corpus (Shakespeare, code, poetry)
- Generate high-quality, coherent text
- Demonstrate NLP fundamentals

## Requirements

### Model Architecture
- LSTM or GRU based architecture
- Multiple layers (2-3)
- Dropout for regularization
- Configurable hidden size

### Training
- Character-level tokenization
- Sequence batching
- Gradient clipping
- Learning rate scheduling
- Perplexity tracking

### Text Generation
- Multiple sampling strategies:
  - Greedy decoding
  - Temperature sampling
  - Top-k sampling
  - Nucleus (top-p) sampling
- Seed text support
- Controllable generation

### Evaluation
- Perplexity calculation
- Sample quality assessment
- Diversity metrics
- Comparison of sampling methods

## Project Structure
```
project2-rnn-textgen/
├── data/
│   └── shakespeare.txt    # Training corpus
├── models/                # Saved checkpoints
├── notebooks/
│   └── text_generation.ipynb
├── src/
│   ├── model.py          # RNN architecture
│   ├── train.py          # Training script
│   ├── generate.py       # Generation script
│   └── utils.py          # Utilities
├── samples/              # Generated text samples
├── requirements.txt
└── README.md
```

## Success Criteria
- [ ] Model generates coherent text
- [ ] Implements multiple sampling strategies
- [ ] Achieves reasonable perplexity (<2.0)
- [ ] Clean, documented code
- [ ] Portfolio-ready presentation

## Dataset Suggestions
- Shakespeare's complete works
- Python code from GitHub
- Poetry collections
- Song lyrics
- Book corpus

## Getting Started
1. Place your text corpus in `data/`
2. Install dependencies: `pip install -r requirements.txt`
3. Train model: `python src/train.py --corpus data/shakespeare.txt`
4. Generate text: `python src/generate.py --checkpoint models/best.pt`

## Related Days
- Day 11-12: NLP basics, embeddings
- Day 13-14: RNNs and LSTMs
- Day 19: Character-level models
- Day 20: Project completion
