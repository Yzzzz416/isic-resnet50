# 🧠 ISIC Skin Lesion Classification with ResNet50

A deep learning-based approach to classify skin lesions using the ISIC dataset. This project fine-tunes a pre-trained **ResNet50** model on dermoscopic images to distinguish between benign and malignant skin conditions.

---

## 📦 Dataset

- **Source:** [ISIC 2020 Challenge Dataset](https://www.kaggle.com/datasets/xhlulu/skin-cancer-mnist-ham10000)
- **Type:** Dermoscopic images of skin lesions
- **Size:** ~25,000 labeled images
- **Task:** Binary classification (Benign vs. Malignant)

---

## 🏗️ Model Architecture

- Base: `ResNet50` pre-trained on ImageNet
- Modified top layers:
  - `GlobalAveragePooling2D`
  - `Dense(1, activation='sigmoid')`
- Loss Function: `Binary Crossentropy`
- Optimizer: `Adam`

---

## 🚀 Getting Started

### 1️⃣ Clone this repo
```bash
git clone https://github.com/Yzzzz416/isic-resnet50.git
cd isic-resnet50
