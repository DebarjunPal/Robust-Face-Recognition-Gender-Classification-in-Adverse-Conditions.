# Robust Face Recognition & Gender Classification in Adverse Conditions

This repository provides a robust solution for **Face Recognition** and **Gender Classification** under challenging conditions such as low resolution, occlusion, and varying illumination. The project leverages deep learning models trained on diverse datasets to ensure high accuracy, and includes all scripts, pretrained weights, and clear instructions for use and extension.

---

## Table of Contents

- [Features](#features)
- [Project Architecture](#project-architecture)
- [Installation](#installation)
- [Pretrained Model Weights](#pretrained-model-weights)
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

- **Face Recognition Model**: [download link or path]
- **Gender Classification Model**: [download link or path]

Place all downloaded files in the `models/` directory.

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
