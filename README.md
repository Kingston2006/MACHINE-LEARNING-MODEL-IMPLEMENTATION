# MACHINE-LEARNING-MODEL-IMPLEMENTATIONCOMPANY: CODTECH IT SOLUTIONS

"NAME: KINGSTON

"INTERN ID: CTO4DG46

"DOMAIN: PYTHON PROGRAMMING

DURATION: 4 WEEEKS

MENTOR: NEELA SANTOSH


Iris Flower Classification Using Random Forest
This Python script demonstrates a complete machine learning pipeline for classifying iris flowers using the Random Forest algorithm. The Iris dataset is a classic dataset in machine learning and statistics, often used for introducing supervised classification. This script walks through all the essential steps—from data loading and visualization to model training and evaluation—making it ideal for beginners and educational demonstrations.

Overview of the Dataset
The Iris dataset, built into scikit-learn, contains 150 rows with 4 numeric features for each flower sample:

Sepal length (cm)

Sepal width (cm)

Petal length (cm)

Petal width (cm)

Each sample belongs to one of three species of Iris:

Iris Setosa

Iris Versicolour

Iris Virginica

The target column represents the species, encoded as 0, 1, or 2.

Step-by-Step Workflow
1. Library Imports
The script uses:

pandas and numpy for data handling

matplotlib.pyplot and seaborn for visualization

scikit-learn for dataset loading, model creation, and evaluation metrics

These libraries form the core of any beginner-friendly machine learning workflow in Python.

2. Load the Dataset
Using load_iris() from sklearn.datasets, the dataset is loaded and then converted into a pandas DataFrame for easier analysis. The feature data and target labels are combined into one DataFrame, which allows for easier plotting and manipulation.

3. Visualize the Data (Optional)
Using Seaborn’s pairplot() function, the script creates scatter plots for each pair of features, colored by target class. This gives a visual intuition of how separable the classes are across dimensions, and it clearly shows that petal-related features are most useful for classification.

4. Data Preparation
Features (X) and labels (y) are separated:

X contains all feature columns

y is the target label

5. Train-Test Split
The dataset is split into training and testing sets using an 80/20 ratio with train_test_split(). The random seed ensures reproducibility.

6. Train a Random Forest Classifier
A Random Forest Classifier with 100 decision trees is instantiated and trained on the training data. Random forests are known for their accuracy, resistance to overfitting, and interpretability via feature importance.

7. Make Predictions
The trained model is used to predict the species of flowers in the test set.

8. Model Evaluation
The script prints:

Accuracy Score: the percentage of correctly predicted labels

Confusion Matrix: a table showing true vs. predicted class counts

Classification Report: includes precision, recall, and F1-score for each class

These metrics give a complete picture of the model’s performance and class-wise prediction quality.

9. Feature Importance (Optional Visualization)
Finally, the script plots a bar chart of feature importances, as calculated by the Random Forest algorithm. This helps identify which features (like petal length and width) contribute most to model decisions.

