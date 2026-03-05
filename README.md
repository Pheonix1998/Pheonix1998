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

## 1. 🏃‍♂️ Customer Fitness Application Analysis – Health & Engagement Optimization Project

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

### 📊 Tableau Executive Dashboard - 
<a href="https://public.tableau.com/app/profile/tathagata.chakraborty5102/viz/STRAVAANALYSIS/Dashboard" target="_blank">
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

## 2. 🚖 Ride-Hailing Operations Intelligence – Reducing Booking Failures & Revenue Leakage  
<a href="https://public.tableau.com/app/profile/tathagata.chakraborty5102/viz/OLADashboard/Dashboard">
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

## 📊 Dashboard Solutions - 
[![Streamlit](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://python-app-7a2zufxyiynnnvdy5glrcu.streamlit.app/)

<a href="https://public.tableau.com/app/profile/tathagata.chakraborty5102/viz/OLADashboard/Dashboard" target="_blank">
  <img src="https://upload.wikimedia.org/wikipedia/commons/4/4b/Tableau_Logo.png" alt="My Tableau Profile" width="200"/>
</a>

Developed interactive Tableau and Streamlit dashboard to monitor:

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


Here is your highly optimized GitHub README. It retains all your custom HTML badges and repository links while fundamentally restructuring the content into punchy, highly scannable bullet points.

It aligns perfectly with the **"Metrics-First"** and **"AI-Proof"** strategies from the videos, and incorporates the deep technical execution and strategic business recommendations directly from your PDF reports.

---

## 👋 Hi, I'm Tathagata Chakraborty

I am a **Business Intelligence & Operations Analyst** bridging the gap between raw data and executive decision-making. Operating with a "Data Product Manager" mindset, I focus on converting fragmented, real-world data into actionable insights that support **business decisions, operational efficiency, and measurable outcomes**.

### 🚀 About Me

* 🎓 **Education:** PGDM in Supply Chain & Analytics | M.Tech in Power Systems
* 🏦 **Background:** Former ICICI Bank professional (Asset & Liability Intern & SME Business Banking)
* 📊 **Technical Stack:** Advanced proficiency in SQL, Python, Excel, Power BI, Tableau, and statistical analysis
* 🔍 **Focus Areas:** ETL pipelines, KPI tracking, and decision support systems

### 💡 My Analytical Philosophy: The Metrics-First Approach

Before writing a single line of SQL or Python, I ensure I am crystal clear on:

* **The Decision:** Pinpointing the exact business choice the stakeholder is stuck on.
* **The Northstar KPIs:** Identifying the specific metrics that influence that decision, filtering out the noise.
* **The Trade-offs:** Balancing deep-dive technical analysis with speed-to-insight to meet real-world deadlines.

---

## 📂 Featured Portfolio Projects (Organized by Business Domain)

<a href="[https://github.com/Pheonix1998/PROJECTS](https://github.com/Pheonix1998/PROJECTS)">
<img src="[https://img.shields.io/badge/All_Projects_Repository-181717?style=for-the-badge&logo=github&logoColor=white](https://img.shields.io/badge/All_Projects_Repository-181717?style=for-the-badge&logo=github&logoColor=white)">
</a>

---

### 1. 🏃‍♂️ Health & Product Analytics: User Engagement Optimization (Strava)

<a href="[https://github.com/Pheonix1998/PROJECTS/tree/main/STRAVA%20PROJECT%20FILES](https://github.com/Pheonix1998/PROJECTS/tree/main/STRAVA%20PROJECT%20FILES)">
<img src="[https://img.shields.io/badge/Project_Repository-181717?style=for-the-badge&logo=github&logoColor=white](https://img.shields.io/badge/Project_Repository-181717?style=for-the-badge&logo=github&logoColor=white)">
</a>

**Tools:** Python (Pandas) | SQL (SQL Server) | Tableau | ETL Pipeline Design

* 🎯 **Core Metrics Tracked:** Peak Engagement Hours, Average Daily Caloric Burn, Step Volume, Sleep Efficiency.
* 📌 **The Business Decision:** The product and marketing teams needed to optimize push notification timing but lacked a "Source of Truth" due to fragmented user data across 18 separate files tracking events on completely different timelines.
* 🛠 **Technical Execution & ETL:**
*
* Consolidated 11 distinct raw datasets into a highly optimized Master Fact Table at the daily grain.
* Aggregated highly granular second-by-second heart rate and minute-by-minute METs into standardized hourly averages.
* Executed a `FULL OUTER JOIN` on the hourly timeline to prevent data loss, followed by a `LEFT JOIN` for daily metrics.
* Handled missing activity with `0` and imputed missing heart rates using the user's personal historical average.


* 📊 **Stakeholder Delivery & Outcomes:**
* Built a 3-tier interactive Tableau dashboard tracking behavioral cadence.
* Discovered the average user records ~7,765 steps and burns ~2,339 calories daily.
* Identified that engagement volume spikes heavily in the late afternoon and early evening (16:00 - 20:00).


* 💡 **Strategic Recommendations:**
* Recommended targeting engagement bursts at peak hours (16:00-20:00) with short, contextual nudges.
* Advised scheduling social challenges on weekends to maximize participation, retention, and viral spread.



---

### 2. 🚖 Supply Chain & Operations: Ride-Hailing Bottleneck Analysis (OLA)  

<a href="[https://public.tableau.com/app/profile/tathagata.chakraborty5102/viz/OLADashboard/Dashboard](https://public.tableau.com/app/profile/tathagata.chakraborty5102/viz/OLADashboard/Dashboard)">
<img src="[https://img.shields.io/badge/Project_Repository-181717?style=for-the-badge&logo=github&logoColor=white](https://img.shields.io/badge/Project_Repository-181717?style=for-the-badge&logo=github&logoColor=white)">
</a>

**Tools Used:** Python | SQL | Streamlit | Data Visualization  

* 🎯 **Core Metrics Tracked:** Booking Conversion Rate, Revenue Leakage, Driver Cancellation Rate, Turnaround Time.
* 📌 **The Business Decision:** Despite stable demand (~42K–46K rides/day), regional operations required a consolidated view to pinpoint bottlenecks, revenue drivers, and service quality gaps causing poor completion rates.
* 🛠 **Technical Execution:**
* Evaluated end-to-end operations at the individual booking level using Python and SQL to identify cancellation drivers.
* Segmented payment methods to correlate transaction types with operational reliability.
* Visualized outputs in an interactive Streamlit application to enable real-time operational monitoring.


* 📊 **Stakeholder Delivery & Outcomes:**
* Identified massive revenue leakage: nearly 38% of bookings do not convert into completed rides.
* Proved this is overwhelmingly a supply-side issue; most customer cancellations occur because drivers do not move toward the pickup location.
* Found that Cash payments generate high booking value but incur the highest operational risk, while UPI emerges as the most reliable payment method.


* 💡 **Strategic Recommendations:**
* Recommended introducing stricter penalties for frequent driver cancellations and improving real-time movement tracking.
* Advised aggressively encouraging UPI and digital payments to directly improve overall platform completion rates.



---

### 3. 🎮 Market & Strategy Analytics: Product Profitability & ROI (Global Game Sales)

<a href="[https://github.com/Pheonix1998/PROJECTS](https://github.com/Pheonix1998/PROJECTS)">
<img src="[https://img.shields.io/badge/Project_Repository-181717?style=for-the-badge&logo=github&logoColor=white](https://img.shields.io/badge/Project_Repository-181717?style=for-the-badge&logo=github&logoColor=white)">
</a>

**Tools:** Python (Pandas) | SQL | Tableau | Exploratory Data Analysis (EDA)

* 🎯 **Core Metrics Tracked:** Global Sales Volume, Regional Market Share, Average Product Rating, Wishlist Velocity.
* 📌 **The Business Decision:** Marketing and development executives needed to identify top-tier revenue drivers and evaluate platform profitability to guide resource allocation and localized ad spend.
* 🛠 **Technical Execution:**
* Processed disjointed product and sales datasets using Python to address missing values and correct structural errors.
* Executed `INNER JOIN` logic in SQL to unify game attributes with global sales performance and user engagement metrics.


* 📊 **Stakeholder Delivery & Outcomes:**
* Engineered a dynamic Tableau dashboard facilitating exploratory market analysis.
* Discovered the Action ($661.65M) and Shooter ($400.68M) genres are the primary global revenue drivers.



* Identified the 'Sweet Spot': Titles rated between 3.5 and 4.0 generate the highest overall sales at $1,058M.
* 💡 **Strategic Recommendations:**
* Recommended implementing a development 'Quality Gate' to delay titles projected to score below 3.5, avoiding steep revenue drop-offs.
* Advised avoiding head-to-head competition with Nintendo's massive 46.30% market share in the family-friendly niche by strategically pivoting to the Shooter genre.
* Suggested utilizing pre-launch 'Wishlist Velocity' as a leading indicator to forecast demand and adjust physical copy production volumes.



---

## 🖥️ Interactive Application-Based Dashboards

[](https://share.streamlit.io/?utm_source=streamlit&utm_medium=referral&utm_campaign=main&utm_content=-ss-streamlit-io-topright)
<a href="[https://public.tableau.com/app/profile/tathagata.chakraborty5102/vizzes](https://public.tableau.com/app/profile/tathagata.chakraborty5102/vizzes)" target="_blank">
  <img src="[https://upload.wikimedia.org/wikipedia/commons/4/4b/Tableau_Logo.png](https://upload.wikimedia.org/wikipedia/commons/4/4b/Tableau_Logo.png)" alt="My Tableau Profile" width="200"/>
</a>

---

## 🛠️ Tools & Skills

* **Languages & Tools:** SQL | Python | R | Excel | Power BI | Tableau | Streamlit
* **Analytics Concepts:** ETL Pipelines | Database Architecture | EDA | KPI Analysis | Business Metrics
* **Domain Exposure:** Banking | Ride-Hailing Operations | Health & Fitness Tracking | Retail Decision-Making

---

## 🤝 Let's Connect

<a href="[https://www.linkedin.com/in/tathagata-chakraborty-26b03a271/](https://www.linkedin.com/in/tathagata-chakraborty-26b03a271/)" target="_blank">
<img src="[https://img.shields.io/badge/LINKEDIN-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white](https://img.shields.io/badge/LINKEDIN-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)">
</a>
<a href="mailto:tathagata4059@gmail.com">
<img src="[https://img.shields.io/badge/EMAIL-D14836?style=for-the-badge&logo=gmail&logoColor=white](https://img.shields.io/badge/EMAIL-D14836?style=for-the-badge&logo=gmail&logoColor=white)">
</a>

---

## 📊 GitHub Stats
