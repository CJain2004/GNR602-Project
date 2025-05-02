# GNR602-Project
This project tackles the land cover classification problem using the DeepSat SAT-4 satellite imagery dataset using SVM Model

## Usage Instructions

> ⚠️ **Important:** This UI is supported **only on Google Colab**.

## 🚀 How to Run

1. Open the `.ipynb` file.
2. Click the **"Open in Colab"** link at the top of the notebook (No need of requirements.txt file)
3. Once opened in Colab, you have two options:

### ▶️ Option 1: Use Pretrained Models (Recommended for Quick Testing)

- Download the `models.zip` file from the repository.
- Extract it to get the two SVM model files.
- Upload these model files to your Colab session.
- Navigate to the **third-to-last cell** in the notebook.
- Run that cell to launch the GUI interface and start testing on images.

### 🔁 Option 2: Train Models from Scratch

- Simply run **all the cells** in the notebook **in order**.
- This will retrain the models before launching the interface.

---
## 🧪 Using the UI

- Scroll to the **third-to-last cell**, which contains the user interface.
- In the interface:
  - Select an image for analysis.
  - Set the `stride` parameter (default is `14`).
- Run the cell to view the GUI output.

> ⏳ **Note:** Image analysis may take some time. Please be patient while the processing completes.


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
