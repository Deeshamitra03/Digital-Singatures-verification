# ✍️ Signature Verification using Deep Learning

This project focuses on **authenticating handwritten signatures** using Convolutional Neural Networks (CNNs). By distinguishing between genuine and forged signatures, this model can serve as a secure and scalable biometric authentication system.

---

## 📌 Project Overview

Handwritten signatures are still widely used for validating identity in legal, financial, and official scenarios. The goal of this project is to build a robust CNN-based classifier that can:
- Accurately detect forged signatures
- Train on preprocessed grayscale images
- Generalize well across unseen signature samples

---

## 📂 Dataset Structure

```
/Signature_Verification
│
├── /original/     → Contains genuine signature images
├── /forged/       → Contains forged signature images
└── signature_verification.ipynb → Model training notebook
```

- All images are resized to `150x150` pixels
- Images are grayscale and normalized to the range `[0, 1]`


---

## ⚙️ Tech Stack

- Python 3.9+
- TensorFlow 2.15
- Keras
- NumPy
- Scikit-learn
- Matplotlib
- Google Colab 
- Google Drive

---

## 🚀 Model Architecture

- 3 Convolutional Layers
- ReLU Activation
- MaxPooling & Dropout Layers
- Flatten Layer
- Fully Connected Layer with Sigmoid (for binary classification)

You can extend it using pre-trained models like **VGG16** or **InceptionV3** with transfer learning.

---

## 📊 Results

| Metric         | Value      |
|----------------|------------|
| Training Accuracy | ~96.5%    |
| Validation Accuracy | ~95%    |
| Test Accuracy   | ~96.3%    |

Model achieves high performance on distinguishing between real and forged signatures.

---

## 🛠️ How to Run

1. Upload your dataset to Google Drive:
    ```
    /MyDrive/original/
    /MyDrive/Forged/
    ```

2. Open `signature_verification.ipynb` in Google Colab.

3. Mount your Drive and install dependencies:
    ```python
    from google.colab import drive
    drive.mount('/content/drive')

    !pip install tensorflow==2.15.0 scikit-learn matplotlib
    ```

4. Run all the cells to load data, train the model, and view evaluation metrics.

---

## 📈 Future Enhancements

- Use Siamese Networks or Triplet Loss for signature similarity scoring
- Integrate with a front-end for real-time uploads and verification
- Expand dataset to cover multiple writing styles and regions

---

## 🤝 Contributors

- **Deesha Mitra**
- **Dashami S**
- **Rajdeep Sikdar**

---

## 📄 License

This project is for academic and research purposes only.
