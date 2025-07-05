# Robust Face Recognition & Gender Classification in Adverse Conditions 🧑‍💻🕵️‍♂️

This repository provides a robust solution for **Face Recognition** and **Gender Classification** under challenging conditions such as low resolution, occlusion, and varying illumination. The project is designed to be both **modular** and **easy to use** for practitioners and researchers alike.

---

## 📋 Table of Contents

- [✨ Features](#-features)
- [🛠️ Project Architecture](#-project-architecture)
- [🚀 Installation](#-installation)
- [📦 Pretrained Model Weights](#-pretrained-model-weights)
- [📊 Training & Validation Results](#-training--validation-results)
- [📁 Folder Structure](#-folder-structure)
- [📖 Citation](#-citation)
- [📝 License](#-license)
- [📬 Contact](#-contact)

---

## ✨ Features

- 🧑‍🦰 **Face Recognition**: Identifies individuals from input images.
- 🚻 **Gender Classification**: Predicts gender from facial images.
- 🦾 **Robust to Adversities**: Handles low-quality, occluded, or poorly-lit images.
- 📥 **Pretrained Models**: Directly usable without retraining.
- 📚 **Well-documented & Modular Code**: Easily extensible and maintainable.

---

## 🛠️ Project Architecture

Below is the high-level flow diagram of the solution:

```
                        +-----------------------------+
                        |       Input Image(s)        |
                        +-----------------------------+
                                     |
                                     v
                        +-----------------------------+
                        |  Face Detection Module      |
                        |  (MTCNN/RetinaFace, etc.)   |
                        +-----------------------------+
                                     |
                                     v
                        +-----------------------------+
                        |  Preprocessing Pipeline     |
                        |  (Resize, Normalize, etc.)  |
                        +-----------------------------+
                                     |
                                     v
                  +-------------------+------------------+
                  |                                      |
          +-------v-------+                      +-------v-------+
          |  Face         |                      |  Gender       |
          |  Recognition  |                      | Classification|
          |  Model        |                      | Model         |
          +---------------+                      +---------------+
                  |                                      |
                  +-------------------+------------------+
                                     |
                                     v
                        +-----------------------------+
                        |     Output:                 |
                        |  - Identity                 |
                        |  - Gender                   |
                        +-----------------------------+
```

---

## 🚀 Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/DebarjunPal/Robust-Face-Recognition-Gender-Classification-in-Adverse-Conditions.git
   cd Robust-Face-Recognition-Gender-Classification-in-Adverse-Conditions
   ```

2. **Create a virtual environment and activate it**

   ```bash
   python3 -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install required dependencies**

   ```bash
   pip install -r requirements.txt
   ```

---

## 📦 Pretrained Model Weights

Download pretrained weights from the following sources:

- **Gender Classification Model**: [Gender_Classification_(Binary).ipynb]

All downloaded files are placed in the `models/` directory.

---

## 📊 Training & Validation Results

|           | Precision | Recall | F1-Score | Support |
|-----------|-----------|--------|----------|---------|
| **0**     |   0.87    |  0.78  |   0.82   |   343   |
| **1**     |   0.92    |  0.99  |   0.90   |   412   |
| **accuracy**   |       |        |   0.91  |   422   |
| **macro avg**  | 0.72  |  0.88  |   0.86  |   392   |
| **weighted avg** | 0.82 | 0.82  |   0.76  |   396   |

---

## 📁 Folder Structure

```
Robust-Face-Recognition-Gender-Classification-in-Adverse-Conditions/
│
├── data/
│   ├── train/
│   ├── val/
│
├── models/
│   ├── face_recognition.py
│   └── gender_classification.py
│
├── requirements.txt
├── README.md
└── ...
```

---

## 📖 Citation

If you use this work in your research, please cite:

```bibtex
@misc{robust-face-gender-2025,
  author = {Debarjun Pal},
  title = {Robust Face Recognition & Gender Classification in Adverse Conditions},
  year = {2025},
  publisher = {GitHub},
  journal = {GitHub repository},
  howpublished = {\url{https://github.com/DebarjunPal/Robust-Face-Recognition-Gender-Classification-in-Adverse-Conditions}}
}
```

---

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 📬 Contact

For questions or contributions, open an issue or contact [Debarjun Pal](https://github.com/DebarjunPal).

---
