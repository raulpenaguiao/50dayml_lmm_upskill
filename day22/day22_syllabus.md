# Day 22: Transformer Decoder and Full Architecture

## 🎯 Goal
Understand and implement the Transformer decoder and complete encoder-decoder architecture.

---

## 📚 Topics Covered
- Decoder architecture
- Masked self-attention
- Cross-attention (encoder-decoder attention)
- Causal language modeling
- Full Transformer assembly

---

## 📝 Syllabus

### 1. Decoder Layer
- Masked multi-head self-attention
- Cross-attention to encoder
- Feed-forward network
- Three attention sublayers

### 2. Masked Attention
- Causal masking
- Look-ahead mask
- Padding mask
- Implementation details

### 3. Cross-Attention
- Attending to encoder output
- Query from decoder, K/V from encoder
- Information flow
- Alignment learning

### 4. Complete Transformer
- Encoder stack
- Decoder stack
- Final linear + softmax
- Tying embeddings

---

## ✅ Tasks

1. **Implement Decoder Layer**
   - Masked self-attention
   - Cross-attention
   - Feed-forward network

2. **Masking**
   - Implement causal mask
   - Combine with padding mask
   - Test masking correctness

3. **Full Transformer**
   - Assemble encoder-decoder
   - Add output projection
   - Test on toy seq2seq task

4. **Training**
   - Train on simple translation
   - Monitor attention patterns
   - Analyze learned alignments

---

## 💡 Stretch Goals (Optional)
- Implement decoder-only architecture (GPT-style)
- Encoder-only architecture (BERT-style)
- Try different mask strategies
- Implement efficient attention
