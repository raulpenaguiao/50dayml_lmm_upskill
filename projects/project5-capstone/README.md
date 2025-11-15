# Project 5: Capstone Project

## Overview
Choose one of three capstone project options to demonstrate mastery of ML/LLM engineering concepts.

---

## Option 1: RAG-Powered Chatbot

### Description
Build an intelligent chatbot that can answer questions based on a custom knowledge base using Retrieval-Augmented Generation.

### Key Features
- Document ingestion (PDF, TXT, MD, etc.)
- Vector store (FAISS or ChromaDB)
- Semantic search and retrieval
- LLM-based answer generation
- Source attribution
- Conversational memory
- Web interface (Gradio/Streamlit)

### Tech Stack
- Hugging Face Transformers
- sentence-transformers
- FAISS/ChromaDB
- LangChain (optional)
- Gradio or Streamlit

### Success Criteria
- [ ] Ingests and indexes documents
- [ ] Retrieves relevant context
- [ ] Generates accurate answers
- [ ] Provides source citations
- [ ] User-friendly interface
- [ ] Handles multi-turn conversations

---

## Option 2: Document Classification Pipeline

### Description
Build a complete document classification system with advanced features and production deployment.

### Key Features
- Multi-class or multi-label classification
- Fine-tuned BERT/DistilBERT with LoRA
- REST API with FastAPI
- Batch processing support
- Model monitoring and versioning
- Docker deployment
- MLflow tracking
- Automated retraining pipeline

### Tech Stack
- PyTorch + Hugging Face
- FastAPI
- Docker
- MLflow
- PostgreSQL (optional for logging)

### Success Criteria
- [ ] >92% test accuracy
- [ ] Production-ready API
- [ ] Comprehensive MLOps
- [ ] Scalable architecture
- [ ] Monitoring and alerting
- [ ] Complete documentation

---

## Option 3: Domain-Specific LLM with LoRA

### Description
Fine-tune a small language model (GPT-2, GPT-J, or Llama) on a specific domain using LoRA.

### Key Features
- LoRA fine-tuning on domain data
- Custom dataset preparation
- Comprehensive evaluation suite
- Multiple generation strategies
- Model comparison (base vs fine-tuned)
- Deployment-ready inference
- API or web interface

### Tech Stack
- Hugging Face Transformers
- PEFT (LoRA)
- FastAPI or Gradio
- Docker

### Success Criteria
- [ ] Successfully fine-tuned LLM
- [ ] Demonstrates domain expertise
- [ ] Comprehensive evaluation
- [ ] Quality generation samples
- [ ] Efficient inference
- [ ] Professional documentation

---

## General Requirements (All Options)

### Code Quality
- Clean, modular code
- Type hints
- Comprehensive docstrings
- Unit tests
- Integration tests

### Documentation
- Detailed README
- API documentation
- Architecture diagram
- Setup instructions
- Usage examples

### Deployment
- Docker containerization
- docker-compose setup
- Environment configuration
- Deployment guide

### Presentation
- Project overview slides
- Live demo
- Results and metrics
- Lessons learned

---

## Project Structure (Template)
```
project5-capstone/
├── data/                 # Datasets and artifacts
├── models/              # Saved models
├── notebooks/           # Jupyter notebooks
├── src/
│   ├── data/           # Data processing
│   ├── models/         # Model code
│   ├── api/            # API code (if applicable)
│   └── utils/          # Utilities
├── tests/              # Test suite
├── deployment/         # Deployment configs
├── docs/               # Documentation
├── Dockerfile
├── docker-compose.yml
├── requirements.txt
└── README.md
```

---

## Timeline

### Day 47: Planning
- Choose project option
- Define scope and requirements
- Design architecture
- Setup infrastructure

### Day 48: Implementation Part 1
- Core functionality
- Data pipeline
- Model setup
- Initial testing

### Day 49: Implementation Part 2
- Complete features
- API/Interface development
- Testing and validation
- Documentation

### Day 50: Finalization
- Polish and bug fixes
- Create presentation
- Record demo
- Portfolio preparation

---

## Evaluation Criteria

### Technical Excellence (40%)
- Code quality and architecture
- Model performance
- System design
- Testing coverage

### Functionality (30%)
- Feature completeness
- User experience
- Reliability
- Scalability

### Documentation (20%)
- README clarity
- Code documentation
- API docs
- Deployment guide

### Presentation (10%)
- Demo quality
- Problem explanation
- Results communication
- Professional polish

---

## Resources

### Datasets
- **RAG Option**: Wikipedia, arXiv papers, company docs
- **Classification**: IMDb, AG News, 20 Newsgroups, custom
- **LLM Fine-tuning**: Code datasets, domain-specific text

### Pretrained Models
- BERT family (bert-base, distilbert)
- GPT family (gpt2, gpt-j)
- Sentence transformers (all-MiniLM-L6-v2)
- T5, BART for generation tasks

### Tools and Libraries
- Hugging Face: transformers, datasets, peft
- Vector DBs: FAISS, ChromaDB, Pinecone
- LLM frameworks: LangChain, LlamaIndex
- APIs: FastAPI, Gradio, Streamlit

---

## Getting Started

1. **Choose your project** based on:
   - Interest and passion
   - Career goals
   - Available resources
   - Time constraints

2. **Plan thoroughly**:
   - Define clear objectives
   - Break down into milestones
   - Identify risks
   - Allocate time wisely

3. **Start building**:
   - Begin with core functionality
   - Iterate quickly
   - Test continuously
   - Document as you go

4. **Polish for portfolio**:
   - Clean up code
   - Comprehensive README
   - Professional presentation
   - Showcase best work

---

## Support and Resources
- Review previous project READMEs
- Reference course materials
- Consult Hugging Face docs
- Engage with ML community

**Good luck with your capstone project!**
