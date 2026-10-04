# 📊 PULSE Analytics — Sales & Customer Intelligence Dashboard

<p align="center">
  <b>Interactive Sales, Customer, Product & Market Intelligence System built in Power BI</b>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black" alt="Power BI" />
  <img src="https://img.shields.io/badge/DAX-Analytics-blue?style=for-the-badge" alt="DAX" />
  <img src="https://img.shields.io/badge/Power_Query-Data_Transformation-5B2C83?style=for-the-badge" alt="Power Query" />
  <img src="https://img.shields.io/badge/Excel-Data_Source-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white" alt="Excel" />
  <img src="https://img.shields.io/badge/Data_Model-Star_Schema-success?style=for-the-badge" alt="Star Schema" />
</p>

---

## 📌 Executive Overview

**PULSE Analytics** is an end-to-end **Power BI sales intelligence solution** designed to transform transactional sales data into an interactive decision-support dashboard.

The project combines a centralized **sales fact table** with reusable analytical dimensions for **date, country, customer, product, and category**. The resulting semantic model supports multi-dimensional analysis of sales performance, customer behavior, product contribution, geographic performance, and data-driven recommendations.

Rather than presenting dashboard visuals as isolated charts, PULSE Analytics is structured around practical business questions:

- Where is sales performance strongest or weakest?
- Which countries, products, and categories drive performance?
- How does sales activity change over time?
- Which customers contribute most to the business?
- Which products deserve greater attention?
- Where can management focus commercial actions?

---

## 🎯 Business Problem & Objectives

The dashboard is built to give decision-makers a single analytical view of commercial performance.

### Core Objectives

1. 📈 **Monitor Sales Performance** — Track results across time, geography, products, categories, and customers.
2. 🌍 **Evaluate Country Performance** — Compare markets and identify geographic concentration and opportunities.
3. 👥 **Understand Customer Contribution** — Analyze customer-level performance and contribution.
4. 🛍️ **Analyze Product & Category Performance** — Identify strong and weak areas of the product portfolio.
5. 🔎 **Identify Trends & Patterns** — Understand changes in sales performance over time.
6. 💡 **Support Commercial Recommendations** — Translate analysis into practical business actions.

---

## 📊 Analytical Framework

| Analytical Area | Key Questions |
| :--- | :--- |
| **Sales Performance** | How are sales performing over time and across the portfolio? |
| **Country Analysis** | Which countries contribute most and where are opportunities concentrated? |
| **Customer Analysis** | Which customers drive value and how is contribution distributed? |
| **Product Analysis** | Which products and categories are the strongest contributors? |
| **Recommendations** | What actions can be prioritized from the observed patterns? |

This structure moves users from **executive monitoring → diagnosis → detailed analysis → recommendation**.

---

## 🧭 Dashboard Navigation & Storytelling

### 1. Landing Page

The report's navigation hub and entry point into the analytical modules.

<p align="center">
  <img src="./Dashboard%20Previews/Landing%20Page.png" width="92%" alt="PULSE Analytics — Landing Page" />
</p>

---

### 2. Overview Page

The executive-level view of the business, bringing the main performance indicators and high-level trends together.

<p align="center">
  <img src="./Dashboard%20Previews/Overview%20Page.png" width="92%" alt="PULSE Analytics — Overview Page" />
</p>

---

### 3. Country Analysis

A geographic view of sales performance that supports market-level comparison and opportunity identification.

<p align="center">
  <img src="./Dashboard%20Previews/Country%20Page.png" width="92%" alt="PULSE Analytics — Country Analysis" />
</p>

---

### 4. Customer Analysis

A customer-centric view of sales performance supporting contribution analysis and customer-level investigation.

<p align="center">
  <img src="./Dashboard%20Previews/Customer%20Page.png" width="92%" alt="PULSE Analytics — Customer Analysis" />
</p>

---

### 5. Product Analysis

A product and category view designed to identify portfolio performance patterns and areas requiring commercial attention.

<p align="center">
  <img src="./Dashboard%20Previews/Products%20Page.png" width="92%" alt="PULSE Analytics — Product Analysis" />
</p>

---

### 6. Recommendations

A decision-oriented page that connects the analytical findings with practical commercial actions.

<p align="center">
  <img src="./Dashboard%20Previews/Recommendation%20Page.png" width="92%" alt="PULSE Analytics — Recommendations" />
</p>

---

### 7. Data Model

The semantic-model view showing how the sales fact table connects to the analytical dimensions.

<p align="center">
  <img src="./Dashboard%20Previews/Model%20Page.png" width="92%" alt="PULSE Analytics — Data Model" />
</p>

---

## 🏗️ Data Architecture — Star Schema

The solution follows a **Star Schema** centered on the sales transaction fact table.

### Fact Table

- `fact_sales`

### Dimension Tables

