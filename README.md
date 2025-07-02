# 🧠 AWS QuickSight Dashboard – Employee Insights

This project demonstrates an end-to-end data visualization solution using **AWS Glue DataBrew** and **Amazon QuickSight**. It starts with cleaning and transforming raw employee data and ends with an insightful, interactive dashboard for HR analytics.

---

## 📌 Project Overview

- **Data Source**: 1000 employee records
- **Data Cleaning Tool**: AWS Glue DataBrew
- **Dashboard Tool**: Amazon QuickSight
- **Storage**: Amazon S3
- **Objective**: Create a clean, filterable HR dashboard showing salary trends, departmental distribution, gender split, and more.

---

## 📊 Dashboard Preview

![Dashboard Screenshot](./assets/Screenshot_2025-06-25_181219.png)

---

## 🧼 Data Cleaning with AWS Glue DataBrew

1. Uploaded the raw dataset to Amazon S3.
2. Created a **DataBrew project** to explore and clean the data.
3. Performed cleaning steps:
   - Removed nulls and duplicate records.
   - Standardized column formats (e.g., dates, gender labels).
   - Derived new columns (if needed).
4. Saved all steps in a **DataBrew Recipe**.
5. Created and ran a **DataBrew Job** to apply the recipe and export the cleaned data back to S3.

➡️ Detailed cleaning steps are available in: [`datacleaning/glue_databrew_steps.md`](./datacleaning/glue_databrew_steps.md)

---

## 📈 Amazon QuickSight Dashboard

Used Amazon QuickSight to build a professional dashboard with the following visuals:

- **KPI Widget**: Total number of employees (1000)
- **Bar Charts**:
  - Total salary by Employee ID
  - Employees by Department
  - Hiring trend over time
- **Donut Chart**: Gender split
- **Pie Chart**: Count of records by city
- **Scrollable Chart**: Average salary by Employee ID

Also included filters for:
- **Department**
- **City**
- **Gender**

➡️ Visual explanation is provided in: [`quicksight/visuals_description.md`](./quicksight/visuals_description.md)

---

## 🗂 Project Structure

