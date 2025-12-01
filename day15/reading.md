# Day 15: Sequence-to-Sequence Models - Further Reading

This day covers encoder-decoder architectures that transform one sequence into another—fundamental to tasks like machine translation, summarization, and question-answering.

## References

1. **Sequence to Sequence Learning with Neural Networks**
   - [Sutskever et al.: Seq2Seq Paper](https://arxiv.org/abs/1409.3215)
   - Seminal paper introducing the encoder-decoder paradigm for machine translation and sequence transformation tasks.

2. **Attention Mechanism (Preview for Next Day)**
   - [Bahdanau et al.: Neural Machine Translation with Attention](https://arxiv.org/abs/1409.0473)
   - Paper introducing attention mechanism to improve seq2seq models, essential context for Day 16 on transformers.

3. **PyTorch Seq2Seq Tutorial**
   - [PyTorch Seq2Seq Translation Example](https://pytorch.org/tutorials/intermediate/seq2seq_translation_tutorial.html)
   - Practical step-by-step tutorial implementing a complete seq2seq model for French-English translation.

4. **Beam Search and Decoding Strategies**
   - [An Empirical Exploration of Beam Search](https://arxiv.org/abs/1907.01248)
   - Paper analyzing different decoding strategies (greedy, beam search, sampling) and their impact on generation quality.

5. **Teacher Forcing and Training Techniques**
   - [Scheduled Sampling Paper](https://arxiv.org/abs/1506.02891)
   - Paper on improving seq2seq training through scheduled sampling, addressing exposure bias between training and inference.

---

**Tip:** Start with reference #1 for seq2seq fundamentals, #3 for implementation, #2 for attention preview, and #4-5 for advanced techniques.
