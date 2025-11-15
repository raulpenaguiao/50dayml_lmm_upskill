# Day 15: Sequence-to-Sequence Models

## 🎯 Goal
Understand encoder-decoder architectures for sequence transformation tasks.

---

## 📚 Topics Covered
- Encoder-decoder architecture
- Sequence-to-sequence (seq2seq) models
- Teacher forcing
- Inference and beam search
- Applications (translation, summarization)

---

## 📝 Syllabus

### 1. Seq2Seq Fundamentals
- Encoder-decoder paradigm
- Context vector
- Variable length input/output
- Translation task setup

### 2. Encoder
- Encoding input sequence
- Final hidden state as context
- Bidirectional encoders

### 3. Decoder
- Conditional generation
- Teacher forcing during training
- Autoregressive generation
- Handling start/end tokens

### 4. Inference
- Greedy decoding
- Beam search
- Sampling strategies
- Evaluation metrics (BLEU score preview)

---

## ✅ Tasks

1. **Build Seq2Seq Model**
   - Implement encoder
   - Implement decoder
   - Train on simple task (number translation or reverse)

2. **Teacher Forcing**
   - Implement teacher forcing
   - Train with/without
   - Compare convergence

3. **Beam Search**
   - Implement greedy decoding
   - Implement beam search
   - Compare outputs

4. **Toy Translation Task**
   - Train on simple language pair
   - Generate translations
   - Analyze errors

---

## 💡 Stretch Goals (Optional)
- Implement scheduled sampling
- Try different beam widths
- Implement length normalization
- Study attention mechanism (preview for next day)
