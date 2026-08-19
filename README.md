# 🎬 Netflix User Behavior Analysis Dashboard

## 📌 Project Overview

This project analyzes **Netflix user behavior** using **Python for Exploratory Data Analysis (EDA)** and **Power BI for interactive visualization**.

The project explores customer demographics, subscription behavior, watch time, churn, customer lifetime value, tenure, and the value users receive from their subscriptions.

After performing EDA and feature engineering in Python, the processed dataset was exported and used to build an interactive **Power BI dashboard**. The dashboard also includes a **What-If Price Increase parameter** to simulate the impact of subscription price changes on monthly revenue.

---

## 🎯 Business Objectives

The project aims to answer the following questions:

- What is the overall customer churn rate?
- How does churn vary across different customer tenure groups?
- Which subscription types contribute the most to monthly revenue?
- Which genres are preferred by users?
- How is revenue distributed across countries?
- How much value does an average customer generate?
- Does the cost incurred per watch hour have any relationship with churn?
- How would an increase in subscription prices affect monthly revenue?

---

# 🖥️ Power BI Dashboard



The dashboard provides an interactive overview of Netflix users and includes dynamic filters for:

- Country
- Favorite Genre
- Primary Device

It also includes a **Price Increase % What-If parameter** that dynamically updates the simulated monthly revenue.

---

## 📊 Dashboard KPIs

The dashboard displays the following key performance indicators:

| KPI | Description |
|---|---|
| Total Users | Total number of Netflix users |
| Churn Rate | Percentage of users who churned |
| Average CLV | Average Customer Lifetime Value |
| Simulated Monthly Revenue | Estimated monthly revenue after applying the selected price increase |

---

# 📈 Dashboard Visualizations

## 1. Churn Rate by Tenure Cohort

Users were divided into three tenure groups based on their account age:

- **New**
- **Established**
- **Veteran**

The dashboard compares churn rates across these groups to understand whether customer tenure has an impact on churn.

---

## 2. Simulated Monthly Revenue by Subscription Type

A donut chart shows the contribution of different subscription plans to simulated monthly revenue.

The subscription types include:

- Standard
- Premium
- Basic

The revenue changes dynamically based on the selected **Price Increase %**.

---

## 3. Total Users by Favorite Genre

A treemap visualizes the distribution of users based on their favorite genres.

Genres analyzed include:

- Documentary
- Romance
- Comedy
- Thriller
- Horror
- Drama
- Action
- Sci-Fi

---

## 4. Simulated Monthly Revenue by Country

A geographical map displays the distribution of simulated monthly revenue across different countries.

This visualization helps identify geographic revenue distribution and allows the user to analyze specific regions.

---

## 5. Churn Rate by ROI Bucket

Users were grouped according to the amount they effectively spend for every hour of content watched.

The ROI buckets include:

- `< $0.10/hr` — Great Value
- `$0.10 - $0.25/hr` — Good Value
- `$0.25 - $0.50/hr` — Fair Value
- `$0.50 - $1.00/hr` — Poor Value
- `> $1.00/hr` — Terrible Value

The churn rate was then compared across these groups.

This analysis explores the hypothesis that users who pay more while consuming less content may be more likely to churn.

---

# 🎛️ What-If Analysis: Price Increase Simulation

A **Price Increase % parameter** was created in Power BI to simulate changes in subscription pricing.

Users can adjust the parameter using the slider on the dashboard.

The simulated revenue is calculated based on:

```text
Simulated Monthly Revenue =
Original Monthly Revenue × (1 + Price Increase %)
