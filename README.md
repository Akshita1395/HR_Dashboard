# 📊 HR Analytics 360 – Attrition, Finance & Wellness Dashboard

## 🔍 Project Overview

**HR Analytics 360** is an end-to-end **Power BI Business Intelligence dashboard** designed to analyze **employee attrition, compensation structure, and wellness indicators**.
The project converts raw HR data into **actionable insights** using advanced **EDA, DAX calculations, and modern UI/UX design**.

This dashboard helps HR teams and leadership:

* Identify **high-risk attrition segments**
* Detect **salary gaps among high performers**
* Monitor **employee wellness and burnout indicators**

---

## 🎯 Business Objectives

* Reduce employee attrition through **data-driven insights**
* Understand **financial drivers of compensation**
* Track **work-life balance and job satisfaction**
* Support **strategic HR decision-making**

---

## 🧰 Tools & Technologies Used

* **Power BI Desktop**
* **Power Query (ETL & Data Cleaning)**
* **DAX (Data Analysis Expressions)**
* **Microsoft Excel (Source Data)**
* **GitHub (Version Control & Portfolio Hosting)**

---

## 📁 Dataset Information

* **Dataset Name:** IBM HR Analytics – Employee Attrition & Performance
* **Source:** Kaggle (Open Source)
* **Records:** 1,470 Employees
* **Features:** 35 Columns

### Key Data Attributes

* **Demographics:** Age, Gender, Education, Marital Status
* **Job Details:** Job Role, Department, Job Level, Years at Company
* **Financials:** Monthly Income, Salary Hike, Daily Rate
* **Wellness:** Job Satisfaction, Work-Life Balance, Environment Satisfaction
* **Target Variable:** Attrition (Yes / No)

---

## 🔄 Data Preparation & EDA

The raw dataset underwent extensive preprocessing in **Power Query**:

* Removal of **zero-variance columns**

  * `EmployeeCount`
  * `Over18`
  * `StandardHours`
* Conversion of coded fields into **business-friendly labels**

  * Education (1–5 → Below College to Doctor)
  * Distance From Home (1–5 → Very Close to Very Far)
* Data quality validation (null & error checks)
* Star schema modeling for optimized performance

---

## 📐 Key DAX Measures

```DAX
Attrition Rate (%) =
DIVIDE(
    CALCULATE(COUNT(HR_Data[EmployeeNumber]), HR_Data[Attrition] = "Yes"),
    COUNT(HR_Data[EmployeeNumber])
)
```

```DAX
Wellness Score =
AVERAGE(HR_Data[WorkLifeBalance])
```

---

## 📊 Dashboard Structure

### 1️⃣ Attrition Command Center

**Purpose:** Identify turnover risks
**Insights:**

* Sales has the highest proportional attrition
* Laboratory Technicians show maximum churn
* Attrition spikes sharply at **1 year tenure**

---

### 2️⃣ Income & Performance Analysis

**Purpose:** Analyze compensation fairness
**Insights:**

* Job Level is the strongest driver of income
* High performers are not always highly paid
* Identifies **“High Performer – Low Pay” risk group**

---

### 3️⃣ Employee Wellness Monitor

**Purpose:** Track burnout & satisfaction
**Insights:**

* Average Work-Life Balance score: **2.76 / 4**
* Sales Executives show lowest environment satisfaction
* Wellness indicators act as **leading predictors of attrition**

---

## 🎨 UI / UX Design

* **Dark Mode Interface** for reduced eye strain
* Neon color palette:

  * Cyan → Attrition
  * Gold → Finance
  * Violet → Wellness
* Interactive slicers & bookmarks
* Executive-friendly layout

---

## 🚀 Deployment

* **Power BI (.pbix)** file included
* GitHub used for:

  * Version control
  * Portfolio showcase
  * Open-source collaboration

---

## 📌 Key Business Recommendations

* Introduce **overtime caps** for technical roles
* Correct **salary gaps for high performers**
* Monitor wellness scores below **2.5** as attrition warning signals

---

## 🔮 Future Enhancements

* Logistic Regression for **attrition prediction**
* Row-Level Security (RLS) for managers
* Automated Power BI Service alerts
* Python integration inside Power BI

---

## 📎 Repository Contents

```
📂 HR-Analytics-360
 ├── HR_Analytics_360.pbix
 ├── Dataset/
 │   └── HR_Employee_Attrition.csv
 ├── Screenshots/
 │   ├── Attrition_Dashboard.png
 │   ├── Finance_Dashboard.png
 │   └── Wellness_Dashboard.png
 └── README.md
```

---

## 👤 Author

Akshita
Data Analyst | Power BI Developer

🔗 LinkedIn: https://www.linkedin.com/posts/akshita9_hr-analytics-portfolio-activity-7404119774634713088-Wops?utm_source=social_share_send&utm_medium=member_desktop_web&rcm=ACoAAFbSz08BIzQ687GbfQsrRu3z_aIkO-KMK88 

---

## ⭐ If You Found This Useful

Please ⭐ star this repository — it helps others discover the project!

