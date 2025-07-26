
# 🧠 Simple Transfer Learning Project with VGG16

This project shows how to train image classification models using **transfer learning**.

We use the **VGG16 , ResNet50 model** and try 4 different ways to train it:

1. Train from scratch
2. Transfer learning (freeze layers)
3. Fine-tune model
4. Pretrain on a new dataset

---

## 📁 Files in This Project

```
├── 1_Train_from_scratch.ipynb     # Train model from scratch (no pretrained weights)
├── 2_Transfer_learning.ipynb      # Use pretrained model and freeze layers
├── 3_Fine_turning.ipynb           # Fine-tune model on sea animals dataset
├── 4_Pretraining.ipynb            # Pretrain model from scratch on sea animals
└── README.md                      # This file
```

---

## 📦 Datasets

We use 2 datasets in this project:

- A small 2-class dataset (train + validation folders)
- A sea animals dataset (downloaded from KaggleHub)

All data is loaded using `ImageFolder` from `torchvision`.

---

## 📘 Notebook Summary

### 1. Train from Scratch
- We build a VGG16 model with **no pretrained weights**.
- Trained fully on a small custom dataset.
- Useful when you want to learn everything from zero.

📄 File: `1_Train_from_scratch.ipynb`

---

### 2. Transfer Learning
- Use a **VGG16 pretrained on ImageNet**.
- **Freeze** the feature extractor (only train the new classifier).
- Good for small datasets.

📄 File: `2_Transfer_learning.ipynb`

---

### 3. Fine-tuning
- Use VGG16 pretrained on ImageNet.
- Train both the classifier and some base layers.
- Works better when your dataset is different from ImageNet.

📄 File: `3_Fine_turning.ipynb`

---

### 4. Pretraining
- Train ResNet50 pretrained weights on the sea animals dataset.
- Prepares the model for tasks in that domain.

📄 File: `4_Pretraining.ipynb`

---

## 🛠 Libraries Used

- `torch`, `torchvision`
- `matplotlib`, `numpy`
- `kagglehub`
- `torchsummary`
- Google Colab + Drive

---

## ✅ How to Run

1. Open any notebook in **Google Colab**.
2. Mount your **Google Drive**.
3. Make sure the dataset path is correct.
4. Run each cell step by step.

---

## 👤 Author

**Nguyễn Tiến Anh**

This project is for learning transfer learning using VGG16, Resnet50 and PyTorch.

