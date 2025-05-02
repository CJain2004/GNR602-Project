# GNR602-Project
This project tackles the land cover classification problem using the DeepSat SAT-4 satellite imagery dataset using SVM Model

# 🌍 Land Cover Patch-Based Classification using SVM (OvO vs OvR)

This project implements a patch-based image classification system to analyze land cover types from satellite or aerial imagery. It uses Support Vector Machines (SVM) with both One-vs-One (OvO) and One-vs-Rest (OvR) strategies to classify patches into four classes: **Barren Land**, **Trees**, **Grassland**, and **Other**.

Interactive UI is built using Jupyter Notebook widgets, and the classification output is visualized with masks and class distribution pie charts.

---

## 🚀 Features

- Patch-wise classification using:
  - Histogram of Oriented Gradients (HOG)
  - Local Binary Patterns (LBP)
  - Gabor filters
  - Color Histograms (HSV)
- Dual SVM classifier support:
  - One-vs-One (OvO)
  - One-vs-Rest (OvR)
- Real-time performance metrics:
  - Total prediction time
  - Average time per patch
- Interactive UI with:
  - Image upload
  - Stride selection for patch sampling
  - Visual results (color masks, pie charts)

---

## 🧠 Dependencies

Install the required Python libraries before running the notebook:

```bash
pip install numpy opencv-python scikit-image matplotlib ipywidgets joblib cupy
```

You can install all dependencies using:
```bash
pip install -r requirements.txt
```

