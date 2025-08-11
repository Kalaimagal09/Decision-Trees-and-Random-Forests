# Classification with Decision Trees & Random Forests 🌳

This project explores the implementation and evaluation of tree-based models for a binary classification task. Using the Breast Cancer Wisconsin dataset, it compares a single Decision Tree Classifier against a more powerful Random Forest ensemble.

The primary objectives are to understand overfitting in decision trees, learn how to control it, interpret feature importance, and use cross-validation for robust model evaluation.

---

## ## Workflow & Key Steps

1.  **Decision Tree Implementation**: A `DecisionTreeClassifier` was trained on the dataset. The initial, full-depth tree was visualized, revealing a highly complex model. 

2.  **Overfitting Analysis & Pruning**: By comparing training and testing accuracy, the initial tree was shown to be overfit. A "pruned" tree with `max_depth=3` was then trained to create a simpler, more generalized model that performed better on unseen data.

3.  **Random Forest Implementation**: A `RandomForestClassifier` was trained. Its performance was compared to the single decision tree, demonstrating the superior accuracy of the ensemble method.

4.  **Feature Importance**: The `feature_importances_` attribute of the trained Random Forest was used to identify and rank the most influential features for predicting the diagnosis.

5.  **Cross-Validation**: 5-fold cross-validation was used to get a more stable and reliable measure of the Random Forest model's performance, confirming its high accuracy.

---

## ## Key Learnings

* **Model Visualization**: How to visualize a decision tree to understand its decision-making logic.
* **Overfitting Control**: The concept of overfitting in complex models and how hyperparameters like `max_depth` can be used to control it.
* **Ensemble Methods**: The power of a Random Forest to improve accuracy and robustness compared to a single model.
* **Feature Interpretation**: The ability of tree-based models to provide insight into which features are most important for prediction.
* **Robust Evaluation**: The importance of using cross-validation over a single train-test split for a more reliable performance estimate.

---

## ## Tools Used

* Python
* Scikit-learn
* Pandas
* Matplotlib & Seaborn
