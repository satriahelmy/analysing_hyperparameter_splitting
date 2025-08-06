# Machine Learning Model Evaluation with Different Data Splits

This project is part of an academic activity to explore how **hyperparameter tuning** and **data splitting strategies** affect machine learning model performance. The experiment was conducted using the built-in **Wine Dataset** from `sklearn.datasets`.

---

## Objective

To compare model performance using:
- Different data split ratios: `60:20:20` vs `70:15:15` (train:validation:test)
- Different models: `Logistic Regression` vs `Support Vector Machine (SVM)`
- Evaluate and reflect on how these choices affect accuracy and generalization.

---

## Experiment Setup

### Dataset:
- **Wine dataset** from `sklearn.datasets.load_wine()`
- Multi-class classification with 3 target classes.

### Data Splits:
- **Experiment 1**: Logistic Regression with 60:20:20
- **Experiment 2**: SVM with 70:15:15


## Results Summary

| Model               | Validation Accuracy | Test Accuracy | Macro F1-score |
|--------------------|---------------------|---------------|----------------|
| Logistic Regression| 0.9444              | 0.9444        | 0.93           |
| SVM (RBF Kernel)   | 0.7407              | 0.7407        | 0.65           |

- **Logistic Regression** performed significantly better across all metrics.
- **SVM** struggled with minority class prediction, especially for `class_2`.

---

## References

- [Scikit-learn Documentation](https://scikit-learn.org/)
- [Wine Dataset Info](https://archive.ics.uci.edu/ml/datasets/wine)
