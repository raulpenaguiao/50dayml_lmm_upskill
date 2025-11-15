# Day 12: Word Embeddings and Vector Representations

## 🎯 Goal
Learn about word embeddings and how to represent words as dense vectors that capture semantic meaning.

---

## 📚 Topics Covered
- One-hot encoding limitations
- Word embeddings (Word2Vec, GloVe)
- Embedding layers in PyTorch
- Pretrained embeddings
- Vector arithmetic and analogies

---

## 📝 Syllabus

### 1. Word Representation Methods
- One-hot encoding
- TF-IDF
- Dense embeddings
- Why embeddings work

### 2. Embedding Concepts
- Distributional semantics
- Context windows
- Skip-gram and CBOW
- Embedding dimensions

### 3. PyTorch Embeddings
- nn.Embedding layer
- Training embeddings from scratch
- Loading pretrained embeddings
- Freezing vs fine-tuning embeddings

### 4. Pretrained Models
- GloVe embeddings
- Word2Vec
- FastText
- Using pretrained weights

---

## ✅ Tasks

1. **Create Embedding Layer**
   - Implement nn.Embedding
   - Train simple embedding model
   - Visualize learned embeddings

2. **Load Pretrained Embeddings**
   - Download GloVe vectors
   - Initialize embedding layer with GloVe
   - Test on word similarity tasks

3. **Embedding Analysis**
   - Find similar words
   - Perform vector arithmetic (king - man + woman = queen)
   - Visualize embeddings with t-SNE

4. **Text Classification**
   - Build classifier with embeddings
   - Compare random vs pretrained init
   - Measure performance difference

---

## 💡 Stretch Goals (Optional)
- Train Word2Vec from scratch
- Implement skip-gram model
- Create visualization dashboard
- Study contextual embeddings (BERT preview)
