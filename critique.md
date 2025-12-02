# Course Critique: Days 1-50

## Overview

This document provides critical feedback on the course materials, identifying strengths, weaknesses, gaps, and areas for improvement. Organized by day/phase, with actionable recommendations.

---

## Phase 1: Foundations of ML & Deep Learning (Days 1-10)

### Day 01: Building First Neural Network in PyTorch

**Strengths:**
- ✅ Excellent entry point with hands-on MNIST classification
- ✅ Good coverage of reproducibility (random seeds)
- ✅ Clear explanation of data loading and preprocessing
- ✅ Multiple model variants tested (2-layer vs deeper, different optimizers)
- ✅ Includes model saving/loading (practical skill)
- ✅ Confusion matrix visualization for deeper analysis

**Weaknesses & Gaps:**
- ❌ **No learning rate justification**: Why lr=0.001? No ablation study
- ❌ **Missing key concepts**:
  - No explanation of why Adam optimizer works better than SGD (just shows results)
  - No discussion of loss curves (overfitting vs underfitting)
  - No learning rate schedule mentioned
- ❌ **Poor accuracy analysis**:
  - The 4-epoch model has LOWER accuracy (88.85%) than 2-epoch (95.21%) - this is suspicious and suggests overfitting or a bug. Not addressed.
  - No learning curves shown to diagnose this
- ❌ **Dataset split not mentioned**: No validation set, only train/test
- ❌ **Batch size choice unexplained**: Why 64 for training, 1000 for testing?
- ⚠️ **Limited experiment scope**: Only 2 epochs due to time. Real training needs more epochs to see convergence

**What's Missing:**
1. Learning rate sensitivity analysis
2. Batch size effects on training
3. Discussion of train/val/test split
4. Explanation of why some optimizers underperform
5. Initialization strategies (Xavier vs random)
6. Regularization concepts (no L2, no dropout yet)

**Actionable Improvements:**
- Add section on learning rate selection with visualization
- Include learning curves (loss vs epoch) to show convergence
- Explain the accuracy drop with more epochs - debug this
- Add validation curve alongside training curve
- Include time complexity discussion (why is it slow?)

---

### Day 02: Convolutional Neural Networks

**Strengths:**
- ✅ Clear CNN architecture explanation
- ✅ Good visual motivation for CNNs (preserving spatial structure)
- ✅ Implements a reasonable CNN architecture
- ✅ Shows training curves and per-class accuracy
- ✅ Includes confusion matrix
- ✅ Bonus: Visualizes learned filters (excellent!)
- ✅ Stretch goals provided for further exploration

**Weaknesses & Gaps:**
- ❌ **No comparison with Day 1 MLP**: Should highlight accuracy improvement quantitatively
- ❌ **Missing parameter counts**: Not comparing model complexity (parameters) vs accuracy
- ❌ **Pooling not explained mathematically**:
  - Max pooling formula not shown
  - Why 2x2? Why max instead of average?
  - No discussion of receptive fields
- ❌ **Architecture choices unjustified**:
  - Why 32 and 64 filters? How would you choose?
  - Why 3x3 kernels? What about 5x5 or 7x7?
  - Dropout=0.5 but Day 3 will show this is important - should mention regularization
- ❌ **Limited scope**: Only 3 epochs. Doesn't show potential for higher accuracy
- ❌ **No discussion of overfitting**: Model seems to fit well but no train vs test comparison shown clearly

**What's Missing:**
1. Mathematical formulation of convolution and pooling
2. Receptive field analysis
3. Comparison with MLP baseline
4. Parameter count comparison
5. Ablation studies (what happens without pooling? with different filter sizes?)
6. Discussion of modern alternatives (average pooling, stride, dilated conv)

**Actionable Improvements:**
- Add formula for 2D convolution
- Show receptive field visualization
- Create table comparing Day 1 MLP vs Day 2 CNN on:
  - Test accuracy
  - Number of parameters
  - Training time per epoch
- Experiment with different pooling strategies
- Include longer training to show potential for 99%+ accuracy

---

### Day 03: Advanced CNNs and Data Augmentation

**Strengths:**
- ✅ Excellent theory section with mathematical formulations
- ✅ Clear motivation for batch norm, dropout, augmentation
- ✅ Implements augmentation with visualization
- ✅ Compares augmented vs non-augmented training
- ✅ Tests different dropout rates systematically
- ✅ Learning rate scheduling included
- ✅ Model checkpointing for best model
- ✅ Well-structured experiments

