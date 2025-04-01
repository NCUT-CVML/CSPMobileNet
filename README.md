# 🧠 CSPMobileNet - Lightweight CNN Architecture with Attention for Resource-Constrained Devices

This repository contains the official implementation of three variants of **CSPMobileNet**, a lightweight convolutional neural network integrating **CSPNet**, **depthwise separable convolutions**, and lightweight attention mechanisms (SE, CBAM, CA).

---

## 📦 Project Structure

```bash
.
!├── main.py                   # Training & evaluation (version 1)
!├── main_1.py                 # Training & evaluation (version 2)
├── config.py / config_1.py / config_2.py   # Model specifications
├── model.py / model_1.py     # Model builders (for each version)
├── Layer/                    # Custom layers (CSP block, MBConv, etc.)
├── DataGenerator.py          # Data loading and preprocessing
├── Flops.py                  # Model complexity (FLOPs) calculation
├── notebooks/                # Jupyter Notebooks for training/testing/visualization
│   ├── 01_train.ipynb, 01_train_1.ipynb, 01_train_2.ipynb
│   ├── 02_test_1.ipynb, 102_test.ipynb
!├── 0-MTAP-D-24-01825-R1.pdf  # Official revised paper
!└── README.md
```

---

## 🚀 Quick Start

### 1. Install dependencies

```bash
pip install -r requirements.txt
```

### 2. Run model training & evaluation

```bash
# For version 1
01_train_v1.ipynb

# For version 2 (dual-attention)
01_train_v2.ipynb

# For version 3 (dual-attention)
01_train_v3.ipynb
```

---

## 📊 Jupyter Notebook Guide

| Notebook | Purpose |
|----------|---------|
| `01_train*.ipynb` | Train models (v1/v2/v3) |
| `02_test_1.ipynb`, `102_test.ipynb` | Test trained models |

---

## 💡 Datasets

- `cifar10`, `cifar100`,`bird100`, `bird365`
- Folder format: `Dataset/train`, `Dataset/valid`, `Dataset/test` with subfolders per class
- https://mega.nz/folder/3JZRSY7C#sS-uAwWTo7msAtV2235alw

---

