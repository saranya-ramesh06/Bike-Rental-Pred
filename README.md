# Bike Rental Demand Prediction

## 📌 Project Overview

This project focuses on predicting bike rental demand using machine learning algorithms. The dataset includes both *hourly* and *daily* rental information. The project involves data merging, feature extraction, exploratory data analysis (EDA), and model training to determine the most accurate predictive model. The insights obtained can assist bike rental companies in understanding rental patterns and optimizing their operations.

## 🔊 Dataset Information

- *Datasets Used*:
  - day.csv: Contains daily bike rental data.
  - hour.csv: Contains hourly bike rental data.

- *Key Features*:
  - instant: Record index
  - dteday: Date
  - season: Season (1:spring, 2:summer, 3:fall, 4:winter)
  - yr: Year (0: 2011, 1: 2012)
  - mnth: Month (1 to 12)
  - hr: Hour (0 to 23)
  - holiday: Whether the day is a holiday (1: Yes, 0: No)
  - weekday: Day of the week
  - workingday: Whether the day is a working day (1: Yes, 0: No)
  - weathersit: Weather situation (1: Clear, 2: Misty, 3: Light Snow/Rain, 4: Heavy Rain)
  - temp: Normalized temperature
  - atemp: Normalized feeling temperature
  - hum: Normalized humidity
  - windspeed: Normalized windspeed
  - casual: Count of casual users
  - registered: Count of registered users
  - cnt: Total count of rentals (Target Variable)

## 🔍 Exploratory Data Analysis (EDA)

- *Merging Datasets*: Hourly and daily datasets were merged to enrich the feature set for better model predictions.
- *Data Cleaning*:
  - Checked and handled missing values.
  - Converted date columns to datetime format.
- *Feature Engineering*:
  - Extracted features like day of the week, time of day, and seasonal trends.
  - Created new features such as peak hour, weekend/weekday categorization.
- *Visualizations*:
  - Line plots to show daily rental trends.
  - Heatmaps for correlation analysis.
  - Distribution plots to analyze target variable skewness.
  - Box plots to visualize relationships between categorical features and rental counts.

## 🤖 Machine Learning Models Used

Several models were trained to compare their performance:

1. *Linear Regression*
2. *Decision Tree Regressor*
3. *Random Forest Regressor*
4. *Gradient Boosting Regressor*
5. *XGBoost Regressor*
6. *K-Nearest Neighbors (KNN) Regressor*

## 📈 Model Evaluation Metrics

- *Mean Absolute Error (MAE)*
- *Mean Squared Error (MSE)*
- *Root Mean Squared Error (RMSE)*
- *R² Score*

## 🛠 Hyperparameter Tuning
- Utilized *GridSearchCV* and *RandomizedSearchCV* for tuning hyperparameters.
- Optimized models for better performance and reduced overfitting.

## 🚀 How to Run the Project

### 1️⃣ Install Dependencies
bash
pip install -r requirements.txt


### 2️⃣ Run the Jupyter Notebook
bash
jupyter notebook PRCP-1018-BikeRental.ipynb


## 📌 Key Insights

- *Peak Rental Hours*: Most rentals occur during morning and evening peak hours, aligning with typical commuting times.
- *Weather Impact*: Rentals significantly decrease during poor weather conditions (e.g., heavy rain).
- *Seasonal Trends*: Summer and fall seasons observe higher rental counts compared to winter.
- *Working Days vs. Holidays*: Rentals are higher on working days, indicating a large portion of rentals is for commuting.
- *Temperature Influence*: Higher temperatures correlate with increased rentals, though extreme heat can reduce demand.
- *Random Forest and XGBoost Models* yielded the highest accuracy in predictions, indicating their robustness for this problem.

## 📄 Conclusion

This project successfully developed a predictive model for bike rental demand. The analysis identified key influencing factors like weather, seasonality, and time of day. These insights can help rental companies optimize fleet distribution, pricing strategies, and marketing campaigns.

---
