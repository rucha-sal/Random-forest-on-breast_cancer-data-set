1.Import Libraries:
pandas is used for data manipulation and analysis (especially with DataFrames).
numpy is a library for numerical computations.
load_breast_cancer loads a built-in breast cancer dataset from scikit-learn.
matplotlib.pyplot is used for plotting and visualization.

2. Load Dataset:
Loads the breast cancer dataset into the variable cancer. It is a dictionary-like object with features, target labels, and metadata.

3. Explore Dataset Attributes:
dir(cancer) returns a list of attributes and methods associated with the cancer object.
print(attributes) displays them—helpful for understanding what’s available (like data, target, feature_names, etc.).

4. Create DataFrame:
Creates a DataFrame df from the feature data (numerical values for each sample).
5. View Data:
Displays the first 5 rows of the DataFrame to preview the data.
6. Add Target Column:
Adds the target column (0 = malignant, 1 = benign) to the DataFrame.
7. Preview Specific Rows:
Displays the first 12 rows of the updated DataFrame.

8. Split Data into Features & Labels:
X: all columns except target (i.e., the features).
y: the target column (the labels we want to predict).

9. Train-Test Split:
plits the dataset into training (80%) and testing (20%) sets.
X_train, y_train: used to train the model.
X_test, y_test: used to test the model.

10. Train Random Forest Model:
Imports and initializes a Random Forest classifier with 40 trees (n_estimators=40).
Trains the model using the training data.

11. Evaluate the Model:
Returns the accuracy of the model on the test set.

12. Make Predictions:
Predicts the class labels for the test set.
y_predicted contains predicted labels (0 or 1).

13. Confusion Matrix:
Calculates the confusion matrix comparing y_test (true labels) and y_predicted (model predictions).
cm is a 2x2 array showing:
True Positives, False Positives
False Negatives, True Negatives

14. Visualize Confusion Matrix:
Imports seaborn for advanced plotting.
Creates a figure of size 9x6 inches.
Plots the confusion matrix as a heatmap with annotations (annot=True shows values in the cells).
Labels the axes: X-axis is "Predicted", Y-axis is "Truth".

