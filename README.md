# Image Classification with CIFAR‑10

A project to study and test deep learning architectures on the CIFAR‑10 dataset to deepen my understanding of deep learning.

## About

CIFAR‑10 is a well‑known benchmark dataset consisting of 60,000 32×32 colour images across 10 classes (airplane, automobile, bird, cat, deer, dog, frog, horse, ship, truck). It is small enough for fast experimentation yet complex enough to expose the behaviour of modern neural networks.

This repository is **not** about chasing state‑of‑the‑art accuracy. It is a personal laboratory where I systematically experiment with:

- Different architectures (MLPs, CNNs, ResNets, etc.)
- Optimisation strategies (SGD, Adam, learning rate schedules)
- Regularisation and augmentation techniques
- Training dynamics and debugging

## Tech Stack

- **Python** and **PyTorch**
- torchvision for dataset handling and transforms
- TensorBoard.

## Goal

The primary aim is to build deep, hands‑on intuition for designing and troubleshooting neural networks. Lessons learned here are intended to transfer to more advanced research projects, such as those involving EEG, network intrusion detection, or medical imaging.