# Project 4: Production-Ready Text Classification System

## Overview
Build an end-to-end text classification system using fine-tuned BERT/DistilBERT with production deployment via FastAPI, Docker, and MLflow tracking.

## Goals
- Fine-tune pretrained transformer for classification
- Build production-ready REST API
- Containerize application with Docker
- Implement MLOps best practices
- Deploy-ready system

## Requirements

### Model Development
- Fine-tune BERT or DistilBERT
- Use LoRA for parameter efficiency
- Hugging Face Trainer API
- MLflow experiment tracking
- Achieve >90% test accuracy

### Evaluation
- Comprehensive metrics (accuracy, F1, precision, recall)
- Confusion matrix
- Per-class analysis
- Error analysis
- Comparison with baseline

### API Development
FastAPI application with endpoints:
- `POST /predict` - Single prediction
- `POST /predict_batch` - Batch predictions
- `GET /health` - Health check
- `GET /metrics` - Model metrics

Features:
- Input validation (Pydantic)
- Error handling
- Request logging
- API documentation (Swagger)

### Containerization
- Optimized Dockerfile
- Docker Compose setup
- Volume management
- Environment variables

### MLOps
- Experiment tracking with MLflow
- Model versioning
- Metrics logging
- Model registry

## Project Structure
```
project4-text-classification/
├── data/
│   ├── raw/              # Original data
│   └── processed/        # Preprocessed data
├── models/
│   └── checkpoints/      # Model checkpoints
├── notebooks/
│   ├── 01_eda.ipynb
│   ├── 02_training.ipynb
│   └── 03_evaluation.ipynb
├── src/
│   ├── api/
│   │   ├── main.py       # FastAPI app
│   │   ├── models.py     # Pydantic models
│   │   └── predict.py    # Prediction logic
│   ├── data/
│   │   └── preprocessing.py
│   ├── models/
│   │   ├── model.py      # Model definition
│   │   └── train.py      # Training script
│   └── utils/
│       └── metrics.py
├── tests/
│   ├── test_api.py
│   └── test_model.py
├── mlruns/               # MLflow artifacts
├── Dockerfile
├── docker-compose.yml
├── requirements.txt
├── .env.example
└── README.md
```

## API Example

### Request
```bash
curl -X POST "http://localhost:8000/predict" \
     -H "Content-Type: application/json" \
     -d '{"text": "This movie was amazing!"}'
```

### Response
```json
{
    "prediction": "positive",
    "confidence": 0.95,
    "probabilities": {
        "positive": 0.95,
        "negative": 0.05
    }
}
```

## Docker Usage
```bash
# Build image
docker build -t text-classifier .

# Run container
docker run -p 8000:8000 text-classifier

# Or use docker-compose
docker-compose up
```

## MLflow Tracking
```bash
# Start MLflow UI
mlflow ui

# View at http://localhost:5000
```

## Success Criteria
- [ ] Model achieves >90% test accuracy
- [ ] API is production-ready and documented
- [ ] Fully containerized and deployable
- [ ] MLflow tracking implemented
- [ ] Comprehensive testing
- [ ] Clean, professional code
- [ ] Complete documentation

## Technical Stack
- **Framework**: PyTorch + Hugging Face Transformers
- **API**: FastAPI
- **Containerization**: Docker
- **Tracking**: MLflow
- **Testing**: pytest
- **Model**: BERT-base or DistilBERT

## Getting Started
1. Install dependencies: `pip install -r requirements.txt`
2. Prepare data: `python src/data/preprocessing.py`
3. Train model: `python src/models/train.py`
4. Start API: `uvicorn src.api.main:app --reload`
5. View docs: `http://localhost:8000/docs`

## Deployment
See `deployment/` directory for:
- Cloud deployment guides (AWS, GCP, Azure)
- Kubernetes configurations
- CI/CD pipeline examples

## Related Days
- Day 31-33: Hugging Face and fine-tuning
- Day 36: FastAPI deployment
- Day 37: Docker containerization
- Day 38: MLflow tracking
- Day 39: ML pipelines
- Day 40: Project completion
