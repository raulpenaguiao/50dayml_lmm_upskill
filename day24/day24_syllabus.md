# Day 24: Introduction to GPT Architecture

## 🎯 Goal
Understand decoder-only Transformers and the GPT architecture for language modeling.

---

## 📚 Topics Covered
- Decoder-only Transformers
- Autoregressive language modeling
- GPT architecture
- Next token prediction
- Causal attention masks

---

## 📝 Syllabus

### 1. Decoder-Only Architecture
- Why decoder-only for LMs?
- Comparison with encoder-decoder
- Masked self-attention
- Autoregressive generation

### 2. GPT Architecture
- Layer structure
- Positional embeddings
- Layer normalization placement
- Scaling laws preview

### 3. Language Modeling Objective
- Next token prediction
- Cross-entropy loss
- Perplexity metric
- Training on large corpora

### 4. Generation
- Greedy decoding
- Sampling strategies
- Temperature, top-k, nucleus
- Handling context window

---

## ✅ Tasks

1. **Build GPT-style Model**
   - Implement decoder-only architecture
   - Add causal masking
   - Create small GPT model

2. **Train Language Model**
   - Prepare text dataset
   - Train on next-token prediction
   - Monitor perplexity

3. **Text Generation**
   - Implement generation function
   - Try different sampling methods
   - Generate coherent samples

4. **Analysis**
   - Analyze model predictions
   - Study attention patterns
   - Compare generation strategies

---

## 💡 Stretch Goals (Optional)
- Implement GPT-2 size model
- Try different positional encodings
- Implement caching for generation
- Study model scaling
