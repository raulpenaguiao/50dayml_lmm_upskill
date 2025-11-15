# Day 14: Long Short-Term Memory Networks (LSTMs)

## 🎯 Goal
Learn about LSTMs and how they solve the vanishing gradient problem in RNNs.

---

## 📚 Topics Covered
- Limitations of vanilla RNNs
- LSTM architecture (gates and cell state)
- GRU as LSTM alternative
- Implementation in PyTorch
- Comparison: RNN vs LSTM vs GRU

---

## 📝 Syllabus

### 1. RNN Limitations
- Vanishing gradient problem
- Long-term dependencies
- Why vanilla RNNs struggle

### 2. LSTM Architecture
- Cell state vs hidden state
- Forget gate
- Input gate
- Output gate
- Gate mechanisms explained

### 3. GRU Networks
- Simplified architecture
- Update and reset gates
- LSTM vs GRU tradeoffs

### 4. Implementation
- nn.LSTM in PyTorch
- nn.GRU in PyTorch
- Stacking LSTM layers
- Dropout in LSTMs

---

## ✅ Tasks

1. **Build LSTM Classifier**
   - Implement LSTM for sentiment analysis
   - Train on IMDb dataset
   - Compare with vanilla RNN

2. **GRU Implementation**
   - Build GRU classifier
   - Compare LSTM vs GRU
   - Analyze speed and accuracy

3. **Stacked LSTMs**
   - Create multi-layer LSTM
   - Experiment with depth
   - Monitor overfitting

4. **Performance Analysis**
   - Compare RNN/LSTM/GRU
   - Measure training time
   - Accuracy comparison table

---

## 💡 Stretch Goals (Optional)
- Implement LSTM from scratch
- Visualize gate activations
- Study attention mechanisms (preview)
- Experiment with layer normalization
