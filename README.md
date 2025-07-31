# 📊 Natural Gas Price Forecasting & Storage Contract Analysis

A two-stage modeling project that forecasts natural gas prices and evaluates gas storage contract value based on injection/withdrawal strategy, price curves, and storage constraints.

---

## 📁 Dataset Overview

- **Source**: Monthly spot prices of natural gas.
- **Columns**:
  - `Dates` – Monthly frequency from Oct 2020 to Sep 2024.
  - `Prices` – Commodity prices in USD or equivalent per unit.

---

## 🎯 Project Objectives

This project has two major components:

1. **Natural Gas Price Forecasting**
   - Analyze seasonality and trends.
   - Predict prices for future dates.
   - Provide continuous pricing via interpolation.

2. **Storage Contract Pricing**
   - Simulate gas injection and withdrawal decisions.
   - Account for rate constraints, volume caps, and storage costs.
   - Evaluate total profit or loss from a given contract strategy.

---

## ⚙️ Methodology

### 📈 Phase 1: Forecasting

- Parsed and indexed time-series data using `pandas`.
- Applied **linear interpolation** to estimate prices for arbitrary dates.
- Used **Exponential Smoothing** for future forecasts.
- Visualized:
  - Price trends over time.
  - Seasonal effects.
  - Forecast.

### 💰 Phase 2: Pricing Model

-Simulates real-world injection (buy) and withdrawal (sell) of gas.
-Tracks volume and costs over time.
-Applies monthly storage costs.
-Returns:
  Total contract value

----

## 📈 Sample Results

<img width="748" height="363" alt="Natural Gas Price Forecast" src="https://github.com/user-attachments/assets/730a146b-0997-4b9b-bc0f-f386deb3ea69" />

Estimated gas prices:

| Date         | Estimated Price (USD) |
|--------------|------------------------|
| 2022-06-15   | $10.55                 |
| 2024-10-31   | $11.99                 |
| 2025-07-31   | $12.21                 |

Total contract value: 150

----

## 📊 Key Insights

Seasonality Observed: Prices peak during winter (Oct–Feb), suggesting seasonal demand cycles.

Forecasting Helps: Anticipated prices aid in choosing injection and withdrawal dates for profit.

Storage Optimization: Profits arise when gas is bought low, stored, and sold high — but only if storage costs and limits are managed well.

Strategic Contracting: The model enables "what-if" analysis for clients or internal traders.

----

## 📬 Contacts 

**Gaurav Mishra**  
📧 Email:7mishragaurav@gmail.com
🌐 LinkedIn: (www.linkedin.com/in/gaurav-mishra-3788ba271)
🐙 GitHub: (https://github.com/mishragaurav7)

---



