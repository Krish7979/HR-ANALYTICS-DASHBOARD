# 👥 HR Analytics Dashboard | Power BI

## 📌 Project Overview
This project focuses on **HR Analytics using Power BI** to analyze employee attrition, workforce demographics, and job satisfaction.  
The dashboard provides clear, numerical insights that help organizations understand **why employees leave** and how retention strategies can be improved using data-driven decisions.

---

## 🎯 Problem Statement
Organizations face challenges in managing employee attrition, workforce productivity, and retention.  
Traditional HR reports lack actionable insights into factors such as **age, salary, job role, tenure, and job satisfaction**.  
The objective of this project is to analyze HR data using Power BI to **identify attrition drivers** and support effective workforce planning.

---

## 💡 Solution
Interactive Power BI dashboards were developed to:
- Track employee attrition rate
- Analyze attrition by age, gender, salary, and job role
- Understand workforce demographics and satisfaction
- Enable HR teams to make data-driven retention decisions

---

## 📊 Dashboard Highlights
- **Total Employees:** 1,470  
- **Attrition Count:** 237  
- **Attrition Rate:** 16.1%  
- **Average Age:** 37 years  
- **Average Salary:** 6.5k  
- **Average Years at Company:** 7 years  

---

## 📈 Key Insights
- Highest attrition observed in the **26–35 age range (116 employees)**
- Maximum attrition among employees with **lower salary levels (163 employees)**
- **Male attrition (140)** is higher than **female attrition (79)**
- Job roles with highest attrition:
  - Laboratory Technician (62)
  - Sales Executive (57)
  - Research Scientist (47)
- Attrition decreases as **years at company increase**

---

## 🗂️ Dataset Description
The dataset contains employee-level HR data for **1,470 employees**, including:
- Age and Gender
- Department and Job Role
- Salary
- Years at Company
- Job Satisfaction
- Attrition Status

---

## 🧹 Data Cleaning
- Removed duplicate employee records
- Handled missing values
- Standardized department and job role names
- Converted categorical fields for Power BI analysis

---

## 🧮 DAX Measures Used
```DAX
Total Employees =
DISTINCTCOUNT(HR_Analytics[EmployeeID])

Attrition Count =
CALCULATE(
    COUNT(HR_Analytics[Attrition]),
    HR_Analytics[Attrition] = "Yes"
)

Attrition Rate =
DIVIDE([Attrition Count], [Total Employees])

Average Age =
AVERAGE(HR_Analytics[Age])

Average Salary =
AVERAGE(HR_Analytics[Salary])

Average Years At Company =
AVERAGE(HR_Analytics[YearsAtCompany])
```

---

## 🛠 Tools & Technologies
- Power BI
- DAX
- Excel / CSV Dataset

---

## ✅ Conclusion
The HR Analytics Dashboard delivers clear numerical insights into employee attrition and workforce behavior.  
It helps organizations identify high-risk attrition segments and take proactive steps to improve employee retention and productivity.

---

## 🔮 Future Scope
- Predictive attrition analysis using Machine Learning
- Integration of performance and appraisal data
- Real-time HR analytics
- Advanced workforce forecasting

---

## 👤 Author
**Krish Modi**  
B.Tech IT Student  
Power BI | Data Analytics | Python | C
