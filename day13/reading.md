# Day 13: Recurrent Neural Networks (RNNs) - Further Reading

This day introduces RNNs—neural networks designed to process sequential data by maintaining hidden states that evolve over time, enabling models to capture temporal dependencies.

## References

1. **The Unreasonable Effectiveness of Recurrent Neural Networks**
   - [Andrej Karpathy's Blog Post](http://karpathy.github.io/2015/05/21/rnn-effectiveness/)
   - Intuitive explanation of RNNs with clear visualizations and practical examples showing their power on sequence tasks.

2. **Understanding LSTM Networks**
   - [Christopher Olah's LSTM Blog Post](https://colah.github.io/posts/2015-08-Understanding-LSTMs/)
   - Classic blog post with excellent visualizations explaining RNN basics and the vanishing gradient problem (preview of Day 14).

3. **PyTorch RNN Tutorial**
   - [PyTorch: Sequence Models and LSTM](https://pytorch.org/tutorials/beginner/nlp/sequence_models_tutorial.html)
   - Official tutorial implementing RNNs and LSTMs with practical examples on NLP tasks.

4. **Handling Variable-Length Sequences**
   - [PyTorch: PackedSequence Documentation](https://pytorch.org/docs/stable/generated.html#torch.nn.utils.rnn.pack_padded_sequence)
   - Guide to efficiently handling variable-length sequences using packing and padding techniques.

5. **Bidirectional RNNs and Attention Preview**
   - [Attention is All You Need (Preview)](https://arxiv.org/abs/1706.03762)
   - Transformers paper that provides context on limitations of RNNs and sets up the need for attention mechanisms (Day 16 topic).

---

**Tip:** Start with reference #1 for intuitive understanding, then #2 for foundations, #3 for PyTorch implementation, and #4 for practical sequence handling.
