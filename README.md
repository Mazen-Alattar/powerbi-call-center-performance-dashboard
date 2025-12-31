# 📞 Call Center Performance Dashboard (Power BI)

<img src="https://raw.githubusercontent.com/Mazen-Alattar/powerbi-call-center-performance-dashboard/refs/heads/main/powerbi-call-center-performance/images/dashboard_preview.png" width="900">

## 📌 Project Overview
This project analyzes call center operations using **Power BI** to evaluate call volume, response efficiency, call duration, and operational performance.
The dashboard transforms raw call logs into actionable insights through proper **data cleaning, data modeling, and DAX measures**.

The project is designed as a portfolio project for **Data Analyst Internship** roles and demonstrates practical Power BI skills.

---

## 🗂 Dataset Information
- **Domain:** Call Center Operations
- **Source:** Unspecified / Unknown
- **Data Type:** Call logs and customer interaction data

### Original Columns
- Id  
- Call Timestamp  
- Call-Centres City  
- Channel  
- City  
- Customer Name  
- Reason  
- Response Time  
- Sentiment  
- State  
- Call Duration In Minutes  
- CSAT Score  

---

## 🔄 Data Cleaning & Preparation (Power Query)

### CSAT Score Handling
- The **CSAT Score** column contained **more than 60% missing values**.
- Due to the high percentage of null values and low analytical reliability, this column was **removed from the dataset**.

### Date & Time Issues
- The **Call Timestamp** column had multiple formatting inconsistencies.
- Custom transformation logic was applied in **Power Query** to:
  - Fix date and time format issues
  - Ensure consistent and usable datetime values
- The cleaned timestamp was then used for time-based analysis.

### Final Preparation Steps
- Verified correct data types for all remaining columns
- Cleaned and standardized categorical values
- Prepared the dataset for modeling and DAX calculations

---

## 🧩 Data Modeling

### Date Table
- Created a dedicated **Date Table using DAX**.
- Established a relationship between the Date Table and the main dataset using the cleaned **Call Timestamp** column.
- Enabled detailed time-based analysis (daily trends and filtering).

---

## 🧮 DAX Measures
The following measures were created to support performance analysis:

- **Total Calls**
- **Total Call Duration (Minutes)**
- **Total Call Duration (Hours)**
- **Average Call Duration (Minutes)**
- **Response Time %**

These KPIs allow dynamic evaluation of call center efficiency across time, channels, locations, and reasons.

---

## 📄 Dashboard Pages

### Home Page
- Executive overview with KPI cards:
  - Total Calls
  - Total Call Duration (Minutes & Hours)
  - Response Time %
  - Average Call Duration
- Call trends by day
- Geographic distribution of calls by state
- Call distribution by:
  - Reason
  - Channel
  - Sentiment
  - Call-Centres City
- Interactive slicers for Date, Channel, and City

### Grid Page
- Detailed, row-level view of call data
- Enables inspection of:
  - Individual calls
  - Response time status (Within / Below / Above SLA)
  - Call duration by customer, city, and channel
- Supports operational drill-down analysis

---

## 📈 Key Insights

### Overall Performance
- The call center handled approximately **32.9K total calls** during the selected period.
- Total call duration exceeded **824K minutes** (~13.7K hours), reflecting a high operational workload.
- The **average call duration** is around **25 minutes**, indicating relatively long customer interactions.

### Response Time & Efficiency
- The **Response Time % is 75.26%**, meaning most calls were handled within the response target.
- There is potential to improve SLA compliance and reduce delayed responses.

### Time-Based Trends
- Call volume varies significantly by **day of the week**, highlighting peak and low-demand periods.
- These trends can support better staffing and scheduling decisions.

### Geographic Insights
- Call activity is concentrated in specific states and cities.
- Some call-centre cities (such as Los Angeles and Baltimore) handle a much higher volume of calls than others.

### Channel Analysis
- Calls are distributed across multiple channels:
  - Call-Center
  - Web
  - Chatbot
  - Email
- Traditional call-center interactions remain dominant, while digital channels contribute a meaningful share.

### Sentiment & Reasons
- A large portion of calls fall under **Negative and Neutral sentiment**.
- Billing issues, payments, and service outages represent the most common reasons for customer calls.

### Detailed Analysis
- The Grid page enables deep inspection at the individual call level.
- This supports both high-level monitoring and detailed operational investigation.

---

## 🛠 Tools & Technologies
- **Power BI**
- Power Query (Data Cleaning & Transformation)
- DAX (Measures & Date Table)
- Data Modeling
- Interactive Visualizations

---

## 🎯 Project Goal
This project was developed as part of a data analytics portfolio to demonstrate:
- Strong Power BI data modeling skills
- Effective data cleaning and preparation using Power Query
- Creation of meaningful operational KPIs using DAX
- Clear and interactive dashboard design  

Targeted toward **Data Analyst Internship** opportunities.
