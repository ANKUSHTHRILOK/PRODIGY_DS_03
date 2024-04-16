Data Loading and Preprocessing:
The dataset (bankdata.csv) is loaded into a pandas DataFrame.
Missing values (NaN) are removed using the dropna() function to ensure clean data.
Data Splitting for Training and Testing:
The dataset is split into training (X_train, y_train) and testing (X_test, y_test) sets.
X_train contains numerical features used for model training.
y_train represents the target variable (label) to be predicted.
Model Selection and Training:
We use the DecisionTreeClassifier from sklearn.tree for building a Decision Tree-based classification model.
LabelEncoder from sklearn.preprocessing transforms categorical target (y_train) into numeric labels suitable for modeling.
Model Training and Prediction:
The Decision Tree Classifier is trained on X_train and y_train using the fit() method.
Predictions (y_pred) are generated for the test set (X_test) using the predict() method.
Evaluation and Analysis:
We print predicted values (y_pred) and actual values (y_test) to assess model performance.
Specific values are selected for prediction using the trained model.
Visualization:
We visualize the Decision Tree structure using plot_tree from sklearn.tree.
The tree shows decision paths for predicting “Purchase” or “No purchase” based on provided features.
