# Day 17: Introduction to Transformers

## 🎯 Goal
Understand the Transformer architecture and why it replaced RNNs for most NLP tasks.

---

## 📚 Topics Covered
- "Attention is All You Need" paper overview
- Self-attention mechanism
- Multi-head attention
- Positional encodings
- Transformer architecture overview

---

## 📝 Syllabus

### 1. Transformer Motivation
- Limitations of RNNs/LSTMs
- Parallelization advantages
- Long-range dependencies
- Modern NLP revolution

### 2. Self-Attention
- Attention on same sequence
- Query, Key, Value from same source
- Scaled dot-product attention
- Mathematical formulation

### 3. Multi-Head Attention
- Multiple attention heads
- Different representation subspaces
- Concatenation and projection
- Why multiple heads help

### 4. Positional Encoding
- Position information problem
- Sinusoidal encodings
- Learned positional embeddings
- Adding position to embeddings

---

## ✅ Tasks

1. **Implement Self-Attention**
   - Build scaled dot-product attention
   - Test on simple sequences
   - Visualize attention patterns

2. **Multi-Head Attention**
   - Implement multi-head attention
   - Create 4-head or 8-head version
   - Compare with single head

3. **Positional Encodings**
   - Implement sinusoidal encoding
   - Visualize encoding patterns
   - Test learned vs fixed

4. **Simple Transformer Block**
   - Combine components
   - Add feedforward network
   - Layer normalization

---

## 💡 Stretch Goals (Optional)
- Read "Attention is All You Need" paper
- Implement full encoder block
- Try different attention variations
- Analyze computational complexity
