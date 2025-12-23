# Explatory Data Analysis and ML models for Used Car Price Prediction

## 📋 Project Overview
This project aims to solve the pricing volatility in the Indian pre-owned car market for **Cars4U**, a budding tech start-up. Unlike new cars, used car pricing is non-deterministic. By leveraging machine learning, I developed a model to predict vehicle prices accurately, allowing for data-driven acquisition and sales strategies.

## 🎯 Business Objective
To build a robust pricing model that:
1.  **Predicts** used car prices based on vehicle attributes.
2.  **Identifies** key drivers of vehicle value to support differential pricing.
3.  **Optimizes** inventory acquisition by identifying underpriced market listings.

## 📊 Key Findings & Model Performance
The **Linear Regression model** was selected as the best-performing algorithm due to its high explainability and strong performance metrics:
* **Accuracy:** Explains **~94.75%** of the variance in training data and **~89.57%** in test data.
* **Error:** Achieved an **RMSE of 3.72 (Lakhs)** on the test set.
* **Robustness:** While showing mild overfitting, the model remains highly effective for business decision-making.

### 🔑 Key Drivers of Price
* **Power & Engine:** Strongest positive predictors; higher BHP and Engine CC significantly increase resale value.
* **Vehicle Age:** Prices depreciate most sharply after the first **4–5 years**.
* **Transmission:** Automatic variants command a significantly higher market value across all segments.
* **Fuel Type:** Diesel vehicles retain higher value than Petrol, while Electric cars occupy a high-price niche.
* **Ownership:** "First-hand" status is a premium; each additional owner significantly reduces the predicted price.

## 💡 Strategic Recommendations for Cars4U
1.  **Arbitrage Opportunity:** Use the model to identify "underpriced" cars (where market price < predicted price) for high-margin acquisition.
2.  **Inventory Redistribution:** Leverage geographical price variances. The data shows cities like **Coimbatore and Bangalore** have higher price coefficients than Kolkata or Jaipur. Cars4U should consider transferring inventory to these high-demand locations to maximize ROI.
3.  **Risk Mitigation:** Prevent overpayment for inventory with high "hidden" depreciation factors identified by the model (e.g., high mileage combined with multiple owners).

## 🛠️ Tech Stack
* **Language:** Python
* **Analysis:** Pandas, NumPy, Matplotlib, Seaborn
* **Modeling:** Scikit-learn, Statsmodels (OLS Regression), Linear Regression, Decision Tree, Random Forest, Hyperparameter Tuning
