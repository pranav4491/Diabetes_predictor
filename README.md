#Diabetes Prediction using Support Vector Machine (SVM)
This project demonstrates how to build a predictive system using a Support Vector Machine (SVM) classifier to predict whether a person has diabetes or not based on various health parameters. The dataset used for this project is the Pima Indians Diabetes Dataset, which is available in the diabetes.csv file.

##Prerequisites
Before running this program, ensure you have the following Python packages installed:

-numpy
-pandas
-scikit-learn

Dataset
The dataset used in this project contains several health-related attributes like:
-Pregnancies
-Glucose
-Blood Pressure
-Skin Thickness
-Insulin
-BMI
-Diabetes Pedigree Function
-Age
###The target variable Outcome is binary, where:

-0 represents non-diabetic
-1 represents diabetic
##Code Overview
###Importing Libraries
We begin by importing the necessary Python modules including numpy, pandas, and scikit-learn.

###Loading the Dataset
The dataset is loaded using pandas.read_csv() and stored in a DataFrame called diabetes_dataset.

###Data Exploration
We inspect the first few rows of the dataset using head().
We check the number of rows and columns with shape.
Statistical measures of the data are obtained using describe().
We check the distribution of the Outcome variable using value_counts() and explore the mean values for each class.
###Data Preprocessing
The feature variables (X) are separated from the target variable (Y).
We standardize the feature variables using StandardScaler to normalize the data.
###Splitting the Data
The data is split into training and testing sets using train_test_split(), with 80% of the data used for training and 20% for testing.

###Model Training
We use an SVM classifier with a linear kernel for training on the training data.

###Model Evaluation
The accuracy of the model is evaluated on both the training and test datasets using accuracy_score().

###Making Predictions
A predictive system is built to classify new input data as diabetic or non-diabetic. The input data is reshaped, standardized, and then passed to the trained classifier to make predictions.

###How to Run
Clone the repository or download the script.
Ensure that diabetes.csv is in the same directory as the script.
Run the script using a Python interpreter.