**Weaknesses & Gaps:**
- ❌ **Results interpretation missing**:
  - Augmentation shows improvement but analysis is shallow
  - Why does augmented data help so much?
  - When would augmentation hurt?
- ❌ **Batch norm placement unclear**:
  - Applied after conv, before ReLU (standard)
  - But exercise asks "before or after ReLU?" - this should be discussed
  - No experiment comparing both
- ❌ **Dropout experiment incomplete**:
  - Only 5 epochs - hard to see the regularization benefit
  - Dropout=0.7 should show more overfitting prevention
- ❌ **Learning rate schedule**:
  - StepLR with gamma=0.5 seems arbitrary
  - No justification or alternatives shown
- ❌ **Missing quantitative analysis**:
  - "Augmentation helps" - by how much exactly?
  - What's the effect on overfitting specifically?

**What's Missing:**
1. Comparison of augmentation types (rotation alone vs all transforms)
2. Effect of augmentation strength on convergence
3. Discussion of BatchNorm vs LayerNorm vs GroupNorm as exercise
4. Analysis of why batch size matters (see Day 8)
5. Training stability metrics (gradient norms)

**Actionable Improvements:**
- Add experiment: Compare augmentation types individually
- Create table showing final accuracy for each dropout rate with confidence intervals
- Show gap between train/test accuracy to quantify overfitting reduction from augmentation
- Explain why StepLR chosen (could mention ReduceLROnPlateau as alternative)
- Run experiments longer (10+ epochs) to better see regularization effects
- Add section on "when augmentation hurts" (e.g., with label-altering transforms)

---

### Day 04: Advanced Optimization and Gradient Dynamics

**Strengths:**
- ✅ Excellent mathematical foundation
- ✅ Implements 5 optimizers from scratch (educational!)
- ✅ Fair comparison with same learning rate
- ✅ Shows gradient norms evolution
- ✅ Loss landscape visualization (sophisticated!)
- ✅ Gradient flow analysis in deep networks
- ✅ Learning rate sensitivity study
- ✅ Clear summary of optimizer characteristics

**Weaknesses & Gaps:**
- ❌ **Custom implementations might have bugs**:
  - No verification that custom optimizers match PyTorch exactly
  - Could cause unfair comparisons
  - Should add numerical tests matching PyTorch outputs
- ❌ **Learning rate not optimized per optimizer**:
  - All use lr=0.01, but Adam typically uses 0.001
  - Makes SGD look worse than it is
  - Should either tune per-optimizer or acknowledge this
- ❌ **Gradient flow analysis is shallow**:
  - Shows that gradients vary by layer
  - But no fix proposed (e.g., batch norm in next section)
  - Doesn't explain why this is a problem
- ❌ **Loss landscape**:
  - 2D projection doesn't capture full picture
  - Random directions might not be meaningful
  - Could use "mode connectivity" or actual optimization trajectories
- ❌ **Missing important topics**:
  - No learning rate warmup
  - No gradient clipping
  - No weight decay vs L2 regularization distinction
  - No discussion of BatchNorm's effect on gradients

**What's Missing:**
1. Verification that custom optimizers match PyTorch
2. Per-optimizer learning rate tuning
3. Discussion of adaptive methods pros/cons for different problem types
4. Connection between gradient flow and batch norm (preview Day 3)
5. Analysis of why Adam converges faster
6. Second-order methods (L-BFGS mentioned but not shown)

**Actionable Improvements:**
- Add test: Compare custom Adam with torch.optim.Adam on same data
- Show learning rate tuning curves for each optimizer
- Explain the relationship between optimizer choice and learning rate
- Add diagram explaining "why momentum helps" more intuitively
- Include ReduceLROnPlateau schedule comparison
- For loss landscape: Show actual optimizer trajectories, not just random directions

---

### Day 05: Building Neural Networks from First Principles (NumPy)

**Strengths:**
- ✅ **Excellent pedagogical approach**: Understanding backprop deeply is crucial
- ✅ Clear mathematical foundation with formulas
- ✅ Implements complete working neural network with NumPy only
- ✅ Includes numerical gradient checking (essential!)
- ✅ Shows layer abstractions cleanly
- ✅ Achieves >90% accuracy validating implementation
- ✅ Side-by-side comparison with PyTorch
- ✅ Identifies vanishing gradient problem

**Weaknesses & Gaps:**
- ❌ **Gradient checking is incomplete**:
  - Only checks first 10 elements of each layer (for speed)
  - Should check systematically or use proper sampling
  - Could miss bugs in specific parts of the layer
