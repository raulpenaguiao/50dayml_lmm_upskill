# Day 2: Convolutional Neural Networks for Image Classification

## 🎯 Goal
Understand and implement a basic Convolutional Neural Network (CNN) in PyTorch for image classification on the MNIST dataset.
Learn how CNNs improve performance over simple MLPs for image data.

**Mathematical Focus:** Understand convolution as a linear operator, receptive fields, and parameter sharing. You should be comfortable with convolution from signal processing or PDEs.

**Time estimate:** 3-4 hours

---

## 📚 Topics Covered
- What is a Convolutional Neural Network (CNN)?
- CNN architecture: convolutional layers, activation functions, pooling layers, fully connected layers
- PyTorch modules for CNNs (`nn.Conv2d`, `nn.MaxPool2d`, `nn.ReLU`, `nn.Flatten`, `nn.Linear`)
- Training and evaluating a CNN on MNIST
- Comparing CNN vs MLP performance

---

## 📝 Syllabus

### 1. Introduction to CNNs
- Motivation for CNNs in image tasks
- Key differences between CNNs and MLPs

### 2. Building a CNN in PyTorch
- Define a simple CNN architecture:
  - 1–2 convolutional layers with ReLU
  - Max pooling
  - Flatten and fully connected output layer
- Print model summary

### 3. Training Loop
- Use `nn.CrossEntropyLoss` for classification
- Optimizer: `Adam` or `SGD`
- Train for 2–3 epochs
- Track loss and accuracy

### 4. Evaluation
- Compute test accuracy
- Visualize predictions for 10 test samples
- Display confusion matrix

### 5. Comparison & Discussion
- Compare CNN results to MLP from Day 1
- Discuss why CNNs perform better on images

---

## ✅ Tasks

1. **Model Implementation**
   - Implement a simple CNN in PyTorch
   - Print model architecture

2. **Training**
   - Train the CNN for 2–3 epochs
   - Log training loss and accuracy

3. **Evaluation**
   - Compute and print test accuracy
   - Visualize predictions vs ground truth for 10 samples
   - Display confusion matrix

4. **Analysis**
   - Compare CNN and MLP results
   - Write a short reflection on CNN advantages

---

## 📚 Study Material
- `day02_syllabus.md` (this file)
- `day02_notebook.ipynb` with:
  - CNN model code
  - Training and evaluation loop
  - Accuracy and confusion matrix
  - Sample predictions

- PyTorch documentation: [https://pytorch.org/docs/stable/nn.html](https://pytorch.org/docs/stable/nn.html)
- Recommended reading:  
  - [CS231n Convolutional Neural Networks](https://cs231n.github.io/convolutional-networks/)

---

## 💡 Stretch Goals (Optional)
- Add more convolutional layers or experiment with kernel sizes
- Try different optimizers or learning rates
- Visualize feature maps from the first convolutional layer
- Apply the CNN to another dataset