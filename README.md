# 🏦 Banknote Authentication using ANN

This project applies an **Artificial Neural Network (ANN)** to classify banknotes as authentic or fake using statistical features of their images (variance, skewness, curtosis, entropy).
Some Basic information that need to understand before going into project is the features in the dataset are wave transformed statistical measures. Instead of using Deep learning on every image, researchers transformed and pulled these measures from images which saves lot of time.
Variance tells you how spread out the values are from the average (mean).
 High variance → more contrast/details in that region.
 Low variance → smoother region.
Skewness measures the asymmetry of the pixel value distribution.
 Positive skew → more pixels with low values (long tail on right).
 Negative skew → more pixels with high values (long tail on left).
 
Curtosis (Kurtosis)Measures the “peakedness” or sharpness of the distribution of pixel values.
 High kurtosis → sharp peaks (maybe forged note has sharper noise patterns).
 Low kurtosis → flatter distribution.
Entropy measures the randomness / complexity in the pixel distribution.
 High entropy → more disorder, complexity.
 Low entropy → more uniform, less information.
 Forged notes might show different entropy compared to genuine ones.

## 📂 Dataset
- Source: [Banknote Authentication Dataset on Kaggle](https://www.kaggle.com/datasets/hellbuoy/banknote-authentication-dataset)
- Features:
  - `variance`
  - `skewness`
  - `curtosis`
  - `entropy`
- Target: `0` = fake, `1` = genuine

## ⚙️ Tech Stack
- Python 3
- TensorFlow / Keras
- Scikit-learn
- Pandas, NumPy, Matplotlib

## 🚀 Model Training
```bash
python main.py