- ❌ **BatchNorm left as exercise but not shown**:
  - Exercise says "implement BatchNorm" but it's not completed
  - Learner has no reference for the answer
  - This is a significant gap for Days 6-10
- ❌ **Performance comparison is unfair**:
  - NumPy runs on CPU, PyTorch on CPU (should specify)
  - But doesn't discuss GPU comparison
  - Training time difference is dramatic but causes not analyzed
- ❌ **Initialization strategy under-discussed**:
  - Xavier init mentioned but not compared with random
  - No discussion of other strategies (He, Lecun)
  - Important for convergence but glossed over
- ❌ **Numerical stability**:
  - Log-sum-exp trick explained but not proven
  - No discussion of other stability issues
  - Clipping in sigmoid mentioned but not justified

**What's Missing:**
1. Completed BatchNorm implementation (or provide answer)
2. Dropout layer implementation
3. Convolutional layer (im2col trick)
4. Weight decay / L2 regularization
5. Discussion of why NumPy is slow (memory layout, BLAS calls)
6. Second-order derivative (Hessian) for analysis
7. Gradient clipping implementation

**Actionable Improvements:**
- Complete BatchNorm implementation with explanation
- Add section on computational complexity (FLOPs)
- Implement Dropout to show it's simple
- Provide reference implementation of Conv layer
- Compare different initialization schemes with ablation study
- Add profiling code showing where time is spent
- Discuss numerical stability issues beyond log-sum-exp

---

### Day 06: Transfer Learning and Pretrained Models

**Status:** Only syllabus/reading materials provided (no notebook yet)

**Expected Content Based on Syllabus:**
- Loading pretrained models (ImageNet-pretrained ResNet, VGG)
- Fine-tuning strategies
- Feature extraction vs end-to-end fine-tuning
- Learning rate strategies for fine-tuning
- Visualizing learned representations

**Critical Issues to Address When Implementing:**
- Need comparison: Fine-tuning vs training from scratch vs feature extraction
- Explain when each strategy is appropriate
- Show learning rate scheduling for fine-tuning (typically lower LR)
- Discuss dataset size dependency
- Include visualization of what different layers learn

---

### Day 07: Model Evaluation and Metrics

**Status:** Only syllabus/reading materials provided (no notebook yet)

**Expected Content Based on Syllabus:**
- Evaluation metrics: accuracy, precision, recall, F1, ROC-AUC
- Confusion matrix deep dive
- Class imbalance handling
- Cross-validation strategies
- Confidence intervals and statistical significance

**Critical Issues to Address When Implementing:**
- Metrics don't tell the whole story - need context about data distribution
- ROC curves vs precision-recall curves (when to use which)
- Difference between micro/macro averaging for multi-class
- Statistical tests for model comparison
- Should show why accuracy alone is insufficient

---

### Day 08: Hyperparameter Tuning and Experimentation

**Status:** Only syllabus/reading materials provided (no notebook yet)

**Expected Content Based on Syllabus:**
- Learning rate selection
- Batch size effects
- Number of layers/hidden units
- Regularization (dropout, L2, data augmentation)
- Systematic experimentation with grid/random search

**Critical Issues to Address When Implementing:**
- Batch size affects learning rate and generalization - important connection
- Learning rate is most impactful - should show sensitivity
- Tradeoffs between model capacity and generalization
- Computational cost of hyperparameter search
- Practical strategies (Bayesian optimization, population-based training)

---

### Day 09: Advanced CNN Architectures (ResNet, VGG)

**Status:** Only syllabus/reading materials provided (no notebook yet)

**Expected Content Based on Syllabus:**
- VGG: Deep stacking of 3x3 convolutions
- ResNet: Residual connections for very deep networks
- Batch normalization role in enabling deep networks
- Architecture comparisons

**Critical Issues to Address When Implementing:**
- Why residual connections work: Understanding the "identity shortcut"
- Difference between ResNet-50, ResNet-101, ResNet-152
- Comparison of test accuracy vs depth (increasing then plateauing)
- Skip connections not just for deep networks - used in modern architectures
- Bottleneck blocks explanation

---

### Day 10: Project 1 - MNIST Neural Network

**Status:** Only syllabus/reading materials provided (no notebook yet)

**Expected Content:**
- Capstone project bringing together Days 1-9
- Students implement MNIST classifier with best practices
- Should include: data loading, preprocessing, model architecture choices, training, evaluation, hyperparameter tuning

