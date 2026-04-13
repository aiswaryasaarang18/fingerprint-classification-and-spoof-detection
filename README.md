# 🧠 Multi-Task Fingerprint Classification and Spoof Detection

## 📌 Overview

This project presents a deep learning-based system for **fingerprint analysis and spoof detection** using a multi-task learning approach. The model simultaneously predicts:

* ✅ Live vs Fake fingerprint
* 👤 Gender (Male/Female/Unknown)
* ✋ Hand (Left/Right/Unknown)
* 🖐️ Finger type (Thumb, Index, Middle, Ring, Little)

The system leverages a powerful convolutional neural network with attention mechanisms to improve feature extraction and classification performance.

---

## 🚀 Key Features

* 🔹 Multi-task learning with 4 output heads
* 🔹 Automatic label extraction from file names
* 🔹 Attention mechanism using CBAM (Convolutional Block Attention Module)
* 🔹 Image preprocessing using CLAHE for contrast enhancement
* 🔹 Works on both full dataset and reduced dataset (500 images)
* 🔹 Real-time prediction support

---

## 🧠 Model Architecture

* **Base Model:** EfficientNetB0
* **Attention Module:** CBAM
* **Framework:** TensorFlow / Keras

The model shares a common feature extractor and branches into multiple outputs for different classification tasks.

---

## 📂 Dataset

* **Dataset:** SOCOFing (Sokoto Coventry Fingerprint Dataset)
* Contains real and altered (spoofed) fingerprint images

📥 Download Dataset:
https://www.kaggle.com/datasets/ruizgara/socofing

### 🏷️ Label Extraction

Labels are automatically extracted from file names.

Example:
1__M_Left_little_finger_Obl.BMP

From this:

* Gender → M (Male)
* Hand → Left
* Finger → Little

---

## ⚙️ Technologies Used

* Python
* TensorFlow / Keras
* OpenCV
* NumPy, Pandas
* Matplotlib, Seaborn
* Scikit-learn

---

## 📊 Results

* ✔ Accurate Live vs Fake detection
* ✔ Successful multi-task predictions
* 📈 Performance evaluated using accuracy and loss curves

> ⚠️ Note: Current evaluation primarily focuses on Live/Fake classification. Other outputs are predicted but not fully evaluated.

---

## ▶️ How to Run

1. Clone the repository:

```
git clone https://github.com/aiswaryasaarang18/fingerprint-classification-spoof-detection.git
```

2. Install dependencies:

```
pip install -r requirements.txt
```

3. Run the notebook:

* Open in Jupyter Notebook or Google Colab
* Execute all cells

---

## 🔍 Sample Prediction

The model can predict:

* Live or Fake fingerprint
* Gender
* Hand (Left/Right)
* Finger type

---

## ⚠️ Important Notes

* Dataset is not included due to size
* Replace dataset paths with your local directory
* Ensure correct folder structure before running

---

## 🌟 Future Improvements

* Full evaluation for all outputs (gender, hand, finger)
* Deployment as a web/mobile application
* Real-time fingerprint scanner integration

---

## 👩‍💻 Author

Aiswarya R

---

## 📜 License

This project is for academic and educational purposes.


