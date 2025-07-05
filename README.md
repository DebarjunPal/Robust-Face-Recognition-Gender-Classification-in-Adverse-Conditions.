# Robust Face Recognition & Gender Classification in Adverse Conditions

This repository provides a robust solution for **Face Recognition** and **Gender Classification** under challenging conditions such as low resolution, occlusion, and varying illumination. The project leverages deep learning models trained on diverse datasets to ensure high accuracy, and includes all scripts, pretrained weights, and clear instructions for use and extension.

---

## Table of Contents

- [Features](#features)
- [Project Architecture](#project-architecture)
- [Installation](#installation)
- [Pretrained Model Weights](#pretrained-model-weights)
- [Training & validation results](#Training-&-validation-results)
- [Folder Structure](#folder-structure)
- [Citation](#citation)
- [License](#license)
- [Contact](#contact)

---

## Features

- **Face Recognition**: Identifies individuals from input images.
- **Gender Classification**: Predicts gender from facial images.
- **Robust to Adversities**: Handles low-quality, occluded, or poorly-lit images.
- **Pretrained Models**: Directly usable without retraining.
- **Well-documented & Modular Code**: Easily extensible and maintainable.

---

## Project Architecture

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

## Installation

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


## Pretrained Model Weights

Download pretrained weights from the following sources:

- **Gender Classification Model**: [Gender_Classification_(Binary).ipynb]

All downloaded files are in the `models/` directory.

---

## Training & validation results

 precision    recall  f1-score   support

           0       0.78      0.09      0.16        79
           1       0.83      0.99      0.90       343

    accuracy                           0.82       422
   macro avg       0.80      0.54      0.53       422
weighted avg       0.82      0.82      0.76       422

---

## Folder Structure

```
Robust-Face-Recognition-Gender-Classification-in-Adverse-Conditions/
│
├── data/
│   ├── train/
│   ├── val/
│  
│
├── models/
│   ├── face_recognition.py
│   └── gender_classification.py
│
│
├── requirements.txt
├── README.md
└── ...
```

---

## Citation

If you use this work in your research, please cite:

```
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

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## Contact

For questions or contributions, open an issue or contact [Debarjun Pal](https://github.com/DebarjunPal).
