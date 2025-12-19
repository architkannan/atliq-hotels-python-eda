# AtliQ Hotels – Exploratory Data Analysis (Python)

A Python-based exploratory data analysis project focused on validating hospitality booking data and uncovering occupancy and revenue patterns across cities and room categories.

---

## ❗ Business Problem

AtliQ Hotels operates across multiple cities, offering diverse room categories and experiencing fluctuating demand patterns.

Before advanced dashboards or predictive models could be built, the leadership team needed clarity on:
- Whether booking and revenue data could be trusted
- Which room categories actually drive occupancy
- How occupancy and revenue vary by city
- Whether extreme revenue values reflected business reality or data issues

The primary challenge was **data reliability and insight extraction**, not prediction.

---

## 💡 How to Explore this Project

- Review the Jupyter Notebook sequentially to follow the analytical flow  
- Key insights are supported directly by code outputs and summary statistics  
- Data cleaning and validation steps are explained inline before analysis  
- The notebook is intended for **reading and understanding**, not deployment  

---

## 📝 Project Overview

This project performs a structured exploratory analysis to:
- Validate raw booking, revenue, and occupancy data
- Detect and correct data quality issues
- Analyze occupancy and revenue behavior by room category and city
- Integrate updated data to test the scalability of the analysis

**Goal:**  
Establish a clean and trustworthy analytical foundation to extract first-order business insights.

---

## 🔢 Data Sources

The analysis uses five core datasets:

- **fact_bookings** – Booking-level data including guests, revenue, ratings, and stay details  
- **fact_aggregated_bookings** – Aggregated occupancy metrics by room and date  
- **dim_hotels** – Hotel and city metadata  
- **dim_rooms** – Room category and class definitions  
- **dim_date** – Calendar mapping for time-based analysis  

An additional **August data refresh** was appended to validate data consistency and scalability.

---

## 🛠 Tools & Technologies

- Python  
- Pandas  
- NumPy  
- Jupyter Notebook  

---

## 🔍 Data Cleaning & Validation Approach

Key validation and cleaning steps included:

### 1. Structural Data Checks
- Identified and removed records with invalid guest counts (negative values)
- Verified missing ratings as expected behavior rather than data corruption

### 2. Revenue Outlier Treatment
- Detected extreme revenue values using statistical thresholds
- Removed records exceeding three standard deviations from the mean
- Validated remaining high-revenue records against premium room categories

### 3. Capacity Consistency Fixes
- Identified inconsistent capacity values in aggregated booking data
- Replaced anomalies using median capacity values by room category

This ensured analytical accuracy without distorting underlying business patterns.

---

## 📊 Key Insights

- **Occupancy varies significantly by room category**, indicating uneven demand across inventory types  
- **Revenue concentration is business-driven**, with higher values aligning to premium room classes rather than data errors  
- **City-level occupancy differences are material**, suggesting localized demand dynamics  
- **August data integrates cleanly**, confirming that the cleaned data structure scales with new inputs  

---

## 🧠 What This Project Demonstrates

- Strong data validation before analysis
- Practical use of statistics for anomaly detection
- Business-context-driven cleaning decisions
- Ability to prepare reliable datasets for downstream BI or modeling work

---

## ⚠️ Scope & Limitations

- No forecasting or predictive modeling
- No customer segmentation or pricing elasticity analysis
- No external seasonality or competitor data

These were intentional exclusions to maintain focus on data quality and exploratory insights.

---

## 🚀 Potential Extensions

- Time-series analysis of occupancy trends
- Revenue per Available Room (RevPAR) analysis
- City and room-category interaction analysis
- Power BI or Streamlit dashboards built on the cleaned dataset

---

## 📌 Deliverables

- Cleaned and validated datasets
- Python EDA notebook with documented logic
- Business-ready insights on occupancy and revenue structure

---

## ✔️ Conclusion

This project demonstrates my ability to:

1. Validate and clean raw operational data to ensure analytical reliability  
2. Use exploratory analysis to uncover occupancy and revenue patterns across cities and room categories  
3. Apply statistical reasoning to distinguish genuine business signals from data anomalies  
4. Prepare a trustworthy data foundation suitable for downstream BI, reporting, or modeling work  

---

### Contact  
🔗 **LinkedIn:** https://www.linkedin.com/in/architkannan/  
📧 **Email:** architkannan@zohomail.in  
