# Image Classification with CIFAR‑10

A project to study and test deep learning architectures on the CIFAR‑10 dataset to deepen my understanding of deep learning.

## About

CIFAR‑10 is a well‑known benchmark dataset consisting of 60,000 32×32 colour images across 10 classes (airplane, automobile, bird, cat, deer, dog, frog, horse, ship, truck). It is small enough for fast experimentation yet complex enough to expose the behaviour of modern neural networks.

This repository is **not** about chasing state‑of‑the‑art accuracy. It is a personal laboratory where I systematically experiment with:

- Different architectures (MLPs, CNNs, ResNets, etc.)
- Optimisation strategies (SGD, Adam, learning rate schedules)
- Regularisation and augmentation techniques
- Training dynamics and debugging

## Setup

### Prerequisites
- Python 3.10 or newer
- (Optional) NVIDIA GPU with updated driver, PyTorch will automatically use it; CPU‑only also works fine

### 1. Clone the repo and create a virtual environment
```bash
python -m venv venv
```

**Activate it:**
- Windows (Command Prompt): `venv\Scripts\activate`
- Windows (PowerShell): `.\venv\Scripts\Activate`
- Linux: `source venv/bin/activate`

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

If you have an NVIDIA GPU and want CUDA support, the `requirements.txt` was created with the CUDA‑enabled PyTorch index. If you prefer a CPU‑only installation, replace `torch` and `torchvision` in `requirements.txt` with the CPU versions from [pytorch.org](https://pytorch.org).

### 3. Verify PyTorch sees your GPU (optional)
```bash
python -c "import torch; print('CUDA available:', torch.cuda.is_available())"
```
If `True`, you're ready to train on GPU.

## Tech Stack

- **Python** and **PyTorch**
- torchvision for dataset handling and transforms
- TensorBoard for experiment tracking
- Jupyter notebooks for interactive exploration

## Goal

The primary aim is to build deep, hands‑on intuition for designing and troubleshooting neural networks. Lessons learned here are intended to transfer to more advanced research projects, such as those involving EEG, network intrusion detection, or medical imaging.