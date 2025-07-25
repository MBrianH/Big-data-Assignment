
# 🚖 Uber Fares Data Analysis Project
**Course:** Introduction to Big Data Analytics INSY 8413

**Student:** Mutsinzi Brian Heritier
**Group:** B  
**Instructor:** Eric Maniraguha  
**Tool Used:** Python & Power BI  
**Dataset Source:** [Uber Fares Dataset on Kaggle](https://www.kaggle.com/datasets/yasserh/uber-fares-dataset)  
**Submission Deadline:** Friday, July 25, 2025 – Before Sabbath (5:00 PM)  

---

## 📌 Project Overview

This data analysis project focuses on Uber fares data to extract meaningful insights and patterns from ride transactions. Using Python for data preprocessing and Power BI for visual analytics, the objective is to understand how various temporal and geographic factors influence fare amounts. This end-to-end pipeline transforms raw CSV data into a professional dashboard and report offering operational recommendations for business improvement.

---

## 🎯 Objectives

- Explore fare trends based on time (hour, day, month)
- Identify peak/off-peak pricing patterns
- Uncover geographic ride hotspots using coordinate mapping
- Detect outliers and pricing anomalies
- Provide actionable business recommendations

---

## 🖼️ Documentation Screenshots

### 📥 1. Data Loading Process

> Dataset was first loaded in Python using pandas, and later imported into Power BI via CSV.

<img width="1127" height="533" alt="Load the dataset into a Pandas DataFrame" src="https://github.com/user-attachments/assets/d5842c61-e649-42ce-948d-b63e9dbcb6d6" />


---

### 🧹 2. Data Cleaning Steps

Data cleaning ensured the dataset was free from errors and suitable for analysis:

- Removed null values using `dropna()`
- Converted `pickup_datetime` to datetime
- Filtered out zero and negative fares
- Removed invalid coordinates (outside -90/90 and -180/180 range)

**Code and output:**

<img width="652" height="449" alt="Handle missing values and clean the data for analysis " src="https://github.com/user-attachments/assets/14d016e0-46a8-4ec9-9354-78288a779999" />

<img width="929" height="572" alt="Handle missing values and clean the data for analysis  output" src="https://github.com/user-attachments/assets/b565bd91-2da2-49f4-a119-b391249890a8" />

**Export the cleaned dataset as a CSV file for Power BI import **
<img width="592" height="111" alt="Export the cleaned dataset as a CSV file for Power BI import " src="https://github.com/user-attachments/assets/088512cc-422d-405a-9722-16d98c9c12c5" />

### 🧮 3. DAX Formulas (If Used)

While feature engineering was mostly done in Python, a few DAX measures were created in Power BI for enhanced analysis:

```DAX
Average Fare = AVERAGE('enhanced_uber'[fare_amount])
Ride Count = COUNT('enhanced_uber'[fare_amount])
```

These were used in line charts, bar charts, and KPI visuals.

---

### 📊 4. Dashboard Development Stages

> Built in Power BI Desktop, this dashboard contains time-based visuals, filters, and spatial maps for intuitive exploration of fare data.

📸 Final Dashboard Preview:

<img width="765" height="436" alt="DASHBOARD" src="https://github.com/user-attachments/assets/9d52683e-d342-4df2-9df2-1dda7bab3f79" />


#### Key Features:
- 📈 Line chart: Average fare over time
- 📊 Bar chart: Daily fare volume
- 🗺️ Map visual: Geographic ride locations

---

## 📈 Key Analytical Insights

- **Fare Distribution:** Majority of rides are between $6 and $12
- **Peak Fare Times:** 7–9 AM and 4–7 PM show higher fares
- **Weekend Pricing:** Fares increase slightly on Friday and Saturday
- **Geographic Hotspots:** Strong clustering around NYC
- **Outliers:** Fares above $22.25 identified as anomalies

---

## 💡 Recommendations

| Area                  | Recommendation                                       |
|-----------------------|------------------------------------------------------|
| Dynamic Pricing       | Focus on peak hour adjustments for demand control    |
| Driver Allocation     | More drivers on Fridays and during peak commute hours|
| Marketing Promotions  | Target off-peak hours with discounts                 |
| Anomaly Monitoring    | Flag and review extremely high fares regularly       |

---