- `dim_date`
- `dim_country`
- `dim_customer`
- `dim_product`
- `dim_category`

The model separates transactional activity from descriptive attributes, making the report easier to filter, aggregate, maintain, and extend.

```
                    ┌─────────────────┐
                    │    dim_date     │
                    └────────┬────────┘
                             │
┌─────────────────┐          │          ┌─────────────────┐
│  dim_country    │          │          │   dim_customer  │
└────────┬────────┘          │          └────────┬────────┘
         │                   │                   │
         └──────────────┐    │    ┌──────────────┘
                        ▼    ▼    ▼
                    ┌───────────────┐
                    │  fact_sales   │
                    └───────┬───────┘
                            │
                   ┌────────┴────────┐
                   ▼                 ▼
          ┌────────────────┐  ┌────────────────┐
          │   dim_product  │  │  dim_category  │
          └────────────────┘  └────────────────┘
```

---

## 📁 Repository Structure

The repository is now organized to separate the Power BI report, dashboard previews, and source data:

```
PULSE-Analytics/
│
├── Assets/
│   └── Landing Page.mp4
│
├── Dashboard Previews/
│   ├── Landing Page.png
│   ├── Overview Page.png
│   ├── Country Page.png
│   ├── Customer Page.png
│   ├── Products Page.png
│   ├── Recommendation Page.png
│   └── Model Page.png
│
├── Data/
│   ├── dim_category.xlsx
│   ├── dim_country.xlsx
│   ├── dim_customer.xlsx
│   ├── dim_date.xlsx
│   ├── dim_product.xlsx
│   └── fact_sales.xlsx
│
├── PULSE Analytics.pbix
├── LICENSE
└── README.md
```

---

## 🛠️ Tools & Technologies

| Technology | Role |
| :--- | :--- |
| **Power BI** | Dashboard development, data modeling, and interactive reporting |
| **DAX** | Measures, KPIs, analytical calculations, and business logic |
| **Power Query** | Data preparation, transformation, and loading |
| **Microsoft Excel** | Source data storage and structured fact/dimension inputs |
| **Star Schema** | Semantic-model architecture for scalable analysis |

---

## 🔄 Analytical Workflow

```
Raw Excel Data
      ↓
Power Query
      ↓
Data Cleaning & Transformation
      ↓
Star Schema Modeling
      ↓
DAX Measures & Business Logic
      ↓
Interactive Power BI Report
      ↓
Sales / Country / Customer / Product Analysis
      ↓
Business Recommendations
```

This keeps the solution focused on the complete analytical lifecycle rather than dashboard design alone.

---

## 💡 Business Value

PULSE Analytics helps decision-makers:

- Compare performance across markets and product portfolios.
- Investigate customer contribution at a detailed level.
- Identify product and category performance patterns.
- Monitor changes in sales over time.
- Move from descriptive reporting toward diagnostic analysis.
- Translate dashboard findings into commercially actionable recommendations.

The report is designed as a **decision-support system**, not simply a collection of visualizations.

---

## 📐 Power BI & DAX Design

The analytical layer is built around reusable Power BI measures and a centralized semantic model.

The model supports analysis across:

- Sales performance
- Time-based trends
- Geographic comparisons
- Customer contribution
- Product and category performance
- Cross-filtering between business dimensions
- Recommendation-oriented analysis

The dimensional model allows analytical logic to be reused consistently across report pages and filter contexts.

---

## 🖥️ Report Experience

The report follows a structured storytelling sequence:

**Landing → Overview → Country → Customer → Products → Recommendations → Model**

This makes the solution suitable for:

- **Executive users** who need a quick overview.
- **Analysts** who need to drill into countries, customers, and products.
- **Commercial teams** who need actionable recommendations.

---

## 📦 Project Files

### Power BI Report

**`PULSE Analytics.pbix`** contains the complete interactive Power BI solution, including the semantic model, transformations, measures, relationships, visuals, and report navigation.

### Source Data

The `Data/` directory contains the source Excel files used to build the model:

- Customer dimension
- Product dimension
- Category dimension
- Country dimension
- Date dimension
- Sales fact table

### Dashboard Previews

The `Dashboard Previews/` directory contains the report screenshots used to document the Power BI experience directly in this README.

---

## 🚀 Key Takeaway

**PULSE Analytics demonstrates an end-to-end Power BI workflow:**

> **Data → Model → Measures → Analysis → Insights → Recommendations**

The project combines dimensional modeling, Power Query transformation, DAX-based analytics, interactive reporting, and business-oriented storytelling into one cohesive sales intelligence solution.

---

## 👤 Author

**Kerelos Nakhla**

Data Analyst & BI Developer

**Core Tools:** Power BI · SQL · Python · Excel · Tableau

---

## 📄 License

This project is licensed under the **MIT License**.

**© Kerelos Nakhla**
