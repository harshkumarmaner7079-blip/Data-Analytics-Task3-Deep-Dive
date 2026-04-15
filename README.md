# Data Analytics Internship - Task 3: Deep-Dive Analysis & Interactive Dashboarding

## **Project Overview**
This is the final phase of the Data Analytics internship at **ApexPlanet Software Pvt. Ltd.** In this task, I transitioned from static data exploration to building a strategic business tool. The project involved defining core business metrics, performing a deep-dive behavioral analysis using Python, and deploying a live, interactive dashboard in **Looker Studio**.

---

## **🚀 [Live Interactive Dashboard Link]**
> **Click here to view the live dashboard:** `https://datastudio.google.com/reporting/b74676c8-d4d6-4574-bee2-7521beef4db6`

---

## **1. Core KPI Definitions**
To evaluate the health of the retail business, I established four "North Star" metrics. These KPIs allow stakeholders to monitor performance at a glance.

| KPI Name | Technical Formula | Business Rationale |
| :--- | :--- | :--- |
| **Total Revenue** | $$\sum(\text{Total Spent})$$ | Measures overall scale and market reach. |
| **Average Order Value (AOV)** | $$\frac{\text{Total Revenue}}{\text{Total Transactions}}$$ | Monitors the spending power per customer visit. |
| **Items Per Transaction (IPT)** | $$\frac{\sum(\text{Quantity})}{\text{Total Transactions}}$$ | Measures "Basket Depth" and cross-selling efficiency. |
| **Discount Utilization Rate** | $$\left( \frac{\text{Discounted Sales}}{\text{Total Sales}} \right) \times 100$$ | Tracks reliance on promotions and brand health. |

### **Baseline Performance Results:**
* **Total Revenue:** $1,637,367.00
* **Average Order Value (AOV):** $130.21
* **Items Per Transaction (IPT):** 5.56
* **Discount Utilization Rate:** 33.55%

---

## **2. Deep-Dive Analysis (Customer Segmentation)**
Using Python (Pandas), I performed a segmentation analysis to determine the effectiveness of the current discount strategy.

### **Segment Comparison: Discount Hunters vs. Full Price Buyers**
| Metric | Discount Hunter (33.55% of users) | Full Price Buyer (66.45% of users) |
| :--- | :--- | :--- |
| **Average Spend (AOV)** | **$130.97** | **$129.82** |
| **Items Per Order** | 5.55 | 5.56 |
| **Total Revenue Share** | 33.75% | 66.25% |

### **Key Executive Insights:**
* **Minimal Spend Lift:** Discounts only provide a **0.8% ($1.15)** increase in Average Order Value. 
* **Volume Neutrality:** Both segments buy nearly identical quantities. This indicates that discounts are not driving customers to buy *more* items; they are simply buying their planned items at a lower price.
* **Strategic Recommendation:** The business should consider shifting from general discounts to "Bundle Offers" (e.g., *Buy 5, Get 1 Free*) to increase the **Items Per Order** metric.

---

## **3. Interactive Dashboarding**
The final tool was built in **Looker Studio** to provide real-time data accessibility for managers.

### **Dashboard Features:**
* **Real-Time Filtering:** Users can filter the entire report by **Category**, **Customer Segment**, or **Time Period**.
* **Revenue Trend Analysis:** A visualized timeline of sales, highlighting the peak revenue month (**January**).
* **Category Drill-Down:** A breakdown of which departments (like Butchers and Furniture) drive the highest margins.
* **Segment Performance View:** A stacked comparison showing how many sales in each category depend on discounts.

