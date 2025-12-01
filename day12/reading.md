# Day 12: Word Embeddings and Vector Representations - Further Reading

This day explores word embeddings—a fundamental shift from discrete token representations to continuous vectors that capture semantic meaning and relationships between words.

## References

1. **Word2Vec: Efficient Estimation of Word Representations**
   - [Mikolov et al.: Word2Vec Paper](https://arxiv.org/abs/1301.3781)
   - Seminal paper introducing Skip-gram and CBOW models, foundational techniques for learning word embeddings at scale.

2. **GloVe: Global Vectors for Word Representation**
   - [Stanford NLP: GloVe](https://nlp.stanford.edu/projects/glove/)
   - Paper and implementation of GloVe embeddings that combine global matrix factorization with local context window methods.

3. **Gensim: Word2Vec Implementation**
   - [Gensim Documentation: Word2Vec](https://radimrehurek.com/gensim_3.8.3/models/word2vec.html)
   - Practical Python library for training and using Word2Vec embeddings, with clear examples and tutorials.

4. **Understanding Word Embeddings Geometrically**
   - [Analogy-based word embeddings](https://towardsdatascience.com/word2vec-explained-deriving-mikolov-s-word2vec-equation-e7da5bbe341c)
   - Intuitive explanation of how word embeddings capture semantic relationships through vector arithmetic (king - man + woman ≈ queen).

5. **PyTorch nn.Embedding and Pretrained Vectors**
   - [PyTorch Embedding Layer Documentation](https://pytorch.org/docs/stable/generated/torch.nn.Embedding.html)
   - Official guide to using embeddings in PyTorch, including loading pretrained GloVe and Word2Vec vectors.

---

**Tip:** Start with reference #4 for geometric intuition, then #1-2 for theoretical understanding, and #3, #5 for practical implementations.
