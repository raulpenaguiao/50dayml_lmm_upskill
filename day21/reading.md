# Day 21: Transformer Encoder Architecture - Further Reading

This day provides a deep dive into the Transformer encoder, understanding how layer normalization, feed-forward networks, and residual connections combine to create powerful sequence models.

## References

1. **Attention Is All You Need - Detailed Analysis**
   - [Vaswani et al.: Transformer Paper](https://arxiv.org/abs/1706.03762)
   - Seminal paper with mathematical details of encoder architecture, layer normalization, and feed-forward networks.

2. **The Illustrated Transformer - Encoder Focus**
   - [Jay Alammar: Transformer Encoder](http://jalammar.github.io/illustrated-transformer/)
   - Visual breakdown of how the encoder layer components work together with clear diagrams and explanations.

3. **Layer Normalization vs Batch Normalization**
   - [Ba et al.: Layer Normalization Paper](https://arxiv.org/abs/1607.06450)
   - Paper introducing layer normalization, explaining why it works better than batch norm for transformers.

4. **Understanding Residual Connections**
   - [He et al.: Deep Residual Learning](https://arxiv.org/abs/1512.03385)
   - Classic ResNet paper introducing skip connections that are fundamental to transformer stability.

5. **Transformer Implementation in PyTorch**
   - [PyTorch Transformer Encoder](https://pytorch.org/docs/stable/generated/torch.nn.TransformerEncoderLayer.html)
   - Official PyTorch implementation of transformer encoder layer with detailed documentation.

---

**Tip:** Start with reference #2 for visual intuition, #1 for theory, #3 for layer norm, and #5 for PyTorch implementation details.
