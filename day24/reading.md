# Day 24: Introduction to GPT Architecture - Further Reading

This day covers decoder-only Transformer architectures used in GPT models, which generate text autoregressively by predicting the next token given all previous tokens.

## References

1. **Language Models are Unsupervised Multitask Learners (GPT-2)**
   - [Radford et al.: GPT-2 Paper](https://d4mucfpksywv.cloudfront.net/better-language-models/language_models_are_unsupervised_multitask_learners.pdf)
   - Influential paper showing how large language models learn multiple tasks unsupervised through next-token prediction.

2. **Language Models are Few-Shot Learners (GPT-3)**
   - [Brown et al.: GPT-3 Paper](https://arxiv.org/abs/2005.14165)
   - Landmark paper demonstrating few-shot learning capabilities and scaling laws of large language models.

3. **Decoder-Only vs Encoder-Decoder**
   - [Unified Transformers: Architecture Comparison](https://huggingface.co/docs/transformers/model_summary)
   - Comparison of different transformer architectures and when to use decoder-only for generation tasks.

4. **Autoregressive Language Modeling**
   - [The Challenge of Realistic Music Generation](https://arxiv.org/abs/1811.06426)
   - Discussion of autoregressive modeling and next-token prediction for sequential generation tasks.

5. **PyTorch GPT Implementation**
   - [Nano GPT by Andrej Karpathy](https://github.com/karpathy/nanoGPT)
   - Minimal, clean PyTorch implementation of GPT for educational purposes with detailed comments.

---

**Tip:** Start with reference #5 for code understanding, #1 for GPT-2 concepts, #2 for scaling insights, and #3 for architecture comparison.
