# Day 41: Introduction to Retrieval-Augmented Generation (RAG)

## 🎯 Goal
Understand RAG architecture and how it combines retrieval with language generation.

---

## 📚 Topics Covered
- RAG architecture overview
- Vector databases basics
- Semantic search
- Combining retrieval with LLMs
- Use cases for RAG

---

## 📝 Syllabus

### 1. RAG Fundamentals
- Limitations of pure LLMs
- Knowledge grounding
- RAG pipeline components
- When to use RAG

### 2. Vector Embeddings
- Sentence embeddings
- Dense retrieval
- Embedding models (sentence-transformers)
- Similarity metrics

### 3. Vector Databases
- FAISS basics
- ChromaDB
- Pinecone
- Storage and retrieval

### 4. RAG Pipeline
- Document preprocessing
- Embedding generation
- Retrieval step
- Generation with context

---

## ✅ Tasks

1. **Setup Embeddings**
   - Install sentence-transformers
   - Generate embeddings for documents
   - Test similarity search

2. **Build Simple Vector DB**
   - Use FAISS
   - Index documents
   - Retrieve top-k similar

3. **Basic RAG System**
   - Combine retrieval + GPT-2/BERT
   - Test on Q&A task
   - Analyze outputs

4. **Evaluation**
   - Compare with/without retrieval
   - Measure answer quality
   - Identify limitations

---

## 💡 Stretch Goals (Optional)
- Try different embedding models
- Implement hybrid search
- Experiment with chunk sizes
- Add re-ranking step
