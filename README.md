# Deep Learning Midterm Projects: DNN & CNN

This repository contains two deep learning projects developed for a midterm assignment.

## 1. DNN — Stroke Prediction
A Deep Neural Network predicts stroke risk from patient health and demographic information. The workflow includes data cleaning, missing-value imputation, categorical encoding, feature scaling, class weighting, and threshold evaluation. Logistic Regression is included as a baseline.

**Reported results:** DNN ROC-AUC ≈ 0.802 and PR-AUC ≈ 0.169. Because the dataset is highly imbalanced, this is a learning project and potential screening aid—not a medical diagnosis tool.

**Dataset:** [Stroke Prediction Dataset on Kaggle](https://www.kaggle.com/datasets/fedesoriano/stroke-prediction-dataset)

## 2. CNN — Supermarket Shelf Classification
A Convolutional Neural Network classifies annotated supermarket shelf image crops into **Product** and **Price** categories. The dataset contains 45 original shelf photographs and 11,656 extracted crops, resized to 128 × 128 RGB images.

**Reported results:** 88.65% test accuracy, test loss of 0.4311, and approximately 2.97 minutes of training over 13 epochs.

**Important limitation:** The model classifies pre-cropped regions. It does not detect products in a full shelf image or read and match prices.

## Technologies
- Python
- TensorFlow / Keras
- NumPy and Pandas
- scikit-learn
- Matplotlib and Seaborn
- Pillow
- Jupyter Notebook

## Getting Started
1. Clone or download this repository.
2. Create and activate a Python virtual environment (recommended).
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Open the relevant notebook in Jupyter or Google Colab.
5. Download the datasets from their sources and update file paths in the notebooks before running them.

## Datasets
- **Stroke prediction:** Download the Kaggle dataset linked above. The DNN notebook expects `healthcare-dataset-stroke-data.csv`.
- **Supermarket shelf classification:** Use `Supermarket shelves.zip` and ensure the CNN notebook points to the correct archive path.

## Notes
Results may vary slightly when notebooks are rerun because of random initialization, data splits, and hardware differences. Check each notebook for preprocessing steps and evaluation outputs.
