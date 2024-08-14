##Diabetes Prediction and Risk Segmentation

#This repository contains Python scripts designed to analyze patient data and predict the likelihood of developing diabetes. The scripts also segment patients into risk categories based on various health indicators.

#Overview
This project uses logistic regression to predict diabetes risk based on patient data such as age, BMI, family history, social determinants of health (SDoH), gender at birth, HbA1C levels, fasting sugar levels, and more. Patients are categorized into Low, Medium, or High risk based on their predicted probability of developing diabetes.

Features
Predict Diabetes Risk: Predict whether a patient is likely to develop diabetes.
Segment Patients: Classify patients into risk segments (Low, Medium, High) based on their predicted probability.
Data Handling: The scripts handle data loaded from a CSV file, making it flexible for real-world applications.
Requirements
Python 3.x
Pandas
Scikit-learn
Installation
Clone the repository:

bash
Copy code
git clone https://github.com/yourusername/diabetes-prediction.git
cd diabetes-prediction
Install the required packages:

bash
Copy code
pip install -r requirements.txt
Prepare Your Dataset:

Ensure your dataset is in CSV format with the following columns: age, gender_at_birth, bmi, family_history, sdoh_index, hba1c, fasting_sugar, fever, cough, fatigue, headache, diabetes.
Replace path_to_your_file.csv in the script with the path to your dataset.
Usage

Script 1: Diabetes Prediction with Sample Data

This script contains a hardcoded dataset used to predict the likelihood of developing diabetes.

Run the script:

bash
Copy code
python diabetes_prediction_sample.py
The script will:

Train a logistic regression model.
Predict diabetes risk for a test set.
Segment patients into Low, Medium, or High risk.
Predict risk for a new patient example.
Script 2: Diabetes Prediction with CSV Data
This script loads patient data from a CSV file and performs similar predictions and segmentation.

Make sure that when you use the dataset has clean data. This means the latest information for every paitient, if the the dataset has things missing, 
make sure to choose the last measure for that patient, 
if the patient is fully missing one measure, make sure to use statistically correct processes to not squew the model

Replace 'path_to_your_file.csv' with the actual path to your CSV file in the script.

Run the script:

bash
Copy code
python diabetes_prediction_csv.py
The script will:

Load your dataset.
Train a logistic regression model.
Predict diabetes risk for a test set.
Segment patients into Low, Medium, or High risk.
Predict risk for a new patient example.
Example Output
The output of both scripts includes:

Model Accuracy: The accuracy score of the model on the test data.
Classification Report: A detailed classification report with precision, recall, and F1-score.
Patient Segmentation: A list of patients with their respective risk segments.
Contributing
Contributions are welcome! Please feel free to submit a Pull Request or open an Issue.

License
This project is licensed under HealthPAct

Contact
For any questions or inquiries, please contact mantilla@healthpact.com
