# Course Overview: ML/LLM 50-Day Upskill Course

## 📌 Target Audience

**This course is ONLY for people with:**
- ✅ Master's degree or PhD in quantitative field (Math, Physics, CS, Engineering, Statistics)
- ✅ Strong linear algebra (eigenvalues, SVD, matrix calculus)
- ✅ Multivariable calculus (gradients, Jacobians, chain rule)
- ✅ Probability & Statistics (distributions, Bayes theorem, MLE)
- ✅ Optimization theory (gradient descent, convex optimization)
- ✅ Proficient Python programming

**NOT suitable for:**
- ❌ Beginners in mathematics
- ❌ Self-taught programmers without formal math background
- ❌ People expecting basic explanations of calculus/linear algebra

---

## ⏱️ Realistic Time Commitment

**Originally advertised:** 2 hours/day × 50 days = 100 hours
**Actual requirement:** 3-4 hours/day × 50 days = 150-200 hours

### Time Breakdown by Day Type:
- **Lecture days** (Days 1-9, 11-19, 21-29, 31-39, 41-46): 3-4 hours
- **Implementation-heavy days** (Days 5, 10, 20, 30, 40): 4-5 hours
- **Project days** (Days 10, 20, 30, 40, 47-50): 5-6 hours

**Recommendation:** Block out **4 hours per day** to complete comfortably without rushing.

---

## 📚 What You'll Learn

### Phase 1: Foundations (Days 1-10)
**Focus:** PyTorch, CNNs, optimization, from-scratch implementations

**Key Days:**
- **Day 1**: PyTorch basics, first neural network (assumes you know backprop math)
- **Day 2**: CNNs (assumes you know convolution from signal processing)
- **Day 3**: Data augmentation, batch norm, regularization
- **Day 4**: Advanced optimizers (Adam, RMSprop), gradient dynamics
- **Day 5**: Implement NN from scratch in NumPy (4-5 hours, substantial)
- **Day 6**: Transfer learning
- **Day 7**: Evaluation metrics
- **Day 8**: Hyperparameter tuning
- **Day 9**: ResNet, VGG architectures
- **Day 10**: **Project 1** - MNIST with custom architecture

**Math Level:** Graduate optimization, numerical linear algebra
**Time:** 35-40 hours total

---

### Phase 2: Deep Learning & NLP (Days 11-20)
**Focus:** NLP fundamentals, RNNs, LSTMs, attention

**Key Days:**
- **Day 11**: NLP preprocessing, tokenization
- **Day 12**: Word embeddings (Word2Vec, GloVe)
- **Day 13**: RNNs for sequences
- **Day 14**: LSTMs and GRUs
- **Day 15**: Seq2seq models
- **Day 16**: Attention mechanisms (foundational for Transformers)
- **Day 17**: Introduction to Transformers
- **Day 18**: Text classification
- **Day 19**: Character-level language models
- **Day 20**: **Project 2** - Character-level RNN text generation

**Math Level:** Sequence modeling, dynamic programming concepts
**Time:** 35-40 hours total

---

### Phase 3: Transformers & LLM Foundations (Days 21-30)
**Focus:** Transformer architecture, GPT, BERT, training LLMs

**Key Days:**
- **Day 21**: Transformer encoder (self-attention, layer norm)
- **Day 22**: Transformer decoder (masked attention, cross-attention)
- **Day 23**: Tokenization (BPE, WordPiece)
- **Day 24**: GPT architecture (decoder-only)
- **Day 25**: Training GPT from scratch
- **Day 26**: BERT (encoder-only, masked language modeling)
- **Day 27**: Karpathy's minGPT code walkthrough
- **Day 28**: Training minGPT on Shakespeare
- **Day 29**: Advanced training techniques
- **Day 30**: **Project 3** - minGPT Shakespeare (major project)

**Math Level:** Attention as matrix operations, softmax numerics
**Time:** 40-45 hours total (most substantial phase)

---

### Phase 4: Modern ML/LLM Engineering (Days 31-40)
**Focus:** Hugging Face, fine-tuning, LoRA, deployment, MLOps

