# Day 13: Recurrent Neural Networks (RNNs)

## 🎯 Goal
Understand sequential data processing and implement basic RNN architectures for text classification.

---

## 📚 Topics Covered
- Sequential data and temporal dependencies
- RNN architecture and mechanics
- Hidden states
- PyTorch RNN implementation
- Handling variable-length sequences

---

## 📝 Syllabus

### 1. Sequential Data
- Why sequence matters
- Temporal dependencies
- Fixed-length vs variable-length sequences
- Sequence modeling tasks

### 2. RNN Architecture
- Recurrent connections
- Hidden state evolution
- Unrolling through time
- Parameter sharing

### 3. RNN in PyTorch
- nn.RNN module
- Input shapes and batching
- Many-to-one (classification)
- Many-to-many (sequence-to-sequence)
- One-to-many (generation)

### 4. Practical Considerations
- Padding sequences
- Packing padded sequences
- Batch-first vs time-first
- Bidirectional RNNs

---

## ✅ Tasks

1. **Build Simple RNN**
   - Implement RNN for sentiment classification
   - Use nn.RNN module
   - Train on IMDb dataset

2. **Handle Variable Lengths**
   - Implement padding
   - Use pack_padded_sequence
   - Compare with and without packing

3. **Bidirectional RNN**
   - Create bidirectional RNN
   - Compare with unidirectional
   - Analyze performance

4. **Visualization**
   - Visualize hidden states
   - Plot attention patterns (preview)
   - Error analysis

---

## 💡 Stretch Goals (Optional)
- Implement RNN from scratch
- Try many-to-many tasks
- Implement simple seq2seq model
- Study vanishing gradient problem
