# Bellabeat Case Study – Smart Device Usage Analysis

This repository contains an end-to-end data analysis project completed as part of the Google Data Analytics Capstone. The objective is to analyze Fitbit smart-device usage data and generate actionable insights to support Bellabeat’s marketing strategy.

---

## 1. Business Task
Identify usage trends in Fitbit smart devices and translate those insights into marketing recommendations for Bellabeat’s wellness products.

---

## 2. Dataset Description
Source: Fitbit Fitness Tracker Data (Public Domain, Kaggle)

Files used:
- dailyActivity_merged.csv  
- sleepDay_merged.csv  
- hourlySteps_merged.csv  
- weightLogInfo_merged.csv  

Contains daily, hourly, and sleep-tracking data from 30 Fitbit users.

---

## 3. Tools & Technologies
- R  
- tidyverse  
- lubridate  
- ggplot2  
- GitHub  

---

## 4. Data Cleaning & Preparation
Performed the following steps:
- Loaded all CSV files  
- Cleaned column names  
- Converted date/time fields  
- Removed duplicates  
- Created new features (weekday, total active minutes, hourly trends)  
- Merged activity and sleep data  

All transformations are documented in the main R script.

---

## 5. Analysis & Visualizations
The analysis includes:
- Daily steps distribution  
- Average steps by weekday  
- Sleep vs activity correlation  
- Hourly activity trends  

Visualizations are automatically generated when running the script.

---

## 6. Key Insights
- Average steps ≈ 6,500–7,000/day (below recommended 10,000)  
- Activity peaks in morning and early evening  
- Weekend activity is lower than weekdays  
- Average sleep ≈ 7 hours/day  
- Better sleep corresponds with slightly higher next-day activity  

---

## 7. Marketing Recommendations
- Launch weekend activity challenges  
- Add personalized sleep guidance in the app  
- Send push notifications during peak activity hours  
- Promote achievable active-minutes goals  
- Bundle Bellabeat wearables with membership programs  

---

## 8. Reproduction Instructions

### Step 1 — Clone Repository
```sh
git clone https://github.com/<your-username>/bellabeat-case-study.git
cd bellabeat-case-study

**Step 2 — Install Dependencies**
install.packages(c("tidyverse", "lubridate", "scales"))

**Step 3 — Add Dataset**

Place all Fitbit CSVs inside:

Fitbit_Dataset/

**Step 4 — Run Script**
source("bellabeat_analysis.R")

9. File Structure
bellabeat-case-study/
│
├── README.md
├── bellabeat_analysis.R
├── Fitbit_Dataset/
│   ├── dailyActivity_merged.csv
│   ├── sleepDay_merged.csv
│   ├── hourlySteps_merged.csv
│   └── weightLogInfo_merged.csv
│
├── clean_daily_activity.csv
├── clean_daily_activity_sleep.csv
└── hourly_trends.csv
