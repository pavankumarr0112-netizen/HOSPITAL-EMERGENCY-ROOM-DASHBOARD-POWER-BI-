# 🏥 Hospital Emergency Room Dashboard (Power BI)

## 📌 Project Overview

A comprehensive **Hospital Emergency Room Analytics Dashboard** built using Power BI to monitor patient flow, waiting time, admission trends, and department referrals. This dashboard helps hospital management improve operational efficiency and patient experience.

---

## 🎯 Problem Statement

Emergency rooms often struggle with:

* Long patient waiting times
* Uneven patient distribution across departments
* Lack of real-time visibility into patient flow

This project solves these issues by providing an **interactive dashboard** that enables data-driven decision-making for hospital administrators.

---

## 📊 Dataset Information

* Source: Hospital ER dataset (CSV file included)
* Total Records: ~9,000+ patients *(based on consolidated dashboard view)*
* Key Columns:

  * Patient ID
  * Gender
  * Age
  * Admission Status
  * Department Referral
  * Patient Wait Time
  * Date & Time

---

## 🛠 Tools & Technologies

* Power BI
* DAX (Data Analysis Expressions)
* Excel / CSV Data Source

---

## 🔄 Project Workflow

1. **Data Cleaning**

   * Handled missing values
   * Standardized categorical data (Gender, Department, Admission Status)

2. **Data Modeling**

   * Created relationships between tables
   * Optimized data structure for performance

3. **DAX Calculations**

   * Calculated KPIs like total patients, average wait time, admission rate
   * Created measures for dynamic filtering

4. **Dashboard Design**

   * Built interactive visuals
   * Added filters (Date, Month, Year)
   * Designed monthly & consolidated views

---

## 📈 Key Insights

* Total Patients handled: **~9K+** *(Consolidated View)*

* Average Wait Time: **~35 minutes**

* Admission Rate: ~50% (Admitted vs Not Admitted nearly equal)

* Peak patient inflow observed during **mid-week (Wed–Fri)** *(based on hourly distribution – page 2)*

* Majority of patients are **not referred to departments (~5.4K cases)**

* Highest referrals observed in:

  * General Practice
  * Orthopedics

* Age group **20–39** contributes the highest number of patients

* Patient satisfaction score remains stable around **4.9 / 5**

👉 These insights help hospitals optimize staffing, reduce wait times, and improve service quality.

---

## 📊 Dashboard Preview

![Monthly Dashboard](Dashboard.pdf)


---

## 🧠 Skills Demonstrated

* Data Cleaning
* Data Modeling
* DAX Calculations
* Data Visualization
* Business Insight Generation
* Dashboard Design

---

## 🚀 How to Use

1. Download the `.pbix` file
2. Open in Power BI Desktop
3. Load/refresh the dataset
4. Interact using filters (Date, Month, Year)

---

## 📌 Key DAX Measures

```DAX
Total Patients = COUNT(Patient[Patient ID])

Average Wait Time = AVERAGE(Patient[Wait Time])

Admission Rate = 
DIVIDE(
    CALCULATE(COUNT(Patient[Patient ID]), Patient[Admission Status] = "Admitted"),
    COUNT(Patient[Patient ID])
)

Patient Satisfaction Score = AVERAGE(Patient[Satisfaction Score])
```

---

## 📌 Project Files

* Power BI Dashboard: `.pbix` file
* Dataset: `Hospital ER_Data.csv`
* Dashboard Preview: `Dashboard.pdf`

---

## ⭐ Conclusion

This project demonstrates how data visualization can transform raw hospital data into actionable insights, improving both operational efficiency and patient care.
