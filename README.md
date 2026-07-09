# 📊 HR Analytics Dashboard | Power BI

## 📌 Project Overview

The **HR Analytics Dashboard** is an interactive Power BI project designed to analyze employee data and provide meaningful insights into workforce trends, employee attrition, job satisfaction, demographics, and organizational performance.

The dashboard helps HR teams and management understand employee behavior, identify key factors affecting attrition, and support data-driven workforce decisions.

---

## 🎯 Project Objectives

* Analyze overall employee workforce data
* Track employee attrition and retention trends
* Identify departments and job roles with high attrition
* Analyze employee demographics
* Understand the relationship between age, salary, job role, and attrition
* Monitor job satisfaction and employee performance
* Build an interactive dashboard using slicers and filters
* Support HR decision-making with clear visual insights

---

## 🛠️ Tools & Technologies Used

* **Power BI Desktop** – Dashboard development and visualization
* **Power Query** – Data cleaning and transformation
* **DAX** – KPI calculations and analytical measures
* **Microsoft Excel / CSV** – Source data handling
* **Data Modeling** – Creating relationships and structured analysis

---

## 📊 Key Performance Indicators

The dashboard focuses on important HR metrics such as:

* 👥 Total Employees
* 🚪 Total Attrition
* 📉 Attrition Rate
* 💼 Active Employees
* 🎂 Average Employee Age
* 💰 Average Monthly Income
* ⭐ Job Satisfaction
* 📅 Average Years at Company

---

## 📈 Dashboard Analysis

### 1. Employee Overview

Provides a high-level summary of the organization's workforce, including total employees, active employees, attrition count, and other major HR KPIs.

### 2. Attrition Analysis

Analyzes employee attrition across different categories to identify major workforce retention challenges.

Key areas include:

* Attrition by Department
* Attrition by Job Role
* Attrition by Age Group
* Attrition by Gender
* Attrition by Education Field
* Attrition by Salary Range
* Attrition by Years at Company

### 3. Department Analysis

Compares workforce distribution and attrition patterns across different departments to identify areas requiring HR attention.

### 4. Employee Demographics

Analyzes employee characteristics based on:

* Age
* Gender
* Marital Status
* Education
* Education Field

### 5. Job Role Analysis

Examines employee distribution and attrition across different job roles to identify positions with higher employee turnover.

### 6. Salary and Income Analysis

Evaluates employee income patterns and explores how salary levels may influence attrition and employee retention.

### 7. Job Satisfaction Analysis

Analyzes employee satisfaction levels to understand their relationship with workforce stability and attrition.

---

## 🔄 Interactive Dashboard Features

The Power BI dashboard includes interactive features such as:

* Dynamic slicers
* Cross-filtering between visuals
* Department-wise filtering
* Job role filtering
* Gender filtering
* Education field filtering
* Attrition-based filtering
* Interactive charts and KPI cards

When a user selects a value from a slicer, all connected dashboard visuals update automatically.

---

## 🧮 Sample DAX Measures

### Total Employees

```DAX
Total Employees = COUNTROWS('HR Analytics')
```

### Total Attrition

```DAX
Total Attrition =
CALCULATE(
    COUNTROWS('HR Analytics'),
    'HR Analytics'[Attrition] = "Yes"
)
```

### Attrition Rate

```DAX
Attrition Rate =
DIVIDE(
    [Total Attrition],
    [Total Employees],
    0
) * 100
```

### Active Employees

```DAX
Active Employees =
[Total Employees] - [Total Attrition]
```

---

## 💡 Key Business Insights

* Employee attrition can be analyzed across departments, job roles, and demographic groups.
* Specific age groups may show higher employee turnover patterns.
* Job satisfaction can influence employee retention.
* Salary and monthly income may be important factors affecting attrition.
* Employees with fewer years at the company may demonstrate different attrition behavior.
* Department-level analysis helps identify workforce areas requiring immediate attention.
* Interactive filtering enables HR teams to perform detailed employee-level analysis.

---

## 📂 Project Structure

```text
HR-Analytics-Dashboard/
│
├── HR ANALYTICS DASHBOARD 1(1).pbix
├── dashboard.png
├── dataset/
│   └── HR_Analytics_Data.csv
└── README.md
```

---

## 🖼️ Dashboard Preview

Add your dashboard screenshot to the GitHub repository and use:

```markdown
![HR Analytics Dashboard](dashboard.png)
```

Recommended repository structure:

```text
HR-Analytics-Dashboard/
│
├── HR ANALYTICS DASHBOARD 1(1).pbix
├── dashboard.png
└── README.md
```

---

## 🚀 How to Use the Project

1. Download or clone the repository.
2. Open the `.pbix` file using Power BI Desktop.
3. Refresh the dataset if required.
4. Use slicers and filters to explore HR metrics.
5. Interact with charts to analyze workforce and attrition patterns.

---

## 🎯 Business Value

This dashboard helps HR professionals and business leaders to:

* Monitor workforce performance
* Identify high-attrition employee groups
* Improve employee retention strategies
* Understand workforce demographics
* Analyze department-level trends
* Support data-driven HR planning
* Improve organizational decision-making

---

## 🔮 Future Enhancements

* Employee attrition prediction using Machine Learning
* Real-time HR database integration
* Advanced drill-through analysis
* Employee performance forecasting
* Automated Power BI Service refresh
* Row-Level Security for department managers
* Integration with SQL databases
* HR recruitment and retention forecasting
