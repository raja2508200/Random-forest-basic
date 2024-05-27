# Random-forest-basic


Loads the dataset from a CSV file:

The dataset is read from a file named 'random forest.csv' using pd.read_csv.
Encodes the 'Gender' column using LabelEncoder:

The 'Gender' column, which likely contains categorical data (e.g., 'Male', 'Female'), is converted to numerical values (e.g., 0 and 1) using LabelEncoder.
Splits the dataset into features (X) and target (y):

The dataset is divided into features (X), which are the input variables, and the target (y), which is the output variable we want to predict (the 'Dataset' column).
Splits the data into training and testing sets:

The data is split into training and testing sets using train_test_split. The training set is used to train the model, and the testing set is used to evaluate the model's performance. The test_size=0.2 parameter means 20% of the data is used for testing.
Initializes and trains a RandomForestClassifier:

A RandomForestClassifier, a type of ensemble learning method, is initialized with 100 trees (n_estimators=100). The classifier is then trained on the training data using the fit method.
Makes predictions on the test set and evaluates the accuracy:

The trained model makes predictions on the test set using the predict method. The accuracy of the model is evaluated by comparing the predicted values with the actual values in the test set using accuracy_score.
Makes a prediction on a new data point:

A new data point, represented by a list of feature values, is provided to the model for prediction using the predict method. The model outputs a prediction for this new data point.
