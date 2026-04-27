# Flight Price Prediction ✈️





     
Predicting flight ticket prices is a classic but challenging problem because prices change dynamically based on time, airline, and route. This project uses Machine Learning to find patterns in historical data and estimate future ticket costs.

## 🧐 Problem Statement
The goal is to build a regression model that can predict the price of a flight based on various factors like the date of journey, duration, source/destination, and the number of stops.

## 🚀 Step-by-Step Workflow

### 1. Data Exploration & Cleaning (EDA)
* **Time Conversion:** Transformed raw 'Date_of_Journey' into separate 'Day' and 'Month' columns so the model can understand seasonal trends.
* **Duration Extraction:** Converted "2h 50m" format into total minutes to make it a mathematical feature.
* **Missing Values:** Handled any null entries in the dataset to ensure model stability.

### 2. Feature Engineering & Preprocessing
* **Categorical Encoding:** * **One-Hot Encoding:** Used for nominal data (Airlines, Source) where there is no inherent order.
    * **Label Encoding:** Used for ordinal data (Total_Stops) where the number of stops has a direct impact on price.
* **Feature Selection:** Not all data is useful. I used **ExtraTreesRegressor** and **Heatmaps** to visualize which features (like duration or total stops) actually influence the price the most.

### 3. Model Building: Random Forest Regressor
I chose **Random Forest** because it:
* Handles non-linear data exceptionally well.
* Is an ensemble method (combines multiple decision trees) which reduces the risk of overfitting.
* **Hyperparameter Tuning:** Used `RandomizedSearchCV` to find the best settings for the model (n_estimators, max_depth, etc.) to get the lowest possible error.

## 🛠️ Tech Stack
* **Language:** Python 3.x
* **Analysis:** Pandas, NumPy
* **Visualization:** Matplotlib, Seaborn
* **ML Framework:** Scikit-learn
* **Deployment:** Flask (Web API)

## 📁 Repository Structure
* `flight_price.ipynb`: The core logic, data cleaning, and training.
* `app.py`: The Flask backend that serves the model.
* `home.html`: The user interface where you input flight details.
* `Data_Train.xlsx`: Historical training data.

## ⚙️ How to Setup
1. **Clone:** `git clone https://github.com/Ayushi22jain/Flight-Price-Predection.git`
2. **Install:** `pip install pandas scikit-learn seaborn matplotlib flask openpyxl`
3. **Launch UI:** `python app.py`

## 👤 Author
**Ayushi Jain**
GitHub: [@Ayushi22jain](https://github.com/Ayushi22jain)
