# Day 6: Transfer Learning and Pretrained Models

## 🎯 Goal
Learn to leverage pretrained models and transfer learning to solve computer vision tasks efficiently.

---

## 📚 Topics Covered
- Transfer learning concepts
- Using pretrained models (ResNet, VGG, MobileNet)
- Feature extraction vs fine-tuning
- Working with different datasets (CIFAR-10)
- Domain adaptation

---

## 📝 Syllabus

### 1. Transfer Learning Fundamentals
- Why transfer learning works
- Feature extraction approach
- Fine-tuning approach
- When to use each strategy

### 2. Pretrained Models
- Load ResNet18/34 from torchvision
- Understanding model architecture
- Freezing and unfreezing layers
- Replacing classification head

### 3. CIFAR-10 Dataset
- Load and explore CIFAR-10
- Data preprocessing for pretrained models
- Handle different input sizes
- Class imbalance considerations

### 4. Training Strategies
- Feature extraction first, then fine-tuning
- Differential learning rates
- Gradual unfreezing
- Performance comparison

---

## ✅ Tasks

1. **Load Pretrained Model**
   - Load ResNet18 with ImageNet weights
   - Freeze convolutional layers
   - Replace final layer for CIFAR-10

2. **Feature Extraction**
   - Train only the final layer
   - Evaluate performance
   - Analyze training time

3. **Fine-Tuning**
   - Unfreeze later layers
   - Train with lower learning rate
   - Compare with feature extraction

4. **Evaluation**
   - Compute accuracy on CIFAR-10
   - Create confusion matrix
   - Analyze misclassifications

---

## 💡 Stretch Goals (Optional)
- Try different architectures (VGG, MobileNet, EfficientNet)
- Implement gradual unfreezing strategy
- Use differential learning rates per layer
- Apply to custom dataset
