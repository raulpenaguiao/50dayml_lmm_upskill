# Day 19: Character-Level Models and Text Generation

## 🎯 Goal
Learn to build character-level language models for text generation tasks.

---

## 📚 Topics Covered
- Character-level vs word-level modeling
- Language modeling task
- Temperature sampling
- Beam search for generation
- Evaluation metrics (perplexity)

---

## 📝 Syllabus

### 1. Language Modeling
- Next token prediction
- Character-level LM
- Autoregressive models
- Perplexity metric

### 2. Character-Level Processing
- Character vocabulary
- Why character-level?
- Advantages and disadvantages
- Unicode handling

### 3. Generation Strategies
- Greedy generation
- Temperature sampling
- Top-k sampling
- Nucleus (top-p) sampling

### 4. Training Considerations
- Sequence length
- Batch generation
- Gradient clipping
- Learning rate schedules

---

## ✅ Tasks

1. **Build Character RNN**
   - Implement char-level RNN/LSTM
   - Train on text corpus
   - Generate sample text

2. **Sampling Strategies**
   - Implement temperature sampling
   - Try different temperatures
   - Implement top-k sampling

3. **Train on Dataset**
   - Choose text corpus (Shakespeare, code, etc.)
   - Train language model
   - Generate creative samples

4. **Evaluation**
   - Calculate perplexity
   - Qualitative analysis
   - Diversity metrics

---

## 💡 Stretch Goals (Optional)
- Try word-level model
- Implement nucleus sampling
- Conditional generation
- Fine-tune on specific style
