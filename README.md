# AtliQ Hotels - Booking, Occupancy, and Revenue Analysis using Python

A Python-based exploratory data analysis project focused on validating hospitality booking data and understanding how demand, occupancy, revenue, and customer experience vary across cities, hotel types, room categories, and booking platforms.

---

## ❗ Business Problem

AtliQ Hotels operates across multiple cities, offering both Luxury and Business hotels with varied room categories and demand patterns.

Before investing in dashboards or predictive models, leadership needed clarity on:
- Whether booking and revenue data could be trusted
- How demand is distributed across booking platforms
- Whether occupancy performance differs meaningfully by room type and city
- What actually drives revenue. Utilization or pricing
- Whether observed patterns are stable across time

The primary challenge was **data reliability and insight extraction**, not prediction.

---

## 💡 How to Explore this Project

- Review the Jupyter Notebook sequentially to follow the analytical flow  
- All insights are supported directly by computed values in the notebook  
- Data cleaning and validation steps precede any interpretation  
- The notebook is intended for **reading and understanding**, not deployment  

---

## 📝 Project Overview

This project performs a structured exploratory analysis to:
- Validate raw booking, revenue, and occupancy data
- Identify structural patterns in demand and utilization
- Compare occupancy, revenue, and ratings across cities
- Understand the role of booking platforms in volume and revenue
- Check whether insights hold consistently across months

**Goal:**  
Establish a clean, trustworthy analytical foundation and extract first-order business insights grounded in real operating data.

---

## 🔢 Data Sources

The analysis uses five core datasets:

- **fact_bookings**. Booking-level data including revenue, ratings, booking platform, and stay details  
- **fact_aggregated_bookings**. Aggregated occupancy metrics by room and date  
- **dim_hotels**. Hotel category and city metadata  
- **dim_rooms**. Room category definitions  
- **dim_date**. Calendar mapping for time-based analysis  

The data covers hotel check-ins from **May 1, 2022 to July 31, 2022**.

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
- Removed records with invalid guest counts
- Verified missing ratings as expected behavior rather than corruption

### 2. Revenue Outlier Treatment
- Identified extreme revenue values using statistical thresholds
- Removed records beyond three standard deviations
- Verified that remaining high values aligned with premium room categories

### 3. Capacity Consistency Fixes
- Detected inconsistent capacity values in aggregated data
- Replaced anomalies using median capacity by room category

This ensured analytical accuracy without distorting underlying business behavior.

---

## 📊 Key Insights. What the Data Is Really Saying

### 1. Demand is heavily platform-led rather than brand-led  
Between May and July, booking volume is dominated by third-party platforms:

- **Others** - 55,066 bookings  
- **MakeYourTrip** - 26,898 bookings  
- **LogTrip** - 14,756 bookings  

In contrast, **direct online and offline bookings combined account for ~20,000 bookings**.

This indicates that AtliQ’s demand engine is largely **intermediated**, limiting direct customer ownership and pricing control.

---

### 2. Room category occupancy is stable, not polarized  
Average occupancy across room categories is tightly clustered:

- Presidential - **59.30%**  
- Standard - **58.22%**  
- Elite - **58.04%**  
- Premium - **58.03%**

Despite differences in pricing and positioning, utilization remains nearly flat. This suggests that **pricing and mix**, rather than availability, are doing most of the revenue work.

---

### 3. Weekends drive performance. Weekdays underutilize capacity  
Occupancy splits sharply by day type:

- **Weekends** - **74.23%**  
- **Weekdays** - **51.82%**

A gap of over **22 percentage points** shows that demand is strongly leisure-driven. Core weekday capacity remains underutilized, especially relevant for Business-category hotels.

---

### 4. Delhi fills rooms better. Mumbai monetizes them better  
Average occupancy by city:

- Delhi - **61.61%**  
- Hyderabad - **58.14%**  
- Mumbai - **57.94%**  
- Bangalore - **56.59%**

Revenue tells a different story:

- Mumbai - **₹668.6M**  
- Bangalore - **₹420.4M**  
- Hyderabad - **₹325.2M**  
- Delhi - **₹294.4M**

Delhi leads on utilization, but Mumbai generates more than **2× Delhi’s revenue**, indicating stronger pricing power and revenue mix.

---

### 5. City-level differences persist within the same month  
June-only occupancy confirms these patterns are stable:

- Delhi - **61.46%**  
- Mumbai - **57.79%**  
- Hyderabad - **57.69%**  
- Bangalore - **55.95%**

This rules out seasonality noise and supports **city-specific strategy**, not a single national lever.

---

### 6. Luxury hotels generate disproportionate revenue  
Hotel portfolio composition:

- Luxury hotels - **16**  
- Business hotels - **9**

Revenue by hotel type:

- Luxury - **₹1,052.6M**  
- Business - **₹656.0M**

Despite similar occupancy behavior, Luxury hotels generate **~60% more revenue**, confirming that monetization, not utilization, is the primary driver.

---

### 7. Customer experience varies meaningfully by city  
Average ratings by city:

- Delhi - **3.78**  
- Hyderabad - **3.66**  
- Mumbai - **3.65**  
- Bangalore - **3.41**

Bangalore ranks lowest on both **ratings and occupancy**, suggesting experience quality may be constraining demand.

---

### 8. Revenue concentration mirrors booking concentration across platforms  
Revenue by booking platform closely follows volume patterns:

- Others - **₹699.3M**  
- MakeYourTrip - **₹340.8M**  
- LogTrip - **₹187.5M**  
- Direct online + offline - **~₹255.3M**

This reinforces platform dependency as a structural risk.

---

## 🧠 What This Project Demonstrates

- Translating raw booking data into business diagnosis
- Using numbers to separate utilization issues from pricing effects
- Identifying platform dependency risks using volume and revenue data
- Framing city-level performance differences with evidence
- Building trust in insights through disciplined validation

---

## ⚠️ Scope & Limitations

- No forecasting or causal modeling
- No customer segmentation or price elasticity analysis
- No external demand or competitor data

These were deliberate exclusions to focus on diagnostic clarity.

---

## 🚀 Potential Extensions

- Weekday-focused demand stimulation analysis
- RevPAR and contribution margin analysis
- Platform-level commission impact modeling
- Power BI or Streamlit dashboards built on cleaned data

---

## 📌 Deliverables

- Cleaned and validated datasets
- Python EDA notebook with documented logic
- Insight-driven diagnosis of demand, utilization, and revenue structure

---

## ✔️ Conclusion

This project demonstrates my ability to:

1. Validate and clean raw hospitality data to ensure analytical reliability  
2. Use exploratory analysis to diagnose demand, utilization, and monetization patterns  
3. Ground business insights in clearly computed metrics rather than assumptions  
4. Build a trustworthy foundation for downstream BI, reporting, or strategy work  

---

### Contact  
🔗 **LinkedIn:** https://www.linkedin.com/in/architkannan/  
📧 **Email:** architkannan@zohomail.in  
