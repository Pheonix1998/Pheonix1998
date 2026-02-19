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

## 1. 🎵 Music Sales Intelligence – Revenue Optimization Project  
<a href="https://github.com/Pheonix1998/PROJECTS/tree/main/MUSIC_PROJECT">
<img src="https://img.shields.io/badge/Project_Repository-181717?style=for-the-badge&logo=github&logoColor=white">
</a>

**Tools:** SQL (SQL Server) | Python | Streamlit  

---

### 📌 Why This Project?

This project simulates how a digital music company would build a reliable reporting system from raw transactional data.

Instead of just creating charts, the focus was on:
- Making revenue numbers accurate  
- Building a clean reporting table  
- Extracting insights that support real business decisions  

---

### 🎯 Business Problem

The data was stored across 11 related tables (customers, invoices, tracks, artists, genres, playlists, etc.).

The main challenges were:

- Revenue was getting duplicated due to incorrect joins  
- Date formats were inconsistent  
- Some customer data had corrupted characters  
- Price columns were not properly formatted  

Because of this, revenue reports were unreliable and could not be trusted for decision-making.

The business needed:
- A single accurate revenue source  
- Clear visibility into top customers and products  
- Reliable monthly and yearly trends  
- Insights into what products are often bought together  

---

### 🛠 My Approach

#### 1️⃣ Cleaned and Validated the Data
- Fixed corrupted characters  
- Standardized date formats  
- Converted price columns safely to numeric values  
- Handled missing values properly  

This ensured the data was ready for accurate analysis.

---

#### 2️⃣ Built a Reliable Reporting Table

Created a new table (`MUSIC_FACT`) with:
- One row per invoice line  
- No duplicate revenue  
- Proper date and numeric formats  

Revenue validation check used:

`Invoice Total = Unit Price × Quantity`

This step ensured financial accuracy before performing any analysis.

---

#### 3️⃣ Performed Business-Focused Analysis

**Customer Insights**
- Top 10 customers by total spend  
- Customer Lifetime Value (CLV)  
- Repeat vs one-time buyers  
- Purchase frequency analysis  

**Revenue Insights**
- Monthly and yearly revenue trends  
- Peak sales periods  
- Average invoice value  
- Revenue by country and city  

**Product Insights**
- Top tracks and artists  
- Revenue by genre  
- Media type performance  
- Tracks never purchased  

**Cross-Sell Insights**
- Frequently purchased track combinations  
- Bundle opportunities  

---

### 📊 Streamlit Dashboard - [![Streamlit](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://python-app-8jiapof4fdah2ntbfb4rw7.streamlit.app/)

Built a Streamlit dashboard to make insights easy to explore.

**Dashboard Highlights:**
- Total Revenue  
- Total Invoices  
- Average Invoice Value  
- Total Customers  
- Revenue trends over time  
- Top artists, genres, and tracks  
- Geographic revenue view  
- Customer segmentation  
- Product bundle insights  

Users can filter by year, country, and genre.

---

### 📈 Key Outcomes

- Built a clean and accurate reporting table  
- Removed revenue duplication errors  
- Identified major revenue drivers  
- Measured customer lifetime value  
- Detected peak sales periods  
- Found product bundling opportunities  

---

### 💡 Business Recommendations

- Use the clean reporting table for all future dashboards  
- Monitor revenue using validated calculations  
- Launch bundle promotions for frequently bought-together tracks  
- Focus marketing efforts on high-value customers  
- Invest more in high-revenue genres  

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

## 📊 Dashboard Solution

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
