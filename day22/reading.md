# Day 22: Transformer Decoder and Full Architecture - Further Reading

This day explores the Transformer decoder with masked self-attention and cross-attention, completing the encoder-decoder architecture used for sequence-to-sequence tasks.

## References

1. **Attention Is All You Need - Complete Architecture**
   - [Vaswani et al.: Transformer Paper](https://arxiv.org/abs/1706.03762)
   - Full description of both encoder and decoder with cross-attention mechanism for seq2seq tasks.

2. **Causal Masking and Attention Masks**
   - [Understanding Attention Masks](https://huggingface.co/docs/transformers/glossary#attention-mask)
   - Clear explanation of different types of masks in transformers and how causal masking prevents looking ahead.

3. **Cross-Attention Mechanism**
   - [Transformer Architecture Visualization](https://drive.google.com/file/d/1xsYF6vP4c1r5L7DxFGbMmVSxD1tTrKq2/view)
   - Detailed visualizations showing how cross-attention connects encoder and decoder for information flow.

4. **Machine Translation with Transformer**
   - [The Best Machine Translation Systems](https://openreview.net/pdf?id=rkgNKkHtvB)
   - Analysis of transformer-based MT systems showing why encoder-decoder excels on sequence transduction.

5. **Implementing Full Transformer in PyTorch**
   - [PyTorch Transformer Module](https://pytorch.org/docs/stable/generated/torch.nn.Transformer.html)
   - Complete PyTorch implementation combining encoder and decoder with examples.

---

**Tip:** Start with reference #2 for attention mask concepts, #1 for architecture theory, #3 for cross-attention, and #5 for implementation.
