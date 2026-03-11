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

* **(a) Core Metrics Tracked:**
  * Average Daily Steps (~7,765)
  * Average Active Minutes (~231)
  * Total Unique Users (33)
  * Average sleep time (~5.8 hrs)

* **(b) The Business Decision (Problem Framing):** The company suffered from severe mid-week loss of activity and reduced user engagements which led to customer           churn. The objective was to pivot from a "tracker" to an active "health partner", increasing Customer Lifetime Value (CLTV).

* **(c) Technical Execution & Analytical Judgment:**
  * Designed a robust Python ETL pipeline to consolidate 11 distinct raw datasets into a single, daily-granular Master Fact Table.
  * Exercised strong analytical judgment during data cleaning: rather than filling missing heart rate data with generic zeros (which would destroy the                 mathematical integrity of health metrics), imputed missing data using the user's specific historical averages.

* **(d) Stakeholder Delivery & Outcomes:**
  * **Biological Churn:** Correlated mid-week app churn directly to user "Sleep Data" (users averaged a dangerously low 5.8 hours of sleep).
  * **Domain Context (May 12th Anomaly):** A massive retention surge on *International Nurses Day*, revealing healthcare workers as the core "Power User".
  *   Identified a strict dual-peak activity rhythm—a mid-day lunch/rounds spike (12:00–14:00) and an end-of-shift spike (17:00–19:00)—confirming behavior is            highly constrained by professional work schedules.

* **(e) Strategic Recommendations:**
  * **Product Strategy:** Deploy a "Module" demonstrating how 30 extra minutes of sleep improves next-day productivity to protect mid-week retention.
  * **Marketing Strategy:** Confine push notifications strictly to the 12:00 PM lunch window and the 17:00 PM post-shift window, launching targeted B2B                  campaigns for healthcare workers.
  * **Growth (Segment Migration):** Launch a "VIP" program utilizing the Power Users to pull the "Casual" majority into higher engagement tiers.
 
* Tableau Dashboard - <a href="https://public.tableau.com/app/profile/tathagata.chakraborty5102/viz/HEATH-TECHANALYSIS/Dashboard" target="_blank">
  <img src="https://upload.wikimedia.org/wikipedia/commons/4/4b/Tableau_Logo.png" alt="My Tableau Profile" width="200"/>
</a>

---

### 2. 🚖 Ride-Hailing Operations: Bottleneck & Revenue Leakage Analysis  

<a href="https://github.com/TATHAGATA23071998/PROJECTS/tree/main/RIDE%20SERVICE%20PROJECT">
<img src="https://img.shields.io/badge/Project_Repository-181717?style=for-the-badge&logo=github&logoColor=white">
</a>

**Tools Used:** SQL Server (SSMS) | Python (Pandas) | Tableau | Streamlit  

 **(a) Core Metrics Tracked:** 
  * Total Booking Value (₹56.53M)
  * Successful Booking Rate (62.09%)
  * Total Ride Volume (103,024)
  * Cancellations by Drivers > Cancellations by Customers

 **(b) The Business Decision (Problem Framing):**  Regional operations were experiencing a massive 38% ride failure rate. The executive team needed to                    definitively answer whether this was a demand-side marketing issue or a supply-side operational bottleneck in order to stop the ₹56.5M revenue leakage.

 **(c) Technical Execution & Analytical Judgment:**
  * Engineered a highly optimized Star Schema in SQL Server to process 100,000+ transaction records, ensuring executive BI dashboards loaded instantly.
  * Used analytical judgment to protect baseline volume metrics: instead of dropping rows with missing wait times (which would artificially shrink the total ride      count), imputed missing values using statistical medians to preserve data integrity.
  * Architected a "Junk Dimension" to handle messy, unstructured cancellation text, drastically reducing the computational load on the central reporting database.

 **(d) Stakeholder Delivery & Outcomes:**
  * Delivered a top-down, interactive Tableau dashboard that proved the bottleneck was 100% supply-side, ruling out customer demand issues.
  * Uncovered widespread driver "gaming" behavior (accepting rides but refusing to move to force customer cancellations).
  * Correlated payment risk, proving that "Cash" payments generate high volume but carry the highest operational cancellation risk.

 **(e) Strategic Recommendations:**
  * Implement an algorithmic 3-minute GPS penalty system to automatically reassign stationary drivers without penalizing the customer.
  * Launch aggressive customer discount campaigns for UPI payments to lock in platform revenue and eliminate the physical friction of cash on the street.
  * Partner with insurance companies to look after the vehicles for reducing the customer cancellation rates.

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
