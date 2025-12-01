# Day 23: Tokenization Strategies for LLMs - Further Reading

This day covers subword tokenization methods (BPE, WordPiece, SentencePiece) that are essential for efficient vocabulary management in modern language models.

## References

1. **Neural Machine Translation of Rare Words with Subword Units (BPE)**
   - [Sennrich et al.: BPE Paper](https://arxiv.org/abs/1508.07909)
   - Influential paper introducing Byte-Pair Encoding for handling rare words efficiently in neural MT.

2. **WordPiece and BERT Tokenization**
   - [Wu et al.: Google's Neural Machine Translation System](https://arxiv.org/abs/1609.08144)
   - Paper describing WordPiece tokenization used in BERT and other Google models.

3. **SentencePiece: A Simple and Language Agnostic Approach**
   - [Kudo & Richardson: SentencePiece](https://arxiv.org/abs/1808.06226)
   - Paper introducing SentencePiece for language-agnostic tokenization, used in T5 and multilingual models.

4. **Hugging Face Tokenizers Library**
   - [Tokenizers Documentation](https://huggingface.co/docs/tokenizers/)
   - Modern library for building and using tokenizers with implementations of BPE, WordPiece, and SentencePiece.

5. **Tokenization and Vocabulary Size Analysis**
   - [The Impact of Tokenization on Language Models](https://towardsdatascience.com/tokenization-an-illustrated-guide-7bf0f9cfc0f5)
   - Analysis of how tokenization affects vocabulary coverage, model performance, and computational efficiency.

---

**Tip:** Start with reference #4 for practical usage, #1 for BPE theory, #3 for multilingual aspects, and #5 for understanding tradeoffs.