**Key Days:**
- **Day 31**: Hugging Face Transformers library
- **Day 32**: Fine-tuning BERT
- **Day 33**: LoRA and PEFT (parameter-efficient fine-tuning)
- **Day 34**: Working with large LLMs
- **Day 35**: NLP evaluation metrics (BLEU, ROUGE, perplexity)
- **Day 36**: FastAPI deployment
- **Day 37**: Docker containerization
- **Day 38**: MLflow experiment tracking
- **Day 39**: Complete ML pipelines
- **Day 40**: **Project 4** - Production text classification API

**Math Level:** Less math-intensive, more engineering
**Time:** 35-40 hours total

---

### Phase 5: Advanced Topics & Capstone (Days 41-50)
**Focus:** RAG, prompt engineering, safety, capstone project

**Key Days:**
- **Day 41**: RAG introduction
- **Day 42**: Document Q&A with RAG
- **Day 43**: Prompt engineering
- **Day 44**: LLM safety and evaluation
- **Day 45**: Training optimization (mixed precision, Flash Attention)
- **Day 46**: LangChain framework
- **Day 47**: Capstone planning
- **Day 48-49**: Capstone implementation
- **Day 50**: **Project 5** - Capstone presentation

**Math Level:** Varies by capstone choice
**Time:** 40-50 hours total (capstone is intensive)

---

## 🎯 Summary: Days 1-3

### **Day 1: Building Your First Neural Network in PyTorch**
**Time:** 3-4 hours

**What you'll do:**
1. Set up PyTorch environment
2. Load MNIST dataset using torchvision
3. Build a 2-layer MLP (784 → 128 → 10)
4. Implement complete training loop from scratch
5. Achieve ~73-93% accuracy
6. Visualize predictions and confusion matrix
7. Experiment with different optimizers (SGD, Adam)
8. Try adding layers and comparing results

**Mathematical assumptions:**
- You already understand gradient descent
- You know what backpropagation is (chain rule)
- You understand cross-entropy loss
- Focus is on PyTorch implementation, NOT theory

**Key skills:**
- PyTorch tensors and autograd
- `nn.Module` architecture
- Training loop structure
- Data loading with DataLoader

---

### **Day 2: Convolutional Neural Networks**
**Time:** 3-4 hours

**What you'll do:**
1. Understand CNN motivation (spatial structure)
2. Implement CNN with:
   - 2 conv layers (1→32→64 channels)
   - Max pooling
   - Fully connected layers
   - Dropout
3. Train on MNIST
4. Achieve ~98% accuracy (vs ~88% for MLP)
5. Visualize learned filters
6. Create comprehensive evaluation
7. Compare CNN vs MLP performance

**Mathematical assumptions:**
- You understand convolution from signal processing or PDEs
- You know what a linear operator is
- You understand parameter sharing
- Focus is on why CNNs work for images

**Key skills:**
- `nn.Conv2d`, `nn.MaxPool2d`
- Understanding receptive fields
- Feature map visualization
- Architectural design choices

---

### **Day 3: Advanced CNNs and Data Augmentation**
**Time:** 3-4 hours

**What you'll do:**
1. Implement data augmentation:
   - Random rotations, flips, crops
   - Using `torchvision.transforms`
2. Add batch normalization to CNN
3. Experiment with dropout rates
4. Implement learning rate scheduling:
   - StepLR
   - ReduceLROnPlateau
5. Model checkpointing (save best model)
6. Compare augmented vs non-augmented training
7. Analyze training stability with batch norm

**Mathematical assumptions:**
- You understand normalization and standardization
- You know why stochastic regularization helps (dropout)
- You understand learning rate schedules from optimization theory
- Focus is on practical improvements

**Key skills:**
- Data augmentation pipelines
- Batch normalization implementation
- Learning rate schedulers
- Model persistence (save/load)
- Training monitoring

---

## 📊 Mathematical Prerequisites by Phase

### Phase 1 (Days 1-10)
**Required Math:**
- Matrix multiplication and derivatives
- Chain rule for multivariable functions
- Gradient descent and convex optimization
- Basic probability (distributions)
- Numerical methods (stability, convergence)

**You'll implement:**
- Backpropagation from scratch
- Various optimizers (SGD, Adam)
- Neural networks in pure NumPy
- Gradient checking

