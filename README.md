## 👋 Hi, I'm Tathagata Chakraborty
I am a Business Analyst with hands-on experience across business banking, supply chain and analytics. I focus on converting raw data into actionable insights that support **business decisions, operational efficiency, and measurable outcomes**.

---

## 🚀 About Me
- 🎓 PGDM in **Supply Chain & Analytics**
- 🏦 Former **ICICI Bank** professional (MSME & Retail Banking)
- 📊 Strong working knowledge of **SQL, Python, Excel, Power BI, Tableau**, and statistical analysis
- 🔍 Interested in **data-driven strategy, process optimization, and decision support systems**

---

## 🧠 What I Deliver as a Business Analyst ?
- Clean, validate, and analyze data using **EDA techniques**
- Build **MIS reports and executive dashboards** for KPI tracking
- Write **SQL queries** for extraction, joins, aggregations, and insights
- Perform **forecasting and trend analysis** using Python and R
- Translate analytical results into **clear, business-focused recommendations**

---
## 📂 Featured Portfolio Projects  
<a href="https://github.com/Pheonix1998/PROJECTS">
<img src="https://img.shields.io/badge/All_Projects_Repository-181717?style=for-the-badge&logo=github&logoColor=white">
</a>

---

## 3. 🏃‍♂️ STRAVA Customer Analysis – Health & Engagement Optimization Project

<a href="https://github.com/Pheonix1998/PROJECTS/tree/main/STRAVA%20PROJECT%20FILES">
<img src="https://img.shields.io/badge/Project_Repository-181717?style=for-the-badge&logo=github&logoColor=white">
</a>

**Tools:** Python (Pandas) | SQL (SQL Server) | Tableau | ETL Pipeline Design

---

### 📌 Why This Project?

This project demonstrates the ability to handle complex **Data Engineering and ETL (Extract, Transform, Load)** pipelines before any visualization occurs.

Instead of starting with a clean dataset, the focus was on:
- Architecting a unified data model from messy, multi-grain sources
- Preventing Cartesian explosions and data duplication
- Building a scalable **Master Fact Table** optimized for BI reporting

---

### 🎯 Business Problem

The raw customer health and activity data was fragmented across **18 separate files** tracking events on completely different timelines (e.g., daily weight logs, hourly steps, and second-by-second heart rates).

The main challenges were:
- Directly joining these tables in SQL would cause massive data duplication
- Null values and missing inputs threatened to break mathematical averages (e.g., a "0" for heart rate ruins physiological trendlines)
- The business lacked a single "Source of Truth" to answer core operational questions

Because of this, it was impossible to track intraday behaviors or correlate health domains (like sleep vs. activity).

The business needed:
- A single, blank-free Master Fact Table
- Clear visibility into peak engagement hours
- Reliable segmentation of workout intensity (casual walking vs. intense cardio)
- Insights into how recovery (sleep) impacts physical exertion

---

### 🛠 My Approach

#### 1️⃣ Data Selection & Deduplication
- Audited 18 raw datasets and scaled down to the **11 most relevant files**
- Dropped pre-aggregated files to prevent redundancy
- Excluded overly noisy minute-level sleep logs to focus strictly on executive-level KPIs

#### 2️⃣ Engineered a Python ETL Pipeline
- **Granularity Alignment:** Aggregated second-level heart rate and minute-level METs into standardized hourly averages
- **Collision Prevention:** Renamed overlapping columns (e.g., `Calories` to `HourlyCalories` and `DailyCalories`)
- **The Master Join:** Executed a `FULL OUTER JOIN` on the hourly timeline, followed by a `LEFT JOIN` for daily metrics
- **Smart Imputation:** Handled missing activity with `0`, and imputed missing heart rates using the user's *personal historical average* to protect mathematical integrity

#### 3️⃣ Database Integration (SQL Server)
Created a rigid database schema to bypass SSMS import errors caused by messy data:
- Mapped IDs to `BIGINT`
- Forced timestamps to `DATETIME` (avoiding the binary timestamp trap)
- Set activity metrics to `FLOAT` for seamless decimal conversions

