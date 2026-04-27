# Banknote-Authentication-UCI-Dataset

Binary classification of genuine vs. forged banknotes using three machine learning models — SVM, K-Nearest Neighbours, and Random Forest — trained on the [Banknote Authentication Dataset](https://archive.ics.uci.edu/ml/machine-learning-databases/00267/) from the UCI Machine Learning Repository.

---

## Abstract: 
Data were extracted from images that were taken for the evaluation of an authentication procedure for banknotes. Click here to get the dataset https://archive.ics.uci.edu/ml/machine-learning-databases/00267/

### Attribute Information
1.  variance of Wavelet Transformed image (continuous)
2.  skewness of Wavelet Transformed image (continuous)
3.  curtosis of Wavelet Transformed image (continuous)
4.  entropy of image (continuous)
5.  class (integer) 

### Data Set Information
Data were extracted from images that were taken from genuine and forged banknote-like specimens. For digitization, an industrial camera usually used for print inspection was used. The final images have 400x 400 pixels. Due to the object lens and distance to the investigated object gray-scale pictures with a resolution of about 660 dpi were gained. Wavelet Transform tool were used to extract features from images. 

## Models & Results

All models were trained on an 80/20 train-test split with `random_state=42`.

| Model | Test Accuracy |
|---|---|
| SVM (RBF kernel, γ=0.7, C=1.0) | **100%** |
| K-Nearest Neighbours (k=6) | **100%** |
| Random Forest (max_depth=5) | **97.8%** |

---

## Exploratory Data Analysis

The notebook includes:
- Missing value analysis
- Correlation heatmap across all numeric features
- Distribution plots for each feature

---

## Requirements

```
numpy
pandas
scikit-learn
seaborn
matplotlib
jupyter
```

Install with:

```bash
pip install numpy pandas scikit-learn seaborn matplotlib jupyter
```

---

## Usage

1. Clone the repo and ensure `bank_notes.csv` is in the working directory.
2. Launch the notebook:

```bash
jupyter notebook banknotes.ipynb
```

---

## Data Source

- **Owner:** Volker Lohweg — University of Applied Sciences, Ostwestfalen-Lippe
- **Donor:** Helene Dörksen — University of Applied Sciences, Ostwestfalen-Lippe
- **Received:** August 2012

UCI dataset link: https://archive.ics.uci.edu/ml/machine-learning-databases/00267/

---

## License

MIT — see [LICENSE](./LICENSE) for details.
