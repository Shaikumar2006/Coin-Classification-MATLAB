# Coin Classification using Image Analysis in MATLAB

## 📌 Overview

This project was completed as the final assignment for the **"Introduction to Data, Signal, and Image Analysis with MATLAB"** course offered by **Vanderbilt University** on **Coursera**.

The goal of this project is to classify U.S. coins (dimes, nickels, quarters) in a composite grayscale image using image processing techniques in MATLAB. The classification is done using a filter bank approach and k-means clustering.

---

## 🧠 Key Concepts Used

- **Otsu's Thresholding** for image segmentation
- **Morphological Filtering** (Dilation and Erosion) to clean and separate coin shapes
- **Feature Extraction** using custom circular filters (filter bank)
- **Clustering** with K-Means to classify coins into three types
- **Centroid Detection** and connected component analysis

---

## 🔍 Project Pipeline

1. **Load and Preprocess Image**
   - Composite image is created from `coins.png` and `eight.tif`
   - Image is zero-padded for edge-safe filtering

2. **Step 1: Coin Segmentation**
   - Otsu's method is used to binarize the image
   - Morphological dilation and erosion clean up the binary mask
   - `regionprops` detects centroids and area of each coin

3. **Step 2: Feature Extraction**
   - A filter bank of three circular filters (dime, nickel, quarter) is constructed
   - For each coin, the correlation with each filter is calculated as a feature

4. **Step 3: Clustering**
   - The resulting feature matrix is passed to MATLAB’s `kmeans` to cluster the coins into 3 groups

5. **Visualization**
   - Centroids and predicted class labels are overlaid on the image for verification

---
## 💻 Requirements

- MATLAB (R2021a or later recommended)
- Image Processing Toolbox

---

## 📚 Course Information

**Course:** [Introduction to Data, Signal, and Image Analysis with MATLAB](https://www.coursera.org/learn/matlab-image-analysis)  
**Institution:** Vanderbilt University  
**Platform:** Coursera  

---

## ✅ Skills Demonstrated

- Classical image segmentation
- Morphological image operations
- Template matching via normalized correlation
- Feature engineering and unsupervised classification
- MATLAB scripting and function writing

---

## 🙌 Acknowledgements

Thanks to **Vanderbilt University**, **Coursera**, and all instructors involved in this course for providing an outstanding learning experience.

---

## 📬 Connect With Me

If you'd like to connect, collaborate, or ask questions:
- [LinkedIn](https://www.linkedin.com/in/umar-shaik-72493a313/)
- [GitHub](https://github.com/Shaikumar2006)
