# 🚖 Not just rides — data.
### Analyzing Uber's ride-booking operations to answer why drivers cancel, where demand peaks, and which routes print money.

---

## 📌 Project Overview

This project analyzes ride-booking operations using transactional data from Uber, India's leading ride-hailing platform. The goal is to uncover insights into booking completion trends, cancellation patterns, revenue performance, and the impact of vehicle type, time-of-day, and ride distance on customer and driver experience — to guide strategic operational decisions.

---

## ❓ Problem Statement

**How can ride-booking operations be analyzed to improve booking completion rates, revenue optimization, and customer & driver experience?**

---

## 🗂️ Dataset Overview

| Feature Group | Columns |
|---|---|
| **Customer Details** | Customer ID, Customer Rating |
| **Vehicle Details** | Vehicle Type, Vehicle Images |
| **Booking Details** | Booking ID, Booking Status, Pickup Location, Drop Location, Date, Time, Payment Method, Booking Value, Ride Distance |
| **Operational Metrics** | V_TAT, C_TAT, Driver Ratings, Incomplete Rides Reason |
| **Cancellation Flags** | Canceled Rides by Customer, Canceled Rides by Driver, Incomplete Rides |

> **Missing Data:** Null values in `Incomplete_Rides_Reason`, `Canceled_Rides_by_Customer`, and `Canceled_Rides_by_Driver` are structurally valid — present only for cancelled or incomplete rides. No imputation required.

---

## 🛠️ Tech Stack

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-005C84?style=for-the-badge&logo=mysql&logoColor=white)
![Power BI](https://img.shields.io/badge/PowerBI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)

---

## 🔄 Project Workflow

```
Raw Data → Python (Clean & Engineer) → SQL (Analyze) → Power BI (Visualize) → Insights & Recommendations
```

### 1. 🐍 Data Preparation & Modeling (Python)
- Handled missing values across key columns
- Engineered new features: Time-of-Day slots, Ride Distance bins, Booking Value categories, Cancellation Source flags
- Exported clean dataset for SQL ingestion

### 2. 🗄️ Data Analysis (SQL)
- Booking completion rate by vehicle type
- Revenue breakdown by vehicle type and payment method
- Cancellation rate — Customer vs Driver
- Top pickup locations by demand
- Incomplete ride root cause analysis
- TAT analysis for successful rides

### 3. 📊 Visualization & Insights (Power BI)
- Interactive dashboard across all booking dimensions
- Revenue trends, driver scorecards, cancellation heatmaps
- Time-of-day demand patterns and rating distributions

### 4. 📝 Report & Recommendations
- Key findings summarized with data-backed recommendations
- Actionable insights on cancellation reduction, revenue optimization, and experience improvement

---

## 📊 Power BI Dashboard

> *(Dashboard screenshots)*

### Overview Page
<!-- Add your Power BI screenshot here -->
![Image Alt](https://github.com/Vansh-glitch1505/UBER-Performance-Analysis/blob/main/overview.jpeg?raw=true)

### Vehicle Type
<!-- Add your Power BI screenshot here -->
[![Ratings Dashboard](images/ratings_dashboard.png](https://github.com/Vansh-glitch1505/UBER-Performance-Analysis/blob/main/vehicle_type.jpeg?raw=true)

### Revenue Analysis
<!-- Add your Power BI screenshot here -->
[![Revenue Analysis](images/revenue_analysis.png)](https://github.com/Vansh-glitch1505/UBER-Performance-Analysis/blob/main/revenue.jpeg?raw=true)

### Cancellation Patterns
<!-- Add your Power BI screenshot here -->
[![Cancellation Patterns](images/cancellation_patterns.png)](https://github.com/Vansh-glitch1505/UBER-Performance-Analysis/blob/main/Cancellations.jpeg?raw=true)

)

---

## 💡 Key Findings

- 📍 **Booking Completion** — Identified which vehicle types have the highest and lowest completion rates
- 💰 **Revenue Leakage** — Quantified lost revenue from cancelled and incomplete rides
- ⏰ **Peak Demand** — Average booking value peaks at **1 PM (Hour 13)**
- 🚗 **Cancellation Source** — Analyzed whether customers or drivers cancel more and under what conditions
- ⭐ **Experience Gaps** — Highlighted vehicle types with below-average driver and customer ratings
- ⏱️ **TAT Impact** — Average vehicle TAT for successful rides is **170.62 seconds**

---

## 📢 Business Recommendations

- **Reduce Driver Cancellations** — Introduce penalty systems and incentive-based rewards for low cancellation rates
- **Capitalise on Peak Hours** — Deploy surge incentives and pre-shift driver notifications 30-60 minutes before demand peaks
- **Fix Incomplete Rides** — Address top incomplete ride reasons operationally to push completion rates above platform benchmark
- **Optimise High Revenue Vehicle Types** — Prioritise driver recruitment in top-earning categories
- **Improve TAT** — Reducing wait time by 20-30 seconds in high-demand zones can meaningfully improve customer ratings

---

## 📁 Repository Structure

```
uber-data-analysis/
│
├── data/
│   └── _bookings_clean.csv
│
├── python/
│   └── uber_analysis.ipynb.ipynb
│
├── images/
│   ├── dashboard_overview.png
│   ├── revenue_analysis.png
│   ├── cancellation_patterns.png
│   └── ratings_dashboard.png
│
└── README.md
```

---

## 🙋‍♂️ About Me

Aspiring Data Analyst passionate about turning raw data into actionable business insights.
Currently building my portfolio across SQL, Python, and Power BI.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)]([https://linkedin.com/in/your-profile](https://www.linkedin.com/in/vansh-rotkar-313530338/))
[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)]([https://github.com/your-username](https://github.com/Vansh-glitch1505))

---

*⭐ If you found this project helpful, consider giving it a star!*
