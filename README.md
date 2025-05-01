# ✈️ Flight Transit Delay Analysis using Causal Machine Learning

## 📌 Project Overview

This project investigates the causes of flight delays in U.S. domestic flights during 2019 using both traditional machine learning and **causal inference techniques**. While most models rely on correlation-based predictions, our goal is to uncover **true causal relationships** between variables like weather conditions, airport congestion, and scheduling, to better inform decisions in the aviation industry.

## 🎯 Objectives

- Predict flight delays using operational and weather data.
- Apply causal machine learning to identify true causes of delays.
- Compare traditional ML models (Random Forest, XGBoost) with causal models (DoubleML, Causal Forests).
- Offer interpretable and actionable insights for airlines and airport authorities.

## 🛠️ Methodology

1. **Data Preprocessing:** Cleaned and merged flight and weather datasets.
2. **Feature Engineering:** Added derived features such as `departure_hour`, `arrival_hour`, and `is_weekend`.
3. **Predictive Modeling:** Used Random Forest and XGBoost to establish performance baselines.
4. **Causal Analysis:**
   - Applied **DoWhy** for Average Treatment Effect (ATE) estimation.
   - Implemented **Double Machine Learning (DoubleML)** for robust treatment effect estimation.
   - Used **Causal Forests** to model heterogeneous treatment effects.

## 📊 Dataset

- **Source:** U.S. Domestic Flight Data (2019)
- **Rows:** ~72,000
- **Important Features:**
  - `departure_delay`, `arrival_delay`
  - `weather_conditions`, `airport_congestion`
  - `departure_hour`, `weekday`, `is_weekend`
  - Weather metrics: `HourlyPrecipitation`, `HourlyVisibility`, `HourlyWindSpeed`

## 📈 Results

Causal models successfully identified features that **directly impact delays**, such as weather conditions and departure time. This provides **actionable insights** over traditional black-box models and enables data-driven planning and intervention by airlines and airport authorities.

## 🧰 Tools & Libraries

- Python
- pandas, numpy, matplotlib, seaborn
- scikit-learn
- XGBoost
- [DoWhy](https://github.com/microsoft/dowhy)
- [DoubleML](https://github.com/DoubleML/doubleml-for-py)
- [EconML](https://github.com/microsoft/EconML)

## 🚀 How to Run

1. **Clone this repository:**
   ```bash
   git clone https://github.com/your-username/flight-delay-causal-ml.git
   cd flight-delay-causal-ml
2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt

3. **Run the code:**
   ```bash
   jupyter notebook FlightTransitDelay.ipynb

## License
This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for details.

## Auther
Chinmay Tripathi
