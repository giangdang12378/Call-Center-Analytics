# Call Center Analytics Dashboard

> An end-to-end Power BI project for analyzing call center performance, SLA compliance, workforce efficiency, and call volume trends.

---

# Project Overview

This project analyzes the operational performance of a global Call Center using Power BI.

The objective is to transform raw operational data into an interactive dashboard that enables management to monitor Service Level Agreement (SLA), workforce performance, call trends, and business efficiency.

The dashboard was developed following a real-world business scenario in which the CEO requested an analytical report to support operational improvements and future branch expansion.

---

# Business Objectives

The dashboard answers the following business questions:

- What is the overall SLA Compliance?
- Is service quality improving or declining over time?
- When are the Peak Hours, Peak Days, and Peak Months?
- Which employees perform the best and worst based on SLA and Wait Time?
- Which Call Type contributes the highest call volume?
- Does business growth negatively impact service quality?

---

# Dataset

The dataset contains approximately **130,000+ call records** collected from **2018–2021**.

## Fact Table

- Call Timestamp
- Employee ID
- Call Type
- Call Duration
- Wait Time
- SLA Compliance
- Year
- Month
- Day
- Hour

## Dimension Tables

### Employee Table

- Employee ID
- Employee Name
- Site
- Manager

### Call Type Table

- Call Type ID
- Call Type Description

### Call Charges Table

- Call Charges by Year
- Call Type

---

# Data Cleaning

The following transformations were performed before building the dashboard:

### 1. Removed unnecessary columns

- Source Name
- Call Abandoned

### 2. Created new calculated columns

- SLA Compliance
- Year
- Month Number
- Month Name
- Short Month
- Day
- Day of Week
- Short Weekday
- Hour
- Wait Time Group

- Corrected data types

### 3. Built relationships between Fact and Dimension tables

---

# Dashboard Pages

## 1. Executive Overview

Provides an overview of business performance.

### KPIs

- Total Calls
- SLA Compliance
- Average Wait Time
- Average Call Duration

### Visualizations

- Call Trend by Year
- SLA Trend by Year
- Call Distribution by Month
- Call Distribution by Type
- Average Wait Time by Call Type

---

## 2. Workforce Performance

Evaluates employee performance.

### KPIs

- Total Employees
- SLA Compliance
- Average Wait Time
- Average Call Duration

### Visualizations

- Employee Performance Matrix
- Employee Efficiency Scatter Plot
- Calls by Site
- Wait Time Distribution

The page helps managers identify top-performing and underperforming employees.

---

## 3. Time Analysis

Analyzes operational workload over time.

### KPIs

- Peak Hour
- Peak Day
- Peak Month

### Visualizations

- Total Calls by Hour
- Total Calls by Day of Week
- Total Calls by Month
- Hour × Weekday Heatmap

The dashboard identifies busy and quiet operating periods for workforce planning.

---

# 📈 Key Insights

## Overall Service Level

- Overall SLA Compliance reached **88.22%**.
- SLA remained relatively stable throughout the analysis period.
- Service quality was maintained despite changes in call volume.

## Workforce Performance

- The average wait time is **27.28 seconds**, which is below the company's SLA threshold of **35 seconds**.
- Most employees achieved SLA above **88%**.
- A small group of employees experienced higher wait times and should receive additional coaching.

## Call Volume Trends

The analysis reveals clear workload patterns.

Peak operating periods:

- Peak Hour: **12:00 PM**
- Peak Day: **Friday**
- Peak Month: **January**

These periods require additional staffing to maintain service quality.

## Call Type Analysis

- Tech Support generated the highest call volume.
- Billing and Sales accounted for smaller proportions.
- Different call types showed varying average waiting times, suggesting different workload complexity.

---

# Business Recommendations

## 1. Improve Workforce Planning

Increase staffing during:

- Friday
- Peak business hours around 12 PM
- January

to reduce waiting time and improve customer experience.

## 2. Employee Coaching

Provide additional coaching for employees with:

- High Wait Time
- Low SLA Compliance

Encourage best-practice sharing from top-performing representatives.

## 3. Optimize Call Routing

Since Tech Support handles the largest proportion of calls:

- Allocate more experienced agents
- Improve call routing
- Expand self-service knowledge bases

to reduce queue length.

## 4. Real-time SLA Monitoring

Implement real-time dashboards and alerts whenever:

- SLA drops below target
- Wait Time exceeds 35 seconds

allowing supervisors to react immediately.

## 5. Capacity Forecasting

Historical trends should be used for:

- Workforce scheduling
- Demand forecasting
- Resource allocation
- Expansion planning

---

# Tools & Technologies

- Power BI
- Power Query
- DAX
- Data Modeling
- Star Schema
- Power BI Service (Ready for Deployment)

---

# Skills

## Data Preparation

- Data Cleaning
- Data Transformation
- Data Modeling

## Power BI

- KPI Cards
- Matrix
- Scatter Plot
- Heatmap
- Bar Chart
- Line Chart
- Donut Chart
- Slicers
- Page Navigation
- Conditional Formatting

## DAX

- Measures
- Time Intelligence
- Aggregations
- Business KPIs

## Business Analytics

- SLA Analysis
- Workforce Planning
- Performance Monitoring
- Trend Analysis
- Executive Reporting

---

# Repository Structure

```text
Call-Center-Analytics/
│
├── Dashboard/
│   └── Call Center Analytics.pbix
│
├── Dataset/
│   ├── CALL_CENTER_ALLYEARS.xlsx
│   ├── Call+Center+Data+2018.xlsx
│   ├── Call+Center+Data+2019.xlsx
│   ├── Call+Center+Data+2020.xlsx
│   ├── Call+Center+Data+2021.xlsx
│   ├── Lookup+Tables.xlsx
│   └── Call Charges.xlsx
│
├── Images/
│   ├── Executive Overview.png
│   ├── Workforce Performance.png
│   └── Time Analysis.png
│
└── README.md
```

---

# 👨‍💻 Author

**Đặng Hồ Giang**

Business Information Technology Student

University of Economics Ho Chi Minh City (UEH)

Power BI | SQL | Python | Data Analytics
