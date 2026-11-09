# Breast Cancer Classification

A machine learning project that predicts whether a tumor is malignant or
benign using the Breast Cancer Wisconsin dataset.

## Dataset
- 569 samples, 30 numerical features (radius, texture, area, etc.)
- Classes: Malignant (212) and Benign (357)
- Source: built into scikit-learn

## Steps
1. Loaded and explored the data
2. Visualized class balance, feature differences, and correlations
3. Split into 80% train / 20% test (stratified) and scaled the features
4. Trained Logistic Regression, KNN, and Decision Tree
5. Evaluated with confusion matrix, precision, recall, and F1-score
6. Reduced Decision Tree overfitting with max_depth=3 (test accuracy 91.23% to 93.86%)
7. Saved the best model
## Results

| Model | Test Accuracy | Missed Malignant Cases |
|---|---|---|
| Logistic Regression | 98.25% | 1 of 42 |
| KNN | 95.61% | 3 of 42 |
| Decision Tree (max_depth=3) | 93.86% | 3 of 42 |

**Best model:** Logistic Regression.

## Tools
Python, pandas, NumPy, matplotlib, seaborn, scikit-learn

## How to run
    python -m venv venv
    venv\Scripts\activate
    pip install -r requirements.txt

## Author
priyanka, B.Tech CSE 