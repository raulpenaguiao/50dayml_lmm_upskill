# Day 26: BERT and Masked Language Modeling

## 🎯 Goal
Understand encoder-only Transformers and bidirectional language models like BERT.

---

## 📚 Topics Covered
- Encoder-only architecture
- Masked Language Modeling (MLM)
- Next Sentence Prediction (NSP)
- BERT pretraining objectives
- Bidirectional context

---

## 📝 Syllabus

### 1. BERT Architecture
- Encoder-only Transformer
- Why bidirectional?
- [CLS] and [SEP] tokens
- Segment embeddings

### 2. Masked Language Modeling
- Random masking strategy
- 15% masking rule
- [MASK] token handling
- Prediction task

### 3. Next Sentence Prediction
- Sentence pair task
- IsNext vs NotNext
- Training data creation
- Usefulness debate

### 4. Pretraining vs Fine-tuning
- Pretrain on large corpus
- Fine-tune on downstream tasks
- Transfer learning with BERT
- Task-specific heads

---

## ✅ Tasks

1. **Implement MLM**
   - Create masking function
   - Build BERT-style model
   - Implement MLM loss

2. **Train on MLM Task**
   - Prepare masked data
   - Train small BERT
   - Evaluate mask predictions

3. **Analyze Representations**
   - Extract embeddings
   - Visualize with t-SNE
   - Test on word similarity

4. **Compare with GPT**
   - Bidirectional vs unidirectional
   - Task suitability
   - Performance comparison

---

## 💡 Stretch Goals (Optional)
- Implement NSP task
- Try RoBERTa modifications
- Dynamic masking
- Whole word masking
