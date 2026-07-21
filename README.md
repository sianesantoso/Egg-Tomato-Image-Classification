<div align="center">

# 🥚🍅 Egg & Tomato Image Classification using Keras Transfer Learning

### Image Classification with **TensorFlow/Keras**, **Transfer Learning**, and **Data Augmentation**

![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-Deep_Learning-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)
![Keras](https://img.shields.io/badge/Keras-Transfer_Learning-D00000?style=for-the-badge&logo=keras&logoColor=white)
![License](https://img.shields.io/badge/License-Educational-green?style=for-the-badge)

</div>

---

# 📖 Overview

This project implements an **image classification system** to distinguish between **egg** and **tomato** images using **TensorFlow/Keras Transfer Learning**. The dataset was manually collected using a smartphone camera and enhanced through **data augmentation** to improve model generalization and reduce overfitting.

The project demonstrates an end-to-end deep learning workflow, from dataset preparation to model training and evaluation.

---

# 🚀 Features

- 🥚 Binary Image Classification (Egg vs Tomato)
- 🤖 Transfer Learning with TensorFlow/Keras
- 📷 Custom Image Dataset
- 🔄 Data Augmentation
- 🧹 Image Preprocessing
- 📈 Training & Validation Evaluation
- 📊 Accuracy and Loss Visualization

---

# 🗂 Dataset

The dataset consists of **JPG images** captured manually using a smartphone.

### Classes

- 🥚 Egg
- 🍅 Tomato

### Dataset Preparation

- Images collected manually
- Organized into training and validation sets
- Preprocessed before training
- Data augmentation applied during training

---

# 🔄 Data Augmentation

To improve model robustness and minimize overfitting, several augmentation techniques were applied:

- 🔁 Rotation
- ↔️ Horizontal Flip
- 🔍 Zoom
- 📏 Width Shift
- 📐 Height Shift
- ☀️ Brightness Adjustment
- 📐 Rescaling

These augmentations help the model better recognize objects under different viewpoints and lighting conditions.

---

# 🏗 Model Architecture

The classification model was developed using **TensorFlow/Keras Transfer Learning**.

## Training Pipeline

```
Input Image
      │
      ▼
Image Preprocessing
      │
      ▼
Data Augmentation
      │
      ▼
Pretrained CNN
      │
      ▼
Global Pooling
      │
      ▼
Dense Layer
      │
      ▼
Softmax Classification
      │
      ▼
Egg / Tomato Prediction
```

---

# 🧠 Model Workflow

The transfer learning process consists of:

| Step | Description |
|------|-------------|
| Load Pretrained Model | Import a pretrained CNN model |
| Freeze Base Layers | Preserve learned feature representations |
| Add Classification Layers | Build a custom classifier for two classes |
| Fine-Tune Model | Train using the custom dataset |
| Evaluate Model | Measure performance on validation data |

---

# 📊 Model Evaluation

The model performance was monitored using:

- ✅ Training Accuracy
- ✅ Validation Accuracy
- ✅ Training Loss
- ✅ Validation Loss

Learning curves are available in the **results/** directory.

---

# 📈 Training Metrics

The project visualizes:

```
Training Accuracy
Validation Accuracy

Training Loss
Validation Loss
```

These metrics help monitor learning progress and identify overfitting during training.

---

# 📁 Project Structure

```
egg-tomato-classification/
│
├── dataset/
│   ├── train/
│   │   ├── egg/
│   │   └── tomato/
│   │
│   └── validation/
│       ├── egg/
│       └── tomato/
│
├── notebooks/
│   └── training.ipynb
│
├── models/
│   └── model.h5
│
├── results/
│   ├── accuracy.png
│   ├── loss.png
│   └── predictions/
│
├── requirements.txt
├── README.md
└── LICENSE
```

---

# ⚙️ Installation

Clone this repository

```bash
git clone https://github.com/yourusername/egg-tomato-classification.git
```

Move into the project directory

```bash
cd egg-tomato-classification
```

Install dependencies

```bash
pip install -r requirements.txt
```

---

# 📦 Requirements

- Python 3.10+
- TensorFlow
- Keras
- NumPy
- OpenCV
- Matplotlib
- Pillow

---

# 🎯 Key Highlights

✅ Built using a **custom image dataset** collected manually.

✅ Applied **transfer learning** to leverage pretrained visual features.

✅ Improved model robustness through **data augmentation**.

✅ Evaluated model performance using **training and validation metrics**.

---

# 🔮 Future Improvements

- Increase dataset size
- Add more object categories
- Fine-tune additional pretrained architectures
- Deploy using Streamlit or Flask
- Convert the model to TensorFlow Lite for mobile deployment

---

# 📜 License

This project is intended for **educational and learning purposes**.

---

<div align="center">

### ⭐ If you found this project useful, consider giving it a star!

</div>