#### 4️⃣ Performed Business-Focused Analysis
**Engagement Insights**
- Peak intraday engagement hours
- Weekly activity trends (Weekend vs. Mid-week)
- Total active users and daily average steps

**Exertion Insights**
- Distance segmented by intensity (Very Active vs. Lightly Active)
- Caloric burn correlated with total distance
- Top 10 "Super Users" by total steps

**Health & Recovery Insights**
- Average resting and peak heart rates
- Sleep efficiency (Time in Bed vs. Time Asleep)
- Impact of sleep duration on next-day activity levels

---

### 📊 Tableau Executive Dashboard - <a href="https://public.tableau.com/app/profile/tathagata.chakraborty5102/viz/STRAVAANALYSIS/Dashboard" target="_blank">
  <img src="https://upload.wikimedia.org/wikipedia/commons/4/4b/Tableau_Logo.png" alt="My Tableau Profile" width="200"/>
</a>
Built a 3-tier interactive Tableau dashboard to translate the Fact Table into visual insights.

**Dashboard Highlights:**
- Top Row: Macro KPIs (Total Users, Avg Steps, Avg Calories, Avg Sleep Duration)
- Middle Row: Behavioral Cadence (Area charts mapping peak hours and weekly step trends)
- Bottom Row: Exertion Quality (Stacked bar charts separating casual walking from intense cardiovascular distance)
- Super User Leaderboard

---

### 📈 Key Outcomes
- Built a clean, blank-free hourly Master Fact Table from 11 disjointed sources
- Eliminated data collisions and Cartesian explosions
- Identified a massive volume spike in user activity between 4:00 PM and 8:00 PM
- Discovered a mid-week engagement slump (Wednesday–Friday)
- Proved that the vast majority of user distance is "Lightly Active" (sedentary/casual walking)

---
---

## 🚖 Ride-Hailing Operations Intelligence – Reducing Booking Failures & Revenue Leakage  
<a href="https://github.com/Pheonix1998/PROJECTS/tree/main/OLA%20Service%20Dashboard">
<img src="https://img.shields.io/badge/Project_Repository-181717?style=for-the-badge&logo=github&logoColor=white">
</a>

**Tools Used:** Python | SQL | Streamlit | Data Visualization  

---

## 📌 Project Context

This project analyzes end-to-end booking data from a ride-hailing platform to understand:

- Why bookings fail  
- Where revenue is leaking  
- How driver behavior impacts performance  
- How payment method affects ride completion  

The focus was operational efficiency and revenue realization — not just dashboard creation.

---

## 🎯 Core Business Problem

Although demand was stable, nearly **38% of bookings were not converting into completed rides**.

This indicated:

- Revenue leakage  
- Operational inefficiencies  
- Driver accountability gaps  
- Customer dissatisfaction  

The business needed a consolidated view of:

- Booking success vs failure  
- Cancellation drivers  
- Vehicle-wise performance  
- Payment reliability  
- Rating mismatches  

---

## 🛠 Analytical Approach

### 1️⃣ Demand & Volume Analysis

- Daily rides remained stable (~42K–46K per day)
- No major spikes or drops
- Slight increase at month-end

**Insight:** Demand is consistent. The issue is not customer demand — it is operational execution.

---

### 2️⃣ Booking Outcome Analysis

Booking distribution:

- 62.06% Completed
- 17.90% Driver Cancelled
- 10.20% Customer Cancelled
- 9.85% Driver Not Found

**Key Finding:**  
Driver-side issues (cancellations + not found ≈ 28%) dominate ride failures.

Revenue loss is primarily supply-driven, not demand-driven.

---

### 3️⃣ Cancellation Root Cause

**Customer Cancellations:**
- Main reason: Driver not moving toward pickup (largest volume)
- Minor reasons: change of plans, AC issues, wrong address

**Driver Cancellations:**
- Mostly due to personal or vehicle-related issues
- Very low customer-related cancellation triggers

**Conclusion:**  
Operational discipline and driver readiness are major improvement areas.

---

### 4️⃣ Vehicle Performance Analysis

