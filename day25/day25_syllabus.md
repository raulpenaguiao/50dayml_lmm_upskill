# Day 25: Training GPT from Scratch

## 🎯 Goal
Train a small GPT model from scratch and understand training dynamics of language models.

---

## 📚 Topics Covered
- Dataset preparation for LM training
- Training loop for autoregressive models
- Gradient accumulation
- Mixed precision training
- Monitoring training progress

---

## 📝 Syllabus

### 1. Data Preparation
- Text corpus selection
- Tokenization
- Creating training sequences
- Batching strategies

### 2. Training Configuration
- Model size considerations
- Batch size and gradient accumulation
- Learning rate scheduling
- Warmup steps

### 3. Efficient Training
- Mixed precision (fp16/bf16)
- Gradient checkpointing
- Memory optimization
- Distributed training preview

### 4. Monitoring and Debugging
- Loss curves
- Perplexity tracking
- Sample generation during training
- Overfitting detection

---

## ✅ Tasks

1. **Prepare Dataset**
   - Choose text corpus
   - Tokenize with BPE
   - Create dataloaders

2. **Configure Training**
   - Set hyperparameters
   - Implement gradient accumulation
   - Add learning rate scheduler

3. **Train Model**
   - Train small GPT (6-12 layers)
   - Monitor metrics
   - Save checkpoints

4. **Evaluation**
   - Calculate test perplexity
   - Generate text samples
   - Compare with baseline

---

## 💡 Stretch Goals (Optional)
- Implement mixed precision training
- Try gradient checkpointing
- Experiment with learning rate schedules
- Study loss spike recovery
