# Optical-Character-Recognition

### Overview

This repository contains the number recognition system using neural networks.

- Training a ResNet9 (with residual connections) on the MNIST handwritten digit dataset.
- Transfer learning for Telugu Numbers with fine-tuning for >90% test accuracy.
- Creating a custom dataset of the first 10 alphabets in a native language.
- Training ResNet9 on the custom dataset.

### Task 1 — MNIST Training

- Defined a [ResNet9](model_architecture.png) architecture with residual (skip) connections using PyTorch nn.Module.
- Trained for 10 epochs on the MNIST dataset (60,000 train / 10,000 test images).
- Validated correctness via test accuracy after each epoch.
- Saved best model checkpoint to Google Drive.

### Task 2 - Transfer Learning with Fine-Tuning

- Froze the convolutional layers of the trained MNIST ResNet9.
- Fine-tuned only the MLP (fully connected) layers.
- Target: >90% test accuracy.

### Results
- Classwise accuracy for MNIST dataset
  -  Accuracy for class: 0     is 98.6 %
  -  Accuracy for class: 1     is 98.7 %
  -  Accuracy for class: 2     is 85.9 %
  -  Accuracy for class: 3     is 92.7 %
  - Accuracy for class: 4     is 92.3 %
  - Accuracy for class: 5     is 93.5 %
  -  Accuracy for class: 6     is 96.8 %
  -  Accuracy for class: 7     is 93.6 %
  -  Accuracy for class: 8     is 88.9 %
  -  Accuracy for class: 9     is 93.1 %
 
- Classwise accuracy for Telugu dataset - finetuned on earlier model trained with MNIST dataset
  - Accuracy for class: 0     is 100.0 %
  - Accuracy for class: 1     is 93.1 %
  -  Accuracy for class: 2     is 100.0 %
  - Accuracy for class: 3     is 96.6 %
  - Accuracy for class: 4     is 96.6 %
  - Accuracy for class: 5     is 96.6 %
  - Accuracy for class: 6     is 100.0 %
  - Accuracy for class: 7     is 100.0 %
  - Accuracy for class: 8     is 100.0 %
  -  Accuracy for class: 9     is 100.0 %
