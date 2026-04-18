# 🚕 NYC Taxi Trips Analysis: Demand Trends & Pricing Insights

## 📌 Project Overview

This project explores New York City taxi trip data to uncover **demand patterns, pricing behavior, and trip characteristics**.
The goal is to transform raw data into meaningful insights that can support **operational decisions and business strategy**.

---

## 🎯 Objectives

* Analyze taxi demand across different **time periods (hour, weekday)**
* Understand factors influencing **fare and total cost**
* Identify **trip patterns and anomalies**
* Build an interactive **dashboard for visualization**

---

## 📂 Dataset

* Source: Kaggle NYC Taxi Trip Dataset
* Size: **83,691 rows × 20 columns**

---

## 🧹 Data Cleaning & Preparation

* Converted datetime columns to proper format
* Created new features:

  * `pickup_hour`, `pickup_day`, `pickup_weekday`
  * `trip_duration`, `speed`, `is_weekend`
* Handled missing values:

  * Numerical → median
  * Categorical → mode
* Removed column:

  * `ehail_fee` (high missing rate)
* No duplicate records found

---

## 📊 Exploratory Data Analysis (EDA)

### 🚕 Trip Characteristics

* Most trips are **short-distance and low-cost**
* Fare typically ranges between **0–100**
* Some **outliers** in duration and fare

---

### ⏱ Time-Based Patterns

* Peak hours: **08:00 – 12:00**
* Peak days: **Thursday & Friday**
* Lowest activity: **Sunday & late night (00:00–05:00)**

---

### 💰 Relationships

* Distance and fare show a **positive but non-linear relationship**
* Pricing influenced by **base fare, tolls, and surcharges**

---

### 🔗 Correlation Highlights

* `fare_amount` ↔ `total_amount`: **0.98**
* `trip_type` ↔ `RatecodeID`: **0.93**
* Moderate:

  * `speed` ↔ `trip_distance`: **0.61**

---

## 🧠 Key Insights

* Taxi demand is strongly influenced by **time (hour & weekday)**
* Most trips are **short and local**
* Pricing is **not strictly distance-based**
* Nighttime demand is significantly lower
* Tolls and additional fees impact total cost

---

## 📊 Dashboard

An interactive dashboard was created using **Tableau** to visualize:

* Trips by hour and weekday
* Fare and distance distributions
* Distance vs fare relationship
* Key KPIs (Total trips, average fare, etc.)

---

## 🛠 Tools & Technologies

* Python (Pandas, NumPy, Matplotlib, Seaborn)
* Tableau (Dashboard & Visualization)
* Jupyter Notebook


---

## 📌 Conclusion

This analysis highlights how taxi demand varies across time and how pricing is influenced by multiple factors beyond distance.
The insights can help improve **resource allocation, pricing strategies, and service efficiency**.

---

## 🚀 Future Improvements

* Add geospatial analysis (pickup/dropoff locations)
* Build predictive models (fare or demand prediction)
* Enhance dashboard with interactive filters

---


