# Model Development Process

## Objective
The goal of this project was to check whether patient medical attributes can be used to predict the risk of heart disease using supervised machine learning.

Instead of using only one algorithm, multiple models were trained and compared to understand which approach handles medical data better.

## Data Preparation
The dataset contains structured medical parameters for each patient.  
Before training the models, the following steps were performed:

- Removed missing values
- Verified numeric ranges for medical attributes
- Separated input features and target label
- Split data into training and testing sets
- Applied feature scaling so that attributes with larger values (like cholesterol) would not dominate smaller ones

Feature scaling was necessary because distance-based models and linear models are sensitive to magnitude differences.

## Model Training
Two models were trained:

### Logistic Regression
Used as a baseline medical classification model because it works well for binary outcomes and gives stable predictions.

### Random Forest
Used to capture non-linear relationships between symptoms and heart disease risk.

Both models were trained on the same dataset and evaluated on unseen test data.

## Model Evaluation
Instead of relying only on accuracy, additional metrics were used:

- Precision → how many predicted patients were actually sick
- Recall → how many sick patients were detected
- F1 Score → balance between precision and recall

F1-score was used for final selection because missing a sick patient is more serious than a false alarm.

## Final Selection
The model with the higher F1-score was selected and saved.  
The saved model is later used by the Flask web application to make real-time predictions.
