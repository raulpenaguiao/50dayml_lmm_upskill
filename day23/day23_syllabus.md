# Day 23: Tokenization Strategies for LLMs

## 🎯 Goal
Master different tokenization techniques used in modern LLMs (BPE, WordPiece, SentencePiece).

---

## 📚 Topics Covered
- Tokenization importance
- Byte-Pair Encoding (BPE)
- WordPiece tokenization
- SentencePiece
- Hugging Face tokenizers

---

## 📝 Syllabus

### 1. Tokenization Fundamentals
- Word-level limitations
- Character-level limitations
- Subword tokenization motivation
- Vocabulary size tradeoffs

### 2. Byte-Pair Encoding (BPE)
- Algorithm overview
- Building vocabulary
- Encoding and decoding
- Used in GPT models

### 3. WordPiece
- Difference from BPE
- Maximum likelihood training
- Used in BERT
- Handling unknown words

### 4. SentencePiece
- Language-agnostic tokenization
- Direct training from raw text
- Unigram language model
- Used in T5, XLNet

---

## ✅ Tasks

1. **Implement Simple BPE**
   - Code BPE algorithm
   - Train on small corpus
   - Test encoding/decoding

2. **Use Hugging Face Tokenizers**
   - Load pretrained tokenizers
   - Tokenize sample texts
   - Compare different tokenizers

3. **Train Custom Tokenizer**
   - Use tokenizers library
   - Train on custom dataset
   - Analyze vocabulary

4. **Comparison Study**
   - Compare BPE vs WordPiece
   - Vocabulary coverage
   - Tokenization speed

---

## 💡 Stretch Goals (Optional)
- Implement WordPiece from scratch
- Try SentencePiece library
- Build multilingual tokenizer
- Study byte-level BPE
