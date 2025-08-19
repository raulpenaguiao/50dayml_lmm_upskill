
# Day 1: Building Your First Neural Network in PyTorch

## 🎯 Goal
Jump straight into building and training a simple neural network using PyTorch to classify handwritten digits from the MNIST dataset.  
The focus is on hands-on learning by coding, running, and experimenting.

---

## 📚 Topics Covered
- PyTorch basics: Tensors, datasets, dataloaders
- Defining a simple feedforward neural network (MLP)
- Training loop (forward pass, loss calculation, backpropagation, optimizer step)
- Evaluating model performance

---

## 📝 Syllabus

### 1. Setup & Warm-up
- Install/verify environment: Python, PyTorch, Jupyter/VSCode
- Import core libraries: `torch`, `torchvision`, `matplotlib`

### 2. Data Loading
- Use `torchvision.datasets.MNIST` to load data
- Apply transforms: tensor conversion, normalization
- Create `DataLoader` objects for training and testing

### 3. Build the Model
- Define a simple 2-layer MLP in PyTorch using `nn.Module`
- Input: 28x28 pixels → Flatten to 784
- Hidden Layer: 128 neurons + ReLU
- Output Layer: 10 classes (digits 0–9)

### 4. Training Loop
- Loss function: `nn.CrossEntropyLoss`
- Optimizer: `torch.optim.SGD` or `Adam`
- Train for 2–3 epochs on MNIST
- Track accuracy

### 5. Evaluation
- Evaluate on test dataset
- Print accuracy and visualize predictions for some samples

---

## ✅ Tasks

1. **Setup & Dataset**
   - Load MNIST dataset with `torchvision`
   - Print dataset size and visualize first 5 samples

2. **Model Implementation**
   - Implement a simple MLP in `nn.Module`
   - Print model summary

3. **Training Loop**
   - Write code for forward pass, loss computation, backward pass, and optimizer update
   - Train for 2 epochs, log loss

4. **Evaluation**
   - Compute test accuracy
   - Visualize predictions vs ground truth for 10 test samples

---

## 🎁 Deliverables
- `day01_syllabus.md` file with this syllabus
- 
- `day1_mnist_nn.ipynb` notebook with:
  - Data loading and visualization
  - Model definition and training loop
  - Test accuracy result
  - Sample predictions with labels
- Short README section (in notebook or repo) describing:
  - The model architecture
  - Training performance (loss curve + accuracy)
  - Key learnings from Day 1

---

## 💡 Stretch Goals (Optional)
- Add a second hidden layer
- Try different optimizers (SGD vs Adam)
- Train for more epochs and compare accuracy
