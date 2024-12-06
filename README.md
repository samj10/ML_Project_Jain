# ML_Project_Jain
 Classification and Missing Value Estimation


Overview

This project involves data preprocessing, missing value estimation, and classification of multiple datasets using a Random Forest classifier. The code loads training data and labels, preprocesses the data by handling missing values and standardizing features, and then trains a classifier while evaluating its performance using cross-validation. Additionally, feature importance and decision tree visualizations are provided for better interpretability.

Prerequisites

Make sure you have Python 3.9 installed, along with the following Python libraries:

numpy

pandas

scikit-learn

matplotlib

To install the required libraries, run the following command:

pip install numpy pandas scikit-learn matplotlib



Ensure that all data is downloaded beforehand.


Use Jupyter or python to run the code


Output
The script will perform the following actions for each dataset:

Load the training data and labels.

Preprocess the data by imputing missing values and standardizing features.

Perform 5-fold cross-validation and output the mean accuracy.

Visualize feature importance and display a sample decision tree from the Random Forest model.

The cross-validation accuracies, as well as visualizations, will be displayed in the terminal and as graphical plots.

Code Functions

load_data(file_path)

Loads the dataset from the given file path, handling multiple delimiters and ensuring numeric data.

preprocess_missing_data(df)

Replaces missing values (1.0e+99) with the mean value of the feature and standardizes the data.

cross_validate_model(X, y, model, k=5)

Performs k-fold cross-validation and returns the mean accuracy.

train_and_visualize_model(X_train, y_train, feature_names)

Trains the Random Forest model, visualizes feature importance, and displays a sample decision tree.

Example Output

During execution, you can expect output similar to the following for each dataset:

Processing Dataset 1 with Cross-Validation and Visualization...
Loading file: /Users/samyakjain/ML_Project_Jain/TrainData/TrainData1.txt
Data before preprocessing: (150, 3312)
Data after preprocessing and scaling: (150, 3312)
Performing 5-fold cross-validation...
Cross-validation accuracies: [0.83333333 0.9        0.9        0.93333333 0.93333333]
Mean accuracy: 0.90
Cross-validation completed for /Users/samyakjain/ML_Project_Jain/TrainData/TrainData1.txt. Mean Accuracy: 0.90
Visualizing Feature Importance...

Troubleshooting

File Not Found: Ensure all datasets and label files are present in the correct directories (TrainData/ and TrainLabel/).

Python Import Errors: If you encounter import errors, ensure that the required libraries are properly installed using pip.

Empty DataFrame: If the data is not loaded properly, check the file formatting and ensure the correct delimiter is used.
