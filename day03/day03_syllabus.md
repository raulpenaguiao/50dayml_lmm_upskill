# Day 3: Advanced CNNs and Data Augmentation

## 🎯 Goal
Learn about advanced CNN architectures and techniques to improve model performance through data augmentation and regularization.

**Mathematical Focus:** Batch normalization (normalization as affine transformation), dropout (stochastic regularization), learning rate schedules (optimization theory).

**Time estimate:** 3-4 hours

---

## 📚 Topics Covered
- Data augmentation techniques (rotation, flipping, cropping)
- Batch normalization
- Dropout for regularization
- Learning rate scheduling
- Model checkpointing and saving

---

## 📝 Syllabus

### 1. Data Augmentation
- Understanding why data augmentation helps
- Implementing transforms: rotation, flipping, random crops
- Using `torchvision.transforms` for augmentation
- Impact on model generalization

### 2. Advanced Training Techniques
- Batch normalization layers
- Dropout strategies
- Learning rate schedulers (StepLR, ReduceLROnPlateau)
- Early stopping

### 3. Model Persistence
- Saving and loading models
- Checkpoint management
- Best practices for model serialization

---

## ✅ Tasks

1. **Data Augmentation**
   - Implement augmentation pipeline
   - Train CNN with and without augmentation
   - Compare results

2. **Batch Normalization**
   - Add batch norm layers to CNN
   - Observe training stability improvements

3. **Learning Rate Scheduling**
   - Implement learning rate decay
   - Monitor training dynamics

4. **Save Best Model**
   - Implement model checkpointing
   - Save the best performing model

---

## 💡 Stretch Goals (Optional)
- Implement custom augmentation functions
- Try mixup or cutout augmentation
- Experiment with different batch sizes
- Plot learning rate vs accuracy curves
