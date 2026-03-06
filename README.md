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
- Transform messy, fragmented datasets into reliable Single Sources of Truth for reporting**
- Design and develop interactive executive dashboards to track **KPIs and business health**
- Query and synthesize large-scale databases to **uncover hidden revenue drivers and operational bottlenecks**
- Perform predictive forecasting and trend analysis to guide proactive business strategies.
- Translate analytical results into **clear, business-focused recommendations for stakeholders**

---
## 📂 Featured Portfolio Projects  
<a href="https://github.com/Pheonix1998/PROJECTS">
<img src="https://img.shields.io/badge/All_Projects_Repository-181717?style=for-the-badge&logo=github&logoColor=white">
</a>

---

### 1. 🏃‍♂️ Health & Product Analytics: User Engagement Optimization

<a href="https://github.com/Pheonix1998/PROJECTS/tree/main/STRAVA%20PROJECT%20FILES">
<img src="https://img.shields.io/badge/Project_Repository-181717?style=for-the-badge&logo=github&logoColor=white">
</a>

**Tools:** Python | SQL (SQL Server) | Tableau | ETL Pipeline Design

* 🎯 **Core Metrics Tracked:** Peak Engagement Hours, Average Daily Caloric Burn, Step Volume, Sleep Efficiency.

* 📌 **The Business Decision:** The product and marketing teams needed to optimize push notification timing but lacked a "Source of Truth" due to highly fragmented user data spread across 18 separate files tracking events on different timelines.

* 🛠 **Technical Execution & ETL:**
  * Consolidated 11 distinct raw datasets into a highly optimized Master Fact Table at the daily granular level.
  * Aggregated highly granular second-by-second heart rate and minute-by-minute METs into standardized hourly averages.
  * Executed a `FULL OUTER JOIN` on the hourly timeline to prevent data loss, followed by a `LEFT JOIN` for daily metrics.
  * Handled missing activity with `0` and intelligently imputed missing heart rates using the user's personal historical average to protect mathematical integrity.

* 📊 **Stakeholder Delivery & Outcomes:** 
  * Built a 3-tier interactive Tableau dashboard tracking behavioral patterns.
  * Discovered the average user records **~7,765 steps** and burns **~2,339 calories** daily.
  * Identified that engagement volume spikes heavily in the late afternoon and early evening (**16:00 - 20:00**).
  * Discovered a mid-week engagement slump (Wednesday–Friday)
  * The vast majority of users are "Lightly Active" (sedentary/casual walking)


* 💡 **Strategic Recommendations:**
  * Target engagement bursts at peak hours (16:00-20:00) with short, contextual nudges.
  * Schedule social challenges on weekends to maximize baseline participation, retention, and viral spread.
  * Create features or premium offerings targeted for the premium customers (e.g., leaderboards, advanced metrics). 

 
* Tableau Dashboard - <a href="https://public.tableau.com/app/profile/tathagata.chakraborty5102/viz/STRAVAANALYSIS/Dashboard" target="_blank"><img src="https://upload.wikimedia.org/wikipedia/commons/4/4b/Tableau_Logo.png" alt="My Tableau Profile" width="200"/>
</a>

---

### 2. 🚖 Supply Chain & Operations: Ride-Hailing Bottleneck Analysis  

<a href="https://public.tableau.com/app/profile/tathagata.chakraborty5102/viz/OLADashboard/Dashboard">
<img src="https://img.shields.io/badge/Project_Repository-181717?style=for-the-badge&logo=github&logoColor=white">
</a>

**Tools Used:** Python | SQL | Streamlit | Data Visualization  

* 🎯 **Core Metrics Tracked:** Booking Conversion Rate, Revenue Leakage, Driver Cancellation Rate, Turnaround Time.

* 📌**The Business Decision:** Despite stable platform demand (~42K–46K rides/day), regional operations required a consolidated view to pinpoint bottlenecks, revenue drivers, and service quality gaps causing poor ride completion rates.

* 🛠 **Technical Execution:**
  * Evaluated end-to-end operations at the individual booking level using Python and SQL to explicitly identify cancellation drivers.
  * Segmented payment methods to mathematically correlate transaction types with operational reliability.
  * Visualized outputs in an interactive Streamlit application to enable real-time operational monitoring for branch managers.

* 📊 **Stakeholder Delivery & Outcomes:**
  * Identified massive revenue leakage: nearly **38%** of bookings do not convert into completed rides.
  * Found huge supply-side issue; the vast majority of customer cancellations (84,474 cases) occur because drivers do not move toward the pickup location.
  * Found that **Cash** payments generate high booking value but incur the highest operational risk, while **UPI** emerges as the most reliable payment method.

* 💡 **Strategic Recommendations:**
  * Introduce stricter penalties for frequent driver cancellations and improve real-time movement tracking.
  * Aggressively encourage UPI and digital payments to directly improve overall platform completion rates.
  * Demand is stable and operational control causes the bottleneck.


* Tableau Dashboard - <a href="https://public.tableau.com/app/profile/tathagata.chakraborty5102/viz/OLADashboard/Dashboard" target="_blank"><img src="https://upload.wikimedia.org/wikipedia/commons/4/4b/Tableau_Logo.png" alt="My Tableau Profile" width="200"/>
</a>


* Streamlit Dashboard - [![Streamlit](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://python-app-7a2zufxyiynnnvdy5glrcu.streamlit.app/)
---

### 3. 🎮 Market & Strategy Analytics: Product Profitability & ROI (Global Game Sales)

<a href="https://github.com/Pheonix1998/PROJECTS">
<img src="https://img.shields.io/badge/Project_Repository-181717?style=for-the-badge&logo=github&logoColor=white">
</a>

**Tools:** Python (Pandas) | SQL | Tableau | Exploratory Data Analysis (EDA)

* 🎯 **Core Metrics Tracked:** Global Sales Volume, Regional Market Share, Average Product Rating, Wishlist Velocity.

* 📌 **The Business Decision:** Marketing and development executives needed to identify top-tier revenue drivers and evaluate platform profitability to strategically guide future resource allocation and localized ad spend.

* 🛠 **Technical Execution:**
  * Processed disjointed product and sales datasets using Python to address missing values, handle data type inconsistencies, and correct structural errors.
  * Executed `INNER JOIN` logic in SQL to successfully unify game attributes with global sales performance and user engagement metrics.

* 📊 **Stakeholder Delivery & Outcomes:**
  * Engineered a dynamic Tableau dashboard facilitating exploratory market analysis.
  * Discovered the **Action ($661.65M)** and **Shooter ($400.68M)** genres are the primary global revenue drivers.
  * Identified the 'Sweet Spot': Titles rated between **3.5 and 4.0** generate the highest overall sales at **$1,058M**.

* 💡 **Strategic Recommendations:**
  * Implement a development **'Quality Gate'** to delay titles projected to score below 3.5, avoiding the steep revenue drop-offs observed with lower-rated games.
  * Avoid head-to-head competition with Nintendo's massive **46.30%** market share in the family-friendly niche by strategically pivoting to the Shooter genre.
  * Utilize pre-launch **'Wishlist Velocity'** as a leading indicator to accurately forecast demand and adjust physical copy production volumes.
 
* Tableau Dashboard - <a href="https://public.tableau.com/app/profile/tathagata.chakraborty5102/viz/GAMESALES_17696307297060/FULLEDA" target="_blank"><img src="https://upload.wikimedia.org/wikipedia/commons/4/4b/Tableau_Logo.png" alt="My Tableau Profile" width="200"/></a>

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
