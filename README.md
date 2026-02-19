# Vision Transformer on CIFAR-10

This repository presents a compact implementation of a Vision Transformer (ViT) model trained for image classification on the CIFAR-10 dataset using PyTorch.

<p align="center">
  <img src="schema.png" width="500">
</p>

<p align="center">
  The schema of Vision Transformer architecture.
</p>

## Objective

The objective is to implement the core ViT pipeline from first principles and evaluate its performance on a standard benchmark dataset.

## Dataset

- Dataset: CIFAR-10
- Training samples: 50,000
- Test samples: 10,000
- Image size: 32x32 RGB
- Number of classes: 10

## Method

The notebook (`main.ipynb`) follows these stages:

1. Data loading and preprocessing with normalization and augmentation.
2. Sample visualization for sanity checks.
3. Patch embedding and tokenization.
4. Class token and positional embedding integration.
5. Multi-head self-attention and transformer block construction.
6. End-to-end training and evaluation.

## Result

- Best test accuracy: **78.67%**
- Training epochs: **20**
- Saved checkpoint: `vit_cifar10_best.pt`

## Repository Structure

- `main.ipynb`: Full implementation, training loop, and plots.
- `vit_cifar10_best.pt`: Best model checkpoint.
- `dataset/`: Local CIFAR-10 files.

## How to Run

1. Install required packages (for example: `torch`, `torchvision`, `matplotlib`).
2. Open `main.ipynb`.
3. Run all cells in order.

## Notes

This repository is prepared for coursework and academic demonstration of ViT fundamentals on small-scale image classification.
