# GNR602-Project
PRBOLEM STATEMENT: Classify a satellite image using SVM classifier with a number of classes > 2 and compare the results of one versus one and one versus rest methods.
This project tackles the land cover classification problem using the DeepSat SAT-4 satellite imagery dataset using SVM Model

## Usage Instructions

> ⚠️ **Important:** This UI is supported **only on Google Colab**.

## 🚀 How to Run

1. Open the `.ipynb` file.
2. Click the **"Open in Colab"** link at the top of the notebook.
3. **Before running anything**, set up the runtime:
   - Click on **"Runtime" > "Change runtime type"** in the Colab menu (next to the "Connect" button).
   - From the dropdown, select **GPU** as the hardware accelerator.
   - Preferably choose **T4 GPU** for optimal performance.
   - Click **Save**.

---

## 🧠 Model Options

You can either use pretrained models for a quick demo or train from scratch.

### ▶️ Option 1: Use Pretrained Models (Recommended for Quick Testing)

- Download the `models.zip` file from this repository.
- Extract the archive to obtain the two SVM model files.
- Upload these model files to your Colab session.
- Scroll down and **navigate to the third-to-last cell** in the notebook.
- Run that cell to launch the GUI interface and start testing on sample images.

### 🔁 Option 2: Train Models from Scratch

- Simply run **all cells in order** from the top of the notebook.
- This will handle training and setup before launching the GUI interface.

---

## 🧪 Using the UI

- Locate and run the **third-to-last cell**, which contains the user interface.
- In the interface:
  - Select an image for analysis.
  - Set the `stride` parameter (default is `14`).
- Run the cell to launch the GUI and begin analysis.

> ⏳ **Note:** Image processing may take a little time. Please be patient as the system analyzes the input.



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