- Premium vehicles (Prime categories) complete longer trips
- Auto and Bike show shorter distances
- Incomplete rides are mostly short-distance trips
- Premium segments show slightly better rating alignment

**Insight:** Higher incentives improve completion rates.

---

### 5️⃣ Payment Method Analysis

- Cash generates high booking value but high cancellations
- UPI shows high value with better completion rates
- Cards contribute minimal share

**Business Interpretation:**  
Digital payments are more reliable. Cash rides increase operational risk.

---

### 6️⃣ Rating & Experience Alignment

- Average ratings are around 4.0 across vehicles
- Rating gaps observed in some categories
- Negative gap = Customer dissatisfaction
- Positive gap = Driver dissatisfaction

Service quality is stable, but perception gaps indicate training opportunities.

---

## 📊 Dashboard Solution - [![Streamlit](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://python-app-7a2zufxyiynnnvdy5glrcu.streamlit.app/)

  <img src="https://upload.wikimedia.org/wikipedia/commons/4/4b/Tableau_Logo.png" alt="My Tableau Profile" width="200"/>
</a>
Developed an interactive Streamlit dashboard to monitor:

- Booking success rate  
- Cancellation breakdown  
- Revenue leakage  
- Vehicle-wise performance  
- Payment method contribution  
- Rating distribution  
- Rating gap analysis  

Filters include:
- Date
- Vehicle type
- Payment method
- Booking status  

This enables real-time operational monitoring.

---

## 📈 Key Business Insights

- 38% booking conversion loss is the biggest revenue risk  
- Driver-related issues cause most failures  
- “Driver not moving” is the top customer frustration  
- Cash payments increase cancellation probability  
- Premium segments perform more efficiently  
- Demand is stable — operational control is the bottleneck  

---

## 💡 Strategic Recommendations

- Introduce stricter penalties for frequent driver cancellations  
- Improve real-time driver movement tracking  
- Encourage UPI and digital payments  
- Monitor high-risk drivers using performance dashboards  
- Improve driver readiness checks before ride acceptance  
- Provide targeted training for low-performing vehicle segments  

---

## 🚀 What This Project Demonstrates

- Operational problem-solving  
- KPI-driven analysis  
- Root cause thinking  
- Revenue impact quantification  
- Driver behavior analysis  
- Business-focused dashboard design  

---
## 🖥️ Interactive Application-Based Dashboards
[![Streamlit](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://share.streamlit.io/?utm_source=streamlit&utm_medium=referral&utm_campaign=main&utm_content=-ss-streamlit-io-topright)

<a href="https://public.tableau.com/app/profile/tathagata.chakraborty5102/vizzes" target="_blank">
  <img src="https://upload.wikimedia.org/wikipedia/commons/4/4b/Tableau_Logo.png" alt="My Tableau Profile" width="200"/>
</a>

---
## 🛠️ Tools & Skills

**Languages & Tools:**  
SQL | Python | R | Excel | Power BI | Tableau  

**Analytics Concepts:**  
EDA | Forecasting | KPI Analysis | OLAP vs OLTP | Business Metrics  

**Domain Exposure:**  
Banking | Operations | Supply Chain Analytics | Retail Decision-Making  

---

## 🤝 Let's Connect
<a href="https://www.linkedin.com/in/tathagata-chakraborty-26b03a271/" target="_blank">
<img src="https://img.shields.io/badge/LINKEDIN-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white">
</a>

<a href="mailto:tathagata4059@gmail.com">
<img src="https://img.shields.io/badge/EMAIL-D14836?style=for-the-badge&logo=gmail&logoColor=white">
</a>

---

## 📊 GitHub Stats
![Stars](https://img.shields.io/github/stars/Pheonix1998?style=for-the-badge)
![Followers](https://img.shields.io/github/followers/Pheonix1998?style=for-the-badge)
![Profile Views](https://komarev.com/ghpvc/?username=Pheonix1998&style=for-the-badge)
![Primary Tools](https://img.shields.io/badge/Primary_Tools-EXCEL%20%7C%20SQL%20%7C%20PYTHON%20%7C%20STREAMLIT%20%7C%20TABLEAU-0B3C5D?style=for-the-badge)

---