**Critical Issues for Project:**
- Need clear rubric for grading/self-evaluation
- Should emphasize reproducibility (seeds, version control)
- Encourage experiments and documentation
- Need baseline for comparison ("if you get >95% accuracy, you've done well")

---

## Cross-Phase Analysis: Days 1-10

### Major Strengths
1. **Excellent mathematical rigor**: Theory is precise with formulas
2. **Progressive complexity**: Starts simple, builds systematically
3. **Hands-on implementation**: Every concept has code
4. **Multiple perspectives**: NumPy (from first principles), PyTorch (modern), comparison
5. **Practical skills**: Saving models, visualizations, metrics

### Major Gaps
1. **Missing connections between days**:
   - Day 3 shows batch norm helps, but Day 4 doesn't use it or analyze gradient flow with it
   - Day 5 (NumPy) completes before Day 3/4 insights applied
   - Sequencing could be better

2. **Incomplete ablation studies**:
   - Often show results without explaining why
   - Limited systematic experiments (usually just one setup)
   - Should show train vs test curves to diagnose overfitting

3. **Hyperparameter choices unjustified**:
   - Learning rates, batch sizes, architecture choices seem arbitrary
   - No guidance on how learner should make these choices
   - Day 8 is only when this is systematically studied

4. **Missing failure cases**:
   - Always show successful training
   - Should show "what happens if you use lr=10?" or other mistakes
   - Debugging strategies not taught

5. **Limited scope**:
   - MNIST is too easy (>99% accuracy easily achievable)
   - Should progress to CIFAR-10 or CIFAR-100 for challenge
   - Real-world complexity not addressed

### Recommended Improvements

**Structure:**
- Reorder: Move Day 5 (NumPy) earlier, maybe after Day 1
- This gives foundation for understanding Days 2-4 better
- Days 2-4 could then be positioned as "advanced techniques for Day 1 model"

**Content:**
- Add "failure case" sections showing common mistakes
- Add learning curves (train/test) to every training loop
- Add ablation study templates for students to fill in
- Provide hyperparameter selection methodology, not just final values

**Experiments:**
- Require students to try 3+ variations and compare
- Provide comparison checklist (accuracy, training time, parameters, etc.)
- Encourage reproducibility checks (same seed → same results)

---

## Summary Table: Days 1-10

| Day | Topic | Status | Quality | Key Missing |
|-----|-------|--------|---------|------------|
| 1 | First NN | ✅ Complete | 8/10 | LR ablation, val split, loss curves |
| 2 | CNNs | ✅ Complete | 8/10 | Math formulas, parameter counts, architecture choices |
| 3 | Advanced CNNs | ✅ Complete | 9/10 | Quantitative analysis of augmentation benefits |
| 4 | Optimization | ✅ Complete | 8/10 | Fair optimizer comparison (lr tuning), batch norm connection |
| 5 | NumPy NN | ✅ Complete | 9/10 | BatchNorm completion, Conv layer, profiling |
| 6 | Transfer Learning | ❌ Pending | - | When complete: strategy comparison |
| 7 | Evaluation | ❌ Pending | - | When complete: class imbalance handling |
| 8 | Hyperparameter Tuning | ❌ Pending | - | When complete: systematic methodology |
| 9 | Advanced Architectures | ❌ Pending | - | When complete: deep diving on each architecture |
| 10 | Project 1 | ❌ Pending | - | When complete: clear rubric needed |

---

## Recommendations for Days 11-50

1. **Build on Phase 1 foundation strongly**:
   - Later phases should reference and reuse concepts from Days 1-10
   - Avoid repeating explanations of basic concepts

2. **Introduce new architectures incrementally**:
   - Don't jump to multi-head attention without building intuition
   - Show the "problem" each architecture solves

3. **Emphasize reproducibility and best practices**:
   - Every notebook should include: seeds, hyperparameters, results table
   - Should be easy to compare across days

4. **Include real-world constraints**:
   - Model size (inference on mobile?)
   - Latency requirements
   - Memory constraints
   - Not just accuracy

5. **Systematic evaluation**:
   - Every notebook should produce consistent metrics
   - Create a results dashboard/table comparing all models

6. **Student reproducibility**:
   - Provide requirements.txt for each day/phase
   - Include seeds and exact hyperparameters
   - Reproducible within ±0.1% accuracy

---

**Assessment:** Phase 1 is strong foundation (8-9/10 quality). With the recommended improvements above, this could be 9-10/10. The challenge ahead is maintaining this quality through Phases 2-5 while introducing significantly more complex topics (NLP, Transformers, LLMs).