---

### Phase 2 (Days 11-20)
**Required Math:**
- Sequence models and dynamic programming
- Probability (conditional distributions)
- Information theory basics (entropy, KL divergence)
- Time series concepts

**You'll implement:**
- RNNs, LSTMs, GRUs
- Seq2seq models
- Attention mechanisms
- Character-level language models

---

### Phase 3 (Days 21-30)
**Required Math:**
- Softmax and log-softmax numerics
- Matrix operations for attention
- Positional encodings (sinusoidal functions)
- Optimization for large models

**You'll implement:**
- Complete Transformer from scratch
- Self-attention mechanism
- GPT architecture
- Training loop for language models

---

### Phase 4-5 (Days 31-50)
**Required Math:**
- Less math-heavy (more engineering)
- Vector embeddings and similarity metrics
- Evaluation metrics theory
- Some optimization for efficiency

**You'll implement:**
- Fine-tuning pipelines
- RAG systems
- Production APIs
- Complete ML systems

---

## ✅ Success Criteria

By the end of this course, you should be able to:

1. **Implement from scratch:**
   - ✅ Neural networks in NumPy
   - ✅ CNN architectures
   - ✅ Transformer architecture
   - ✅ GPT-style language models

2. **Use modern tools:**
   - ✅ PyTorch for deep learning
   - ✅ Hugging Face Transformers
   - ✅ Docker for deployment
   - ✅ MLflow for experiment tracking

3. **Build complete systems:**
   - ✅ End-to-end ML pipelines
   - ✅ REST APIs for model serving
   - ✅ RAG-based Q&A systems
   - ✅ Production-ready deployments

4. **Understand deeply:**
   - ✅ How backpropagation works (you implemented it)
   - ✅ Why Transformers replaced RNNs
   - ✅ How attention mechanisms work mathematically
   - ✅ Trade-offs in model design and optimization

---

## 🚨 Common Pitfalls

1. **Underestimating time**: Budget 4 hours/day, not 2
2. **Skipping mathematical understanding**: Don't just copy code
3. **Not doing projects thoroughly**: Projects are 30% of learning
4. **Rushing through Phase 1**: Strong foundation is critical
5. **Skipping from-scratch implementations**: These build deep understanding

---

## 💡 Study Tips for People with Strong Math Backgrounds

1. **Derive before implementing**: Use your math skills to derive gradients before coding
2. **Numerical validation**: Always check analytical vs numerical gradients
3. **Read papers**: Original Transformer paper, ResNet paper, GPT papers
4. **Connect to theory**: Relate DL to optimization, numerical methods you know
5. **Question everything**: Your math background lets you understand WHY, not just HOW
6. **Implement variants**: Once you understand something, try variations
7. **Profile and optimize**: Use your computational complexity knowledge

---

## 📖 Recommended Supplementary Reading

- **Deep Learning** by Goodfellow, Bengio, Courville (theoretical foundation)
- **Pattern Recognition and Machine Learning** by Bishop (Bayesian perspective)
- **Attention is All You Need** (Vaswani et al., 2017) - Original Transformer paper
- **Deep Residual Learning** (He et al., 2015) - ResNet paper
- CS231n lecture notes (Stanford - computer vision)
- CS224n lecture notes (Stanford - NLP)
- **The Annotated Transformer** - Practical walkthrough

---

## 🎓 What This Course Prepares You For

**Job Titles:**
- ML Engineer (mid-level)
- LLM Engineer
- Research Engineer
- Applied Scientist (at some companies)
- Deep Learning Engineer

**Skills Demonstrated:**
- Strong mathematical foundations + implementation
- Modern deep learning frameworks
- Production deployment skills
- End-to-end project experience
- Research to production pipeline

**Salary Range (2024):**
- Entry-level: $120k-150k (despite math background, you're new to ML)
- With projects: $140k-180k
- After 1-2 years experience: $180k-250k+

**Companies:**
- Tech companies (Google, Meta, Microsoft, Amazon)
- AI startups (OpenAI, Anthropic, Cohere, etc.)
- Finance (quant ML roles)
- Research labs

---

**Ready to start? Begin with Day 1 and leverage your mathematical background to move quickly through fundamentals!**
