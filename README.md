# Task-5-Decision-Trees-and-Random-Forests
---

1.Train a Decision Tree Classifier and visualize the tree.

2.Analyze overfitting and control tree depth.

3.Train a Random Forest and compare accuracy.

4.Interpret feature importances.

5.Evaluate using cross-validation.

---

# Objective: 
Learn tree-based models for classification & regression.

---

# Tools: 
Scikit-learn, Graphviz

---

# code explanation 


---

1. Importing Libraries

Essential Python libraries are imported:

pandas for data handling.

numpy for numerical operations.

matplotlib & seaborn for data visualization.

scikit-learn for machine learning models and evaluation tools.

graphviz and tree.plot_tree for visualizing decision trees.




---

2. Load Dataset

The heart disease dataset is loaded from your Google Drive location.

The dataset includes features like age, cholesterol, blood pressure, etc., and a target column indicating presence of heart disease.



---

3. Feature and Target Split

Features (X) are separated from the target variable (y).

The target column represents the class (heart disease or not).



---

4. Train-Test Split

The dataset is split into training (80%) and testing (20%) sets.

This ensures we can train the model and then test it on unseen data.



---

5. Train Decision Tree Classifier

A Decision Tree model is created with a maximum depth (e.g., max_depth=4) to prevent overfitting.

The model is trained on the training data.



---

6. Visualize the Decision Tree

The trained tree is displayed graphically using plot_tree.

It shows:

Splits at each node based on feature values.

The predicted class at the leaf nodes.

How the model makes decisions.




---

7. Evaluate Decision Tree

Predictions are made using the test data.

Metrics used:

Accuracy score: Proportion of correct predictions.

Classification report: Includes precision, recall, and F1-score.

Confusion matrix: Shows counts of true positives, false positives, etc.




---

8. Train Random Forest Classifier

A Random Forest model is trained, which is an ensemble of many decision trees (default 100).

It uses bagging and random feature selection to improve accuracy and reduce overfitting.



---

9. Evaluate Random Forest

Predictions are made using the test set.

Same evaluation metrics are used as with the decision tree.

Random Forest typically performs better and is more robust.



---

10. Feature Importance Analysis

Random Forest computes importance scores for each feature.

Features contributing more to predictions are given higher scores.

A bar plot is generated showing which features are most informative.



---

11. Cross-Validation

5-fold cross-validation is used to assess model performance more reliably.

The model is trained and tested on different subsets of data five times.

Average accuracy across folds is reported for both Decision Tree and Random Forest.
