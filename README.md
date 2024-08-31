# **SVM Model for ADHD Prediction in ASD**

This repository contains the code for implementing and evaluating a Support Vector Machine (SVM) model to predict ADHD in individuals with Autism Spectrum Disorder (ASD). The code leverages the SRS scores dataset (derived from ABIDE) to train and test the SVM model and includes performance evaluation and feature importance analysis.<br>

To run this code, ensure you have the following Python packages installed:
numpy
pandas
scikit-learn
matplotlib
seaborn
joblib
scipy
You can install these packages using pip/pip3: pip install numpy pandas scikit-learn matplotlib seaborn joblib scipy


### **Dataset**

The dataset used in this project is expected to be in the following directory structure: ../input/srsno-avg2/
The specific file required is MLsheet - SRSno-avg.csv. The dataset is a preprocessed version of the combined ABIDE I and II datasets, cleaned to include the SRS values and binary categorization of HAS_ADHD (0=ASD-only, 1=ASD+ADHD).


### **Code Overview**

1. Data Loading and Preparation: Loads the dataset, filters relevant columns, and splits it into training and testing sets.
2. Model Training: Trains an SVM model with hyperparameter optimization using RandomizedSearchCV.
3. Model Evaluation:
  - Prints the best parameters found and model accuracy.
  - Displays a classification report and confusion matrix.
  - Plots the calibration curve and scatter plots of SRS scores.
  - Generates and displays a correlation matrix.
4. Feature Importance: Computes and plots permutation importance of features.
5. Model Saving: Saves the trained model using joblib.


### **Results**

The code evaluates the SVM model's performance, providing accuracy, classification report, and confusion matrix. It also plots calibration curves, scatter plots of predictions, and feature importance.


### **Feature Importance**

The feature importance scores for the SVM model are computed using permutation importance and visualized in a bar chart.


### **Model Saving**

The trained SVM model is saved as best_svm_model.pkl using joblib.


### **Usage**

To run the code, ensure you have the required dataset in the specified directory and execute the script. The script will output model performance metrics, display plots, and save the trained model.
