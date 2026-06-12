# Credit Loan Approval Prediction

A simple machine learning classification project to predict whether a loan application should be approved or not.

## Project Goal

The main goal of this project is to minimize the chances of approving loans for potential defaulters. Because of this, **Precision** was considered the most important evaluation metric.

A higher precision means that when the model predicts a loan should be approved, it is more likely to be correct.

---

## Data Preprocessing

The following preprocessing steps were performed before training the models:

- Handling missing values using `SimpleImputer`
- Encoding categorical features using `LabelEncoder`
- Applying `OneHotEncoder` where required
- Feature scaling using `StandardScaler`
- Train-Test Split

---

## Models Used

The following classification models were trained and evaluated:

1. K-Nearest Neighbors (KNN)
2. Gaussian Naive Bayes
3. Logistic Regression

---

## Model Comparison (Based on Precision)

| Model | Precision |
|---------|---------|
| KNN | 0.5957 |
| Naive Bayes | 0.8036 |
| Logistic Regression | 0.7869 |

---

## Results

Since the main focus of this project was precision, **Gaussian Naive Bayes** performed the best among all tested models.

### Best Model: Gaussian Naive Bayes

- Precision: **80.36%**
- Recall: 73.77%
- F1 Score: 76.92%
- Accuracy: 86.50%

Confusion Matrix:

```text
[[128 11]
 [ 16 45]]
```

---

## Conclusion

Among the three models tested, Gaussian Naive Bayes achieved the highest precision score. Since precision was the primary metric for this loan approval problem, Naive Bayes was selected as the preferred model.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-Learn
- Jupyter Notebook

---

## Future Improvements

- Hyperparameter tuning
- Cross-validation
- Testing additional classification models
- Building a simple web application for predictions
