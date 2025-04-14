# 🧠 Brain Tumor Classification Using Classical Machine Learning

This project involves detecting brain tumors from MRI images using classical machine learning models such as **SVM**, **Random Forest**, and **KNN**. The pipeline includes **image preprocessing**, **feature extraction**, **model training**, and **evaluation**. Implemented using **Python**, **OpenCV**, and **scikit-learn** in Google Colab.

---

## 📁 Dataset

- **Source**: Brain Tumor Dataset stored on Google Drive.
- **Categories**: 
  - `yes` → Tumor present
  - `no` → Tumor absent
- **Format**: JPEG / PNG MRI images

---

## 🔄 Image Preprocessing

Each image undergoes the following steps:
1. **Resize** to 128x128 pixels
2. **Grayscale conversion**
3. **Cropping** the brain region using contour detection
4. **Gaussian Blurring**
5. **Thresholding** (binary)

---

## 📊 Feature Extraction

Two types of features were extracted:

### ✅ Statistical Features:
- Mean
- Standard Deviation
- Variance
- Skewness
- Entropy

### ✅ Texture Features (GLCM):
- Contrast
- Dissimilarity
- Homogeneity
- Energy
- Correlation

> Note: GLCM features were extracted using **multiple distances (1, 2, 3)** and **angles (0°, 45°, 90°, 135°)** for richer texture information.

---

## 🤖 Models Used

- **Support Vector Machine (SVM)**
- **Random Forest Classifier**
- **K-Nearest Neighbors (KNN)**

### Model Evaluation Metrics:
- **Accuracy**
- **Precision**
- **Recall**
- **F1-Score**
- **Confusion Matrix Visualization**
- **Feature Importance (Random Forest)**

---

## 📉 Performance Summary

| Model          | Accuracy | F1 Score | Precision | Recall |
|----------------|----------|----------|-----------|--------|
| SVM            | 48.6%    | 0.50     | 0.50      | 0.50   |
| Random Forest  | 57.1%    | 0.48     | 0.64      | 0.39   |
| KNN            | 48.6%    | 0.44     | 0.50      | 0.39   |

> ⚠️ Due to dataset complexity and limited features, classical ML models showed limited performance.

---

## 🖼️ Visualizations

- **Confusion Matrices** for all models
- **Classified Sample Images**
- **Feature Importance** bar plot (Random Forest)
- **Model Comparison** bar chart

---

## 🛠 Future Improvements

- Switch to **deep learning (CNNs)** for better image representation
- Apply **data augmentation** to increase dataset diversity
- Try **transfer learning** with pre-trained models (e.g., VGG, ResNet)
- Perform **hyperparameter tuning** and **cross-validation**

---

## 💻 Tech Stack

- Python
- OpenCV
- NumPy, SciPy
- scikit-learn
- matplotlib, seaborn
- Google Colab, Google Drive

---

## 📎 Results

All features and evaluation results were exported to:
- `extracted_features.csv`
- Confusion matrices & visualizations saved via Matplotlib

---

## 📚 Learning Outcome

This project was an insightful journey into:
- Image preprocessing and texture analysis
- Feature engineering for medical imaging
- Evaluating classical ML models on real-world tasks
- Understanding limitations and preparing for deep learning solutions

---

## ✨ Author

**Gunjan Duseja** – [LinkedIn](https://www.linkedin.com/in/gunjan-duseja-83b3a828b/)

---

