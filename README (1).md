
# 🐶🐱 Image Classification of Dogs vs Cats using KNN and HOG Features

This project performs image classification on the popular **Dogs vs Cats** dataset using a **K-Nearest Neighbors (KNN)** classifier. Feature extraction is done using **Histogram of Oriented Gradients (HOG)**, and visualization is performed using confusion matrices and classification reports.

---

### 📁 Contents

- `Vaishnavi_imageClassification.ipynb` – Notebook implementing:
  - Dataset download via Kaggle
  - Image preprocessing
  - HOG feature extraction
  - KNN training and evaluation

---

### 📌 Workflow Summary

1. **Download Dataset**
   - Automatically downloads `dogs-vs-cats` dataset from Kaggle using API token.

2. **Image Preprocessing**
   - Resizes images to 64x64
   - Loads and batches ~300 sample images

3. **Feature Extraction**
   - Converts images to grayscale
   - Extracts HOG features using `skimage.feature.hog`

4. **Classification**
   - Splits data (80% train / 20% test)
   - Trains a **KNN classifier** (with `k=3`)
   - Evaluates performance

5. **Visualization**
   - Classification report
   - Confusion matrix heatmap

---

### 🛠️ Dependencies

Install the following packages before running the notebook:

```bash
pip install numpy opencv-python scikit-learn scikit-image tensorflow matplotlib seaborn
```

---

### 📂 Dataset Details

- Dataset: [Dogs vs Cats](https://www.kaggle.com/datasets/salader/dogs-vs-cats)
- Structure:
  ```
  dataset/
  └── dogs_vs_cats/
      ├── train/
      │   ├── cat.0.jpg
      │   ├── dog.0.jpg
      ├── test/
      │   ├── cat.1.jpg
      │   ├── dog.1.jpg
  ```

---

### 🚀 How to Use (in Google Colab)

1. **Upload your `kaggle.json` token** (from your Kaggle account API).
2. Run the notebook cells in order.
3. Outputs:
   - HOG feature-based KNN model performance
   - Confusion matrix heatmap
   - Precision, recall, and F1-score

---

### 📊 Results

- **Classifier**: K-Nearest Neighbors (`k=3`)
- **Feature Extractor**: HOG
- **Evaluation**:
  - Confusion Matrix
  - Classification Report

---

### 📬 Contact

For questions or suggestions, contact **Vaishnavi Mishra**.
