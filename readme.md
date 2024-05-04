# Project: Sonar Rock vs. Mine Classification

## Importing the Dependencies
The required Python libraries, including NumPy, Pandas, and scikit-learn, are imported at the beginning of the project.

## Data Collection and Preprocessing
- The sonar dataset is loaded into a Pandas DataFrame.
- Exploratory data analysis is performed on the dataset, including:
   - Inspecting the first few rows
   - Checking the number of rows and columns
   - Calculating summary statistics
   - Analyzing the distribution of the target variable
## Splitting the Data
- The input features (independent variables) and the target variable (dependent variable) are separated from the dataset.
- The data is then split into training and test sets using scikit-learn's `train_test_split` function.
- The `stratify` parameter is used to ensure that the class distribution of the target variable is preserved in both the training and test sets.

## Model Selection and Training
- A logistic regression model from scikit-learn is chosen for this classification problem.
- The model is instantiated, and then trained on the training data (`X_train` and `Y_train`).

## Evaluating the Model
- The trained model's performance is evaluated by calculating the accuracy scores on both the training and test data.
- The `accuracy_score` metric from scikit-learn is used to compare the predicted values with the true values.

## Making Predictions
- After evaluating the model's performance, it is used to make predictions on new, unseen data.
- A sample input (a tuple of feature values) is provided, which is preprocessed (converted to a NumPy array and reshaped) before being passed to the model's `predict` method.
- The prediction ('R' for Rock or 'M' for Mine) is then printed.

The project demonstrates the end-to-end process of working with a dataset, from data loading and preprocessing to model training, evaluation, and making predictions on new data. It showcases the use of popular Python libraries like Pandas and scikit-learn for data analysis and machine learning tasks.
