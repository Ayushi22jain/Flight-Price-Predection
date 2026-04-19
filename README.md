# Flight Price Prediction
This repository features a machine learning project designed to predict flight ticket prices. The project involves a deep dive into data preprocessing, feature engineering, and ensemble learning to provide accurate price estimations based on historical flight data.

## 🚀 Project Workflow
1. Data Exploration & Visualization
Statistical Analysis: Initial data description to understand distribution and variance.

Visualization: Used Matplotlib and Seaborn to identify trends and correlations.

EDA: Detailed Exploratory Data Analysis, including converting timestamps into usable features for the model.

2. Feature Engineering & Preprocessing
Categorical Encoding: Handled nominal and ordinal data using One-Hot Encoding and Label Encoding.

Outlier Detection: Utilized Seaborn plots to identify and manage data anomalies.

Feature Selection: Employed multiple techniques to find the most impactful variables:

Heatmaps for correlation.

Feature Importance scores.

SelectKBest for statistical selection.

3. Model Building & Optimization
Algorithm: Fitted the processed data using the Random Forest Regressor.

Tuning: Performed Hyperparameter Tuning to optimize model performance and reduce error rates.

## 🛠️ Tech Stack
Language: Python

Libraries: Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn

Tools: Jupyter Notebook

## 📁 Repository Structure
FlightPrice.ipynb: The complete notebook covering data cleaning, EDA, and modeling.

Data_Train.xlsx / Test_set.xlsx: The datasets used for training and validation.

README.md: Documentation.

## ⚙️ How to Run
Clone this repository:

Bash
git clone https://github.com/Ayushi22jain/Flight-Price-Predection.git
Install dependencies:

Bash
pip install pandas numpy scikit-learn seaborn matplotlib openpyxl
Run the FlightPrice.ipynb notebook.

👤 Author
Ayushi Jain

GitHub: @Ayushi22jain



