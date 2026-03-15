# 🧠 Brain Tumor Classification — CNN + Flask Web App

> A deep learning web application that classifies brain MRI scans to detect the presence of tumors in real-time. Upload an MRI image and get an instant prediction.

🌐 **Live Demo:** https://shivanalli-brain-tumor-classification.hf.space
http://127.0.0.1:5000


![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![TensorFlow](https://img.shields.io/badge/TensorFlow-Keras-orange?logo=tensorflow)
![Flask](https://img.shields.io/badge/Flask-Web%20App-lightgrey?logo=flask)
![CNN](https://img.shields.io/badge/CNN-Deep%20Learning-red)
![Accuracy](https://img.shields.io/badge/Detection%20Accuracy-99.33%25-brightgreen)

---

## 📌 Problem Statement

Brain tumor detection from MRI scans is a critical medical challenge. Manual diagnosis is time-consuming and prone to human error. This project implements a CNN-based web application that allows users to upload brain MRI images and receive real-time predictions on whether a tumor is present.

---

## 🌐 Web Application

A full-stack Flask web app with:
- **Upload interface** — drag and drop or select MRI image
- **Real-time prediction** — CNN model processes the image instantly
- **Result display** — Tumor Detected / No Tumor with confidence score
- **Responsive UI** — built with HTML, CSS, JavaScript

---

## 📊 Dataset

MRI images organized into two classes:

| Class | Folder | Description |
|---|---|---|
| Tumor | `Y1.jpg – Y259.jpg` | Brain MRI scans with tumor |
| No Tumor | `No1.jpg – No22.jpg`, `N1.jpg – N26.jpg` | Healthy brain MRI scans |

---

## 🤖 Model Details

| Property | Details |
|---|---|
| Architecture | Convolutional Neural Network (CNN) |
| Training Epochs | 10 |
| Saved Models | `BrainTumor10Epochs.h5`, `BrainTumor10EpochsCategorical.h5` |
| Detection Accuracy | **99.33%** |
| AUC-ROC | **0.9995** |
| Task | Binary Classification (Tumor / No Tumor) |

---

## ⚙️ Project Workflow

```
1. Dataset Preparation  →  Tumor (Y) and No Tumor (N/No) MRI images
2. Model Training       →  CNN trained for 10 epochs using Keras/TensorFlow
3. Model Saving         →  Exported as .h5 files for inference
4. Flask App            →  Web interface to upload & predict
5. Prediction           →  Real-time classification on uploaded MRI
```

---

## 🛠️ Tech Stack

| Tool | Usage |
|---|---|
| Python | Core language |
| TensorFlow / Keras | CNN model training & inference |
| OpenCV | Image preprocessing |
| Flask | Web framework |
| HTML / CSS / JavaScript | Frontend interface |
| NumPy | Numerical operations |

---

## 📁 Project Structure

```
Brain-Segmentation-CV-/
│
├── templates/                        # HTML templates (Flask)
├── static/                           # CSS, JS, assets
├── uploads/                          # Uploaded MRI images
├── pred/                             # Prediction outputs
├── no/                               # No tumor images
├── app                               # Flask app entry point
├── mainTrain                         # Model training script
├── mainTest                          # Model testing script
├── BrainTumor10Epochs.h5             # Trained CNN model
├── BrainTumor10EpochsCategorical.h5  # Categorical CNN model
└── README.md
```

---

## 🚀 How to Run Locally

```bash
# 1. Clone the repository
git clone https://github.com/nallishiva/Brain-Segmentation-CV-.git

# 2. Install dependencies
pip install tensorflow keras flask opencv-python numpy pillow

# 3. Run the Flask app
python app.py

# 4. Open in browser
http://localhost:5000
```

---

## 📬 Languages Used

- Python — 28%
- CSS — 47.1%
- JavaScript — 13.8%
- HTML — 11.1%

---

## 👤 Author

**Nalli Shiva** — B.Tech CSE, Lovely Professional University (2024)
[LinkedIn](https://www.linkedin.com/in/nallishiva) · [GitHub](https://github.com/nallishiva)

---
*Built with ❤️ as part of B.Tech CSE — Computer Vision & Deep Learning (2024)*
