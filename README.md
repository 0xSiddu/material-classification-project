# Material Classification

An end-to-end image classification pipeline that identifies material types — wood, metal, plastic, glass, and more — using CNN-based deep learning.

![Python](https://img.shields.io/badge/Python-3.8+-blue?style=flat-square)
![TensorFlow](https://img.shields.io/badge/TensorFlow-Keras-orange?style=flat-square)
![License](https://img.shields.io/badge/license-MIT-green?style=flat-square)

---

## What it does

Trains a convolutional neural network to distinguish between material types from raw image input. The pipeline covers everything from dataset loading and augmentation through to training, evaluation, and single-image inference.

**Supported materials:** wood · metal · plastic · glass · and more

---

## Pipeline

1. **Load dataset** — images from `dataset/`, split into train and test sets
2. **Augment** — flips, rotations, and zoom to improve generalization
3. **Train** — CNN learns discriminative features per material class
4. **Evaluate** — validation accuracy, confusion matrix, loss curves
5. **Predict** — pass any image to get a predicted material label

---

## Project structure

```
material-classification/
├── dataset/          # training & test images
├── models/           # saved model weights
├── notebooks/        # exploratory notebooks
├── src/
│   ├── train.py      # training loop
│   ├── predict.py    # inference script
│   └── utils.py      # shared helpers
├── main.py
└── requirements.txt
```

---

## Getting started

```bash
git clone https://github.com/your-username/material-classification.git
cd material-classification
pip install -r requirements.txt
```

**Train the model**

```bash
python src/train.py
```

**Run inference on an image**

```bash
python src/predict.py --image path/to/image.jpg
```

---

## Tech stack

- Python 3.8+
- TensorFlow / Keras
- NumPy, Pandas
- OpenCV / PIL
- Matplotlib / Seaborn

---

## Results

The model achieves strong accuracy on the validation set with good generalization to unseen images. Training curves (accuracy and loss) are saved automatically to `models/` after each run.

---

## Roadmap

- [ ] Transfer learning via ResNet / EfficientNet
- [ ] Larger, more diverse dataset
- [ ] Web demo with Streamlit or FastAPI
- [ ] Real-time webcam classification
- [ ] Mobile export via TFLite

---

## Acknowledgements

Built using open-source datasets and resources from the deep learning community.

---

Built by [0xSiddu](https://github.com/0xSiddu)
