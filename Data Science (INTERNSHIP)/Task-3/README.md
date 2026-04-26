# Customer Churn Prediction

## Overview
This project is Task 3 of the Data Science Internship program. It focuses on predicting customer churn using machine learning techniques. The goal is to analyze customer data and build a model that can identify customers likely to leave (churn) based on various features.

## Dataset
The dataset used is `Churn_Modelling.csv`, which contains customer information including demographics, account details, and churn status. Key features include:
- Customer demographics (age, gender, geography)
- Account information (balance, number of products, etc.)
- Churn status (Exited: 1 for churned, 0 for retained)

## Requirements
To run this project, you need the following Python libraries:
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

You can install them using pip:
```
pip install pandas numpy matplotlib seaborn scikit-learn
```

## How to Run
1. Ensure you have Jupyter Notebook or Jupyter Lab installed.
2. Open the `customer_churn_prediction.ipynb` notebook.
3. Run the cells in order from top to bottom.
4. The notebook will load the dataset, preprocess the data, train a Random Forest model, and evaluate its performance.

## Project Steps
The notebook follows these main steps:
1. **Import Libraries**: Load necessary Python libraries for data handling, visualization, and machine learning.
2. **Load Dataset**: Read the CSV file into a pandas DataFrame.
3. **Data Exploration**: Examine the dataset structure, check for missing values, and get statistical summaries.
4. **Data Cleaning**: Remove unnecessary columns that don't contribute to prediction.
5. **Encode Categorical Data**: Convert categorical variables (Gender, Geography) into numerical format using Label Encoding and One-Hot Encoding.
6. **Define Features and Target**: Separate the input features (X) from the target variable (y = Exited).
7. **Train-Test Split**: Split the data into training (80%) and testing (20%) sets.
8. **Train Model**: Use Random Forest Classifier to train the model on the training data.
9. **Make Predictions**: Predict churn on the test set.
10. **Model Evaluation**: Assess model performance using accuracy, confusion matrix, and classification report.
11. **Feature Importance**: Visualize which features are most important for the predictions.
12. **Extra Visualizations**: Plot churn distribution and relationships like age vs. churn.

## Expected Output
- Model accuracy score
- Confusion matrix showing true positives, false positives, etc.
- Classification report with precision, recall, and F1-score
- Feature importance bar chart
- Visual plots of churn distribution and age analysis

## Notes
- The dataset path in the notebook is set for Google Colab (`/content/drive/MyDrive/Churn_Modelling.csv`). Adjust the path if running locally.
- The model uses default Random Forest parameters; hyperparameter tuning could improve performance.
- This is a binary classification problem where 1 indicates churn and 0 indicates retention.