# Day 19: Character-Level Models and Text Generation - Further Reading

This day covers building language models that operate at the character level and generate coherent text using sampling strategies like temperature sampling and nucleus sampling.

## References

1. **The Unreasonable Effectiveness of Recurrent Neural Networks**
   - [Andrej Karpathy: Character-Level RNNs](http://karpathy.github.io/2015/05/21/rnn-effectiveness/)
   - Seminal blog post with excellent visualizations showing character-level RNNs can learn language structure and generate coherent text.

2. **Language Models are Unsupervised Multitask Learners (GPT-2 Paper)**
   - [Radford et al.: GPT-2](https://d4mucfpksywv.cloudfront.net/better-language-models/language_models_are_unsupervised_multitask_learners.pdf)
   - Paper showing how large language models learn multiple tasks unsupervised, providing context for modern text generation.

3. **Temperature and Top-k Sampling Strategies**
   - [The Curious Case of Neural Text Degeneration](https://arxiv.org/abs/1904.09751)
   - Paper analyzing sampling strategies for text generation including temperature, top-k, and nucleus (top-p) sampling.

4. **Perplexity and Language Model Evaluation**
   - [Understanding Perplexity in NLP](https://towardsdatascience.com/perplexity-in-language-models-5aab550d6ab)
   - Clear explanation of perplexity metric for evaluating language models with practical examples and intuitions.

5. **PyTorch Language Modeling Tutorial**
   - [PyTorch: Language Modeling with RNNs](https://pytorch.org/tutorials/intermediate/char_rnn_classification_tutorial.html)
   - Official tutorial implementing character-level RNN from scratch for name classification and generation.

---

**Tip:** Start with reference #1 for visual intuition, #5 for PyTorch implementation, #3 for sampling strategies, and #4 for evaluation metrics.
