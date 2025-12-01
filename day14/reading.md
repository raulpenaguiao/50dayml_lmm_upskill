# Day 14: Long Short-Term Memory Networks (LSTMs) - Further Reading

This day covers LSTMs—a specialized RNN architecture with gating mechanisms that solve the vanishing gradient problem and enable learning long-term dependencies in sequences.

## References

1. **Understanding LSTM Networks (Comprehensive)**
   - [Christopher Olah's LSTM Visualizations](https://colah.github.io/posts/2015-08-Understanding-LSTMs/)
   - Detailed explanation of LSTM gates (forget, input, output) with clear diagrams showing information flow through the cell state.

2. **LSTM Paper: Hochreiter & Schmidhuber (1997)**
   - [Long Short-Term Memory](https://direct.mit.edu/neco/article/9/8/1735/6109/Long-Short-Term-Memory)
   - Original paper introducing LSTMs, providing mathematical foundations and addressing vanishing gradient problem.

3. **GRU vs LSTM Comparison**
   - [Empirical Evaluation of GRU and LSTM](https://arxiv.org/abs/1412.3555)
   - Paper comparing GRU and LSTM architectures showing tradeoffs in complexity, training time, and performance.

4. **PyTorch LSTM Implementation**
   - [PyTorch nn.LSTM Documentation](https://pytorch.org/docs/stable/generated/torch.nn.LSTM.html)
   - Complete reference for LSTM implementation in PyTorch with examples on text classification and sequence tasks.

5. **Visualizing and Understanding LSTMs**
   - [Visualizing and Understanding Recurrent Networks](https://arxiv.org/abs/1506.02078)
   - Paper with techniques to visualize and interpret LSTM hidden states and gate activations.

---

**Tip:** Start with reference #1 for intuitive understanding of gates, then #2 for theory, #4 for implementation, and #3 to understand GRU alternatives.
