# 🚗 Vehicle Insurance Cross Sell Analysis (Tableau)

### 📌 Project Overview

The **Vehicle Insurance Cross Sell Analysis Dashboard** is a **Tableau-based data visualization project** designed to help an insurance company identify potential customers for cross-selling vehicle insurance policies.

The dashboard provides a **comprehensive overview of client demographics, insurance coverage, vehicle conditions, and interest in vehicle insurance**, helping business stakeholders design more targeted marketing strategies and improve customer conversion rates.
<img width="1880" height="847" alt="image" src="https://github.com/user-attachments/assets/1df78e99-0d88-4346-adc6-44642cf841e3" />

---

## 🎯 Objective

To analyze client profiles and identify **cross-selling opportunities** by:

* Understanding the relationship between health insurance and vehicle insurance ownership.
* Assessing customer interest levels in purchasing vehicle insurance.
* Identifying demographic patterns such as **age**, **gender**, and **vehicle condition**.
* Enabling the business to **target potential customers** efficiently for insurance marketing campaigns.

---

## 🧾 Dataset Description

The dashboard is built using the dataset **`Vehicel Insurance Data.csv`**, which contains customer-level data including demographic, vehicle, and insurance-related attributes.

| **Column Name**        | **Description**                                                 |
| ---------------------- | --------------------------------------------------------------- |
| `id`                   | Unique client identifier                                        |
| `Gender`               | Gender of the client (Male/Female)                              |
| `Age`                  | Age of the client                                               |
| `Driving_License`      | 1 if the client holds a driving license, 0 otherwise            |
| `Region_Code`          | Encoded region of the client                                    |
| `Previously_Insured`   | 1 if the client had previous vehicle insurance, 0 otherwise     |
| `Vehicle_Age`          | Age of the vehicle (<1 Year, 1-2 Year, >2 Years)                |
| `Vehicle_Damage`       | Indicates whether the vehicle was previously damaged            |
| `Annual_Premium`       | Amount paid annually for health insurance                       |
| `Policy_Sales_Channel` | Distribution channel code for policy acquisition                |
| `Vintage`              | Number of days the client has been associated with the company  |
| `Response`             | 1 if the client is interested in vehicle insurance, 0 otherwise |

---

## ⚙️ Data Preparation

Before visualization, several preprocessing steps were applied in Excel and Tableau:

1. **Data Cleaning**

   * Removed missing or null entries in key columns such as `Age`, `Annual_Premium`, and `Vehicle_Damage`.
   * Standardized categorical variables for consistency (`< 1 Year`, `1-2 Year`, `> 2 Years`).
2. **Feature Creation**

   * Created bins for **Client Age** for grouped visual analysis.
   * Calculated average annual premium by **Vehicle Damage Status**.
3. **Data Aggregation**

   * Summarized total client counts by insurance type, gender, and interest status.

---

## 📊 Dashboard Components

### 1️⃣ **KPI Cards (Donut Charts)**

These visual indicators summarize the key performance metrics for the business:

| **KPI**                                                 | **Description**                                                                   |
| ------------------------------------------------------- | --------------------------------------------------------------------------------- |
| **Total Clients having Health Insurance**               | Clients currently holding health insurance (381.11K)                              |
| **Total Clients not Having Previous Vehicle Insurance** | Clients without prior vehicle insurance (174.6K)                                  |
| **Total Clients Interested in Vehicle Insurance**       | Clients expressing interest in purchasing vehicle insurance (46.7K)               |
| **Average Premium if Car not Damaged**                  | Average annual premium paid by clients whose cars have not been damaged (≈30.56K) |
| **Total Clients Based on Gender**                       | Client segmentation by gender (206K male, 175K female)                            |

Each donut chart visually represents the **percentage of total clients** in each category relative to the overall base population.

---

### 2️⃣ **Client Age-wise Vehicle Count**

* **Visualization Type:** Stacked Column Chart
* **Purpose:** Shows how the number of vehicles varies across client age groups and **vehicle age categories** (`<1 Year`, `1-2 Year`, `>2 Years`).
* **Insight:** Clients aged between **25–45 years** own the majority of vehicles, with most cars being **1–2 years old**.

---

### 3️⃣ **Vehicle Damage Percentage**

* **Visualization Type:** Stacked Bar Chart
* **Purpose:** Displays the percentage of vehicles reported as damaged versus undamaged, categorized by vehicle age.
* **Insight:** Older vehicles (>2 years) show a significantly higher damage rate (**~99%**) compared to newer ones, highlighting potential **higher risk segments**.

---

### 4️⃣ **Interactive Controls**

* **Age Bin Selector:** Slider filter to dynamically adjust client age grouping for deeper insights.
* **Vehicle Age Filter:** Allows the user to isolate data by vehicle age (`<1 Year`, `1–2 Year`, `>2 Years`).
* **Gender Filter:** Enables gender-based segmentation and comparison across KPIs.

---

## 💡 Key Insights

* **64%** of total clients have reported some form of **vehicle damage**, suggesting high claim activity.
* **174K clients** lack previous vehicle insurance — a strong cross-sell opportunity.
* **46.7K clients** are actively interested in purchasing vehicle insurance, representing a **potential conversion funnel**.
* **Males (206K)** slightly outnumber **females (175K)** among the client base, but both groups show comparable interest in insurance.
* Clients aged **25–45 years** represent the **highest cross-sell potential**, with vehicle ownership and interest peaking in this demographic.

---

## 🧠 Business Use Case

By leveraging this dashboard, insurance companies can:

* Identify **high-potential customers** who already own health insurance but lack vehicle insurance.
* Prioritize **marketing efforts** for specific **age groups**, **vehicle conditions**, and **geographic regions**.
* Develop **personalized campaigns** for customers showing high intent (based on `Response = 1`).
* Forecast potential **premium revenue** from vehicle insurance cross-sell opportunities.

---

## 🛠️ Tools & Technologies

| **Tool**                             | **Purpose**                               |
| ------------------------------------ | ----------------------------------------- |
| **Tableau Desktop (Public Edition)** | Dashboard design and visualization        |
| **Microsoft Excel / CSV**            | Data preprocessing and feature creation   |
| **Calculated Fields (Tableau)**      | KPI computation and conditional logic     |
| **Donut Charts, Bar Graphs, Maps**   | Visual storytelling and trend analysis    |
| **Parameters & Filters**             | Interactivity and user-driven exploration |

---

## 🧩 Skills Demonstrated

* Data cleaning and preparation for Tableau
* Dashboard design and layout optimization
* KPI visualization using donut and bar charts
* Data segmentation and parameter control
* Business analysis for cross-sell targeting

---

## 📁 Deliverables

* **Dataset:** `Vehicel Insurance Data.csv`
* **Tableau Workbook:** `Vehicle Insurance Cross Sell Analysis.twbx`
* **Documentation:** `Problem Statement.docx`

---

## 🚀 Insights Summary

This dashboard provides an **end-to-end analytical overview** of client profiles and behaviors that can drive cross-selling strategies. By combining demographic, behavioral, and vehicle-related data, insurance providers can:

* Increase vehicle policy sales.
* Minimize acquisition costs.
* Design data-driven marketing campaigns to boost profitability.

---

## 👨‍💻 Author

**Puneeth Vijay Krishna Samarla**
M.S. in Information Science (Machine Learning), University of Arizona
📧 [puneethvks9@email.com](mailto:puneethvks9@email.com)
🔗 [LinkedIn](https://www.linkedin.com/in/puneeth-samarla)
