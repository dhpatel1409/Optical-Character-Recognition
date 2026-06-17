# Optical-Character-Recognition

### Overview

This repository contains the number recognition system using neural networks.

- Training a ResNet9 (with residual connections) on the MNIST handwritten digit dataset.
- Transfer learning for Telugu Numbers with fine-tuning for >90% test accuracy.
- Creating a custom dataset of the first 10 alphabets in a native language.
- Training ResNet9 on the custom dataset.
- 
###Task 1 — MNIST Training

- Defined a ResNet9 architecture with residual (skip) connections using PyTorch nn.Module.
- Trained for 10 epochs on the MNIST dataset (60,000 train / 10,000 test images).
- Validated correctness via test accuracy after each epoch.
- Saved best model checkpoint to Google Drive.
