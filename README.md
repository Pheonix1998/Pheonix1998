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
## 📂 Featured Projects  
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

### 2. 🚖 Ride-Hailing Operations: Bottleneck & Revenue Leakage Analysis  

<a href="https://github.com/TATHAGATA23071998/PROJECTS/tree/main/RIDE%20SERVICE%20PROJECT">
<img src="https://img.shields.io/badge/Project_Repository-181717?style=for-the-badge&logo=github&logoColor=white">
</a>

**Tools Used:** SQL Server (SSMS) | Python (Pandas) | Tableau | Streamlit  

* **(a) Core Metrics Tracked:** * Total Booking Value (₹56.5M)
  * Successful Booking Rate (62.09%)
  * Total Ride Volume (103,024)
  * Driver Cancellation Rate

* **(b) The Business Decision (Problem Framing):**  Regional operations were experiencing a massive 38% ride failure rate. The executive team needed to definitively answer whether this was a demand-side marketing issue or a supply-side operational bottleneck in order to stop the ₹56.5M revenue leakage.

* **(c) Technical Execution & Analytical Judgment:**  Engineered a highly optimized Kimball Star Schema in SQL Server to process 100,000+ transaction records, ensuring executive BI dashboards loaded instantly.
  * Used analytical judgment to protect baseline volume metrics: instead of dropping rows with missing wait times (which would artificially shrink the total ride count), imputed missing values using statistical medians to preserve data integrity.
  * Architected a "Junk Dimension" to handle messy, unstructured cancellation text, drastically reducing the computational load on the central reporting database.

* **(d) Stakeholder Delivery & Outcomes:**  Delivered a top-down, interactive Tableau dashboard that proved the bottleneck was 100% supply-side, ruling out customer demand issues.
  * Uncovered widespread driver "gaming" behavior (accepting rides but refusing to move to force customer cancellations).
  * Correlated payment risk, proving that "Cash" payments generate high volume but carry the highest operational cancellation risk.

* **(e) Strategic Recommendations:**  Implement an algorithmic 3-minute GPS penalty to automatically reassign stationary drivers without penalizing the customer.
  * Launch aggressive customer discount campaigns for UPI payments to lock in platform revenue and eliminate the physical friction of cash on the street.

**Live Dashboards:**
* <a href="https://public.tableau.com/app/profile/tathagata.chakraborty5102/viz/RIDESERVICEANALYSISDASHBOARD/Dashboard" target="_blank"><img src="https://upload.wikimedia.org/wikipedia/commons/4/4b/Tableau_Logo.png" alt="My Tableau Profile" width="100"/></a>
* [![Streamlit](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://python-app-7a2zufxyiynnnvdy5glrcu.streamlit.app/)

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
![Stars](https://img.shields.io/github/stars/TATHAGATA23071998?style=for-the-badge)
![Followers](https://img.shields.io/github/followers/TATHAGATA23071998?style=for-the-badge)
![Profile Views](https://komarev.com/ghpvc/?username=Pheonix1998&style=for-the-badge)
![Primary Tools](https://img.shields.io/badge/Primary_Tools-EXCEL%20%7C%20SQL%20%7C%20PYTHON%20%7C%20STREAMLIT%20%7C%20TABLEAU-0B3C5D?style=for-the-badge)

---
