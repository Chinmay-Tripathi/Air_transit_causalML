# Air_transit_causalML
This is the repository to manage the mini project of CausalML for Air Transit Delay.


## ✈️ Flight Delay Prediction using Machine Learning

This project focuses on predicting arrival delays of flights using machine learning algorithms. It uses a dataset containing detailed information about domestic flights, including carriers, departure/arrival times, delays, distance, and more.

## 📊 Dataset

The dataset used is from Kaggle's Flights Dataset, containing over 5 million records of U.S. domestic flights. Key features include:

    carrier – Two-letter airline code

    origin / dest – Airport codes

    dep_time / sched_dep_time – Actual and scheduled departure times

    dep_delay / arr_delay – Departure and arrival delays (in minutes)

    distance – Flight distance

    air_time – Actual flying time

## 🧹 Data Preprocessing & EDA

    Handled missing values by filling or replacing with logical estimates

    Imputed missing dep_time using sched_dep_time and set dep_delay to 0

    Performed label encoding on categorical features (carrier, origin, dest)

    Engineered new time-based features such as hour from sched_dep_time

    Visualized delay distributions and correlation heatmaps for exploratory insights

## 🤖 Machine Learning Models

The following regression models were used to predict `arr_delay`:

| Model              | MAE (↓) | R² Score (↑) |
|--------------------|---------|--------------|
| Random Forest      | 8.19    | 0.9471       |
| Gradient Boosting  | 11.78   | 0.9067       |
| XGBoost            | **5.22**| **0.9382**   |

XGBoost performed the best with the lowest Mean Absolute Error and a high R² score, indicating a strong fit.

## 📈 Goals

    Predict flight arrival delays with high accuracy

    Explore how different features influence delays

    Compare performance across multiple ML models

## 🛠️ Future Improvements

    Hyperparameter tuning using GridSearchCV

    Incorporating weather and air traffic data

    Deploying the model with a web-based interface for real-time prediction

## 📚 References

    Kaggle: US DOT Flight Delay Dataset

    Scikit-learn Documentation

    XGBoost Python API
