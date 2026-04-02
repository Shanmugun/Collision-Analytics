# 🚗 Collision Analytics Dashboard

## 📌 Project Overview
The **Collision Analytics** project provides an end-to-end data pipeline and interactive dashboard to analyze traffic collisions across the United States. It focuses on identifying trends, high-risk regions, and patterns in accident data for 2022 and 2023.

The project leverages ETL processes, data visualization, and cloud publishing to deliver actionable insights through an interactive Tableau dashboard and story.

---

## 📊 Data Source
- Dataset: Fatality Analysis Reporting System (FARS)
- Source: https://geodata.bts.gov/datasets/usdot::fatality-analysis-reporting-system-fars-2022-accidents/about  
- Years Used: **2022 & 2023**

---

## ⚙️ Tech Stack
- **Data Processing (ETL):** Tableau Prep Builder  
- **Visualization & Dashboarding:** Tableau Desktop  
- **Cloud Hosting:** Tableau Cloud  
- **Presentation Layer:** Tableau Stories  

---

## 🔄 Data Pipeline (ETL)
The ETL pipeline was built using **Tableau Prep Builder**:

1. **Data Ingestion**
   - Imported raw accident datasets for 2022 and 2023

2. **Data Transformation**
   - Merged datasets using a **Union operation**
   - Cleaned null values and inconsistencies
   - Standardized fields across both years
   - Created calculated fields for analysis (e.g., collision types, trends)

3. **Output**
   - Clean dataset exported and published to **Tableau Cloud**
   - Scheduled refresh configured via Prep pipeline

---

## ☁️ Data Publishing & Scheduling
- Processed dataset published to **Tableau Cloud**
- Automated refresh scheduling implemented using Tableau Prep pipelines
- Ensures dashboard always reflects updated data

---

## 📈 Dashboard Features

### Key Metrics
- Total Collisions
- Number of Vehicles Involved
- Fatalities Count  
- Year-over-Year Trends

### Visual Insights
- 🗺️ **Collision Hot Zones (Map View)**  
  - State-level accident distribution  

- 📊 **Day-wise Collision Analysis**  
  - Identifies peak accident days (e.g., weekends)

- 📉 **Time Series Trends**  
  - Monthly accident trends across years  

- 🚘 **Collision Type Breakdown**  
  - Front-to-rear, sideswipe, angle collisions, etc.

---

## 📖 Tableau Story
A **Tableau Story** was created to guide users through:
- Key findings
- Trends and anomalies
- Regional insights
- Actionable interpretations

The story uses narrative-driven visuals to make the data easy to understand for stakeholders.

---

## 🖼️ Project Architecture
<img width="767" height="554" alt="Screenshot 2026-04-02 at 4 12 16 PM" src="https://github.com/user-attachments/assets/03d25497-bbbc-47cd-a4c9-efc46555acd2" />

---

## 🚀 Key Insights
- Collisions show **slight decline (~4%) year-over-year**
- **Weekends (especially Saturday)** have the highest accident rates
- Certain states act as **collision hotspots**
- Seasonal trends indicate fluctuations across months

---

## 📂 Repository Contents
- `README.md` – Project documentation  
- `data/` – Sample or reference datasets  
- `images/` – Dashboard screenshots  
- `prep-flow/` – Tableau Prep flow  
- `presentation/` – Tableau Story / PPT

---

## 🔮 Future Improvements
- Integrate real-time accident data feeds  
- Add predictive analytics (ML models)  
- Drill-down analysis at city/county level  
- Enhance geospatial clustering  
