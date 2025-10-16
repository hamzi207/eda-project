# 🏠 Real Estate Market Analysis for Charles Christensen

**Goal:**  
Identify undervalued properties and optimal selling months for maximum ROI using exploratory data analysis and predictive modeling.

---

## 📊 Project Overview

This project analyzes housing sales data from **King County** to support real-estate investment decisions.  
The stakeholder, **Charles Christensen**, is an investor aiming to identify profitable resale opportunities and favorable sale timings.

---

## 🧩 Dataset

**Source:** Provided CSV files (`king_county_house_sales_*.csv`)  
**Rows:** 21,597  
**Main features:**

- `sqft_living`, `bedrooms`, `bathrooms`
- `grade`, `condition`, `view`, `waterfront`
- `yr_built`, `yr_renovated`
- `zipcode`, `lat`, `long`
- Target variable: `price`

---

## ⚙️ Workflow

1. **Setup & Imports** – Load required Python libraries.
2. **Data Loading & Cleaning** – Merge datasets, handle missing values, engineer new features (`renovated`, `month_sold`).
3. **Exploratory Data Analysis (EDA)** – Visualize distributions, correlations, and price drivers.
4. **Feature Engineering** – Encode categorical features, apply `log(price)` transformation.
5. **Modeling** – Train linear regression on log-transformed price (R² ≈ 0.77).
6. **Evaluation** – Actual vs Predicted and Residual plots confirm reliable model performance.
7. **Investment Scenarios** – Simulate seasonal price variations and identify top 3 undervalued properties.
8. **Insights & Recommendations** – Business-oriented findings for Charles.

---

## 📈 Key Results

| Metric                    | Result      | Meaning                              |
| ------------------------- | ----------- | ------------------------------------ |
| **R²**                    | 0.77        | Model explains 77% of price variance |
| **MAE**                   | ~$78,000.00 | Average prediction error of ±14%     |
| **Best Selling Month**    | **June**    | Highest predicted sale price         |
| **Least Favorable Month** | **January** | Lowest predicted sale price          |

**Top 3 Investment Zipcodes:** `98004`, `98006`, `98033`  
**Exported Report:** `investment_report_charles_christensen.csv`

---

## 💡 Insights

- Larger living areas and higher construction grades significantly raise property value.
- Renovations yield clear returns — upgraded homes are priced 10–15% higher on average.
- Premium zipcodes and properties with views command strong price premiums.
- June is the most favorable month for selling, while January has the weakest market activity for selling but better opportunities for buying & investments.

---

## 💼 Recommendations

1. Focus investments on high-grade homes with renovation potential.
2. Acquire properties in profitable neighborhoods (98004, 98006, 98033).
3. Plan resales around **June** for peak returns.
4. Avoid January listings when buyer demand is low.
5. Plan Investments/buying in January.
6. Use this predictive model for pre-purchase ROI estimation.

---

## 🧰 Tools Used

- **Python** (Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, GeoPandas)
- **Jupyter Notebook** for analysis and visualization
- **GitHub** for project version control and documentation
- **Google Slides** for presentations

---

## 📁 Repository Structure

📂 real-estate-analysis/
┣ 📜 EDA.ipynb
┣ 📜 README.md
