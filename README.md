# 🧠 Brain Tumor Detection using Artificial Neural Network (ANN)

## Project Overview

This repository contains a machine learning project focused on the binary classification of medical data to detect the presence of a brain tumor. We utilize an **Artificial Neural Network (ANN)**, built with TensorFlow/Keras, to classify based on extracted image characteristics.

This project serves as a demonstration of applying deep learning principles to a critical medical diagnostics problem.

## Methodology and Workflow

The Jupyter Notebook (`Brain_tumor.ipynb`) implements a standard machine learning pipeline:

1.  **Data Loading:** Imports image feature data from a `Brain Tumor.csv` file.
2.  **Feature Selection:** Uses calculated image statistics (e.g., Mean, Variance, Contrast, Energy) as independent variables (`X`) to predict the binary target class (`y`).
3.  **Data Preprocessing:** Applies **Feature Scaling** using `StandardScaler` to normalize the input data, which is essential for stable and efficient training of the Neural Network.
4.  **Model Architecture (ANN):** Constructs a **Sequential Deep Learning Model** using TensorFlow/Keras with dense layers.
5.  **Training and Evaluation:** The model is trained on the preprocessed data to learn the relationship between image features and the presence of a tumor.

## Technical Stack

* **Language:** Python
* **Core Libraries:**
    * `pandas`, `numpy` (Data manipulation)
    * `sklearn` (Data splitting, `StandardScaler`)
    * `tensorflow.keras` (Building the ANN model)
    * `matplotlib` (Visualization)
* **Model:** Artificial Neural Network (ANN)
* **Task:** Binary Classification

## Predicted Outcome

The model is trained to output a binary class:
* **0:** No Tumor Detected
* **1:** Tumor Detected

The snippet showcases a successful prediction: `Predicted Class: 1 (Tumor Detected) 🚨`.

## How to Run Locally

1.  **Clone this repository:** `git clone [Your Repository URL]`
2.  **Install Dependencies:** Ensure you have the necessary libraries installed.
    ```bash
    pip install pandas numpy scikit-learn tensorflow matplotlib
    ```
3.  **Data Requirement:** This project requires the `Brain Tumor.csv` dataset to be present in the project root directory.
4.  **Execute:** Open and run the `Brain_tumor.ipynb` file in a Jupyter environment (Jupyter Lab, VS Code, or Google Colab).
