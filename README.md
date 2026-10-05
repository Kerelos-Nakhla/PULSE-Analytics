# 📊 PULSE Analytics — E-Commerce Sales & Customer Intelligence Dashboard

<p align="center">
  <b>Enterprise E-Commerce Sales Intelligence, Customer RFM Segmentation, Basket Composition & What-If Predictive Simulation in Power BI</b>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black" alt="Power BI" />
  <img src="https://img.shields.io/badge/DAX-Time_Intelligence_&_What--If-blue?style=for-the-badge" alt="DAX" />
  <img src="https://img.shields.io/badge/Data_Modeling-Snowflake_Schema-success?style=for-the-badge" alt="Data Modeling" />
  <img src="https://img.shields.io/badge/Analytics-RFM_Customer_Tiers-orange?style=for-the-badge" alt="RFM Tiers" />
  <img src="https://img.shields.io/badge/Simulation-Parameter_Modeling-brightgreen?style=for-the-badge" alt="Simulation" />
</p>

---

## 📌 Executive Overview

The **PULSE Analytics E-Commerce Sales & Customer Intelligence Dashboard** is an enterprise-grade commercial decision-support platform engineered in **Microsoft Power BI**. Designed for digital retail executives, commercial strategists, and marketing directors, it translates granular transactional line items, global multi-currency checkout events, customer behavioral profiles, and catalog performance into high-impact operational intelligence.

The platform monitors **15,670 orders** encompassing **62,810 order items** placed by **1,000 unique customers** across **10 international markets**, governing **$3,293,892.40 (~$3.29M) in gross merchandise value (GMV)**. It bridges the gap between historical retrospective reporting and proactive predictive planning through dynamic What-If parameter simulation.

```
+----------------------------------------------------------------------------------------------------+
|                                    EXECUTIVE PORTFOLIO AT A GLANCE                                 |
+--------------------------+--------------------------+-----------------------+----------------------+
|    $3,293,892.40 Gross   |       15,670 Orders      |    1,000 Customers    |   $210.20 Mean AOV   |
|   62,810 Items Shipped   |   4.01 Items / Basket    |  10 Global Territories|   3.44% Conversion   |
+--------------------------+--------------------------+-----------------------+----------------------+
```

---

## 📊 Commercial Financial Summary & Core KPIs

The enterprise scorecard synthesizes transactional velocity, monetization ratios, and operational volume:

| Key Performance Indicator | Portfolio Value | Benchmark / Formula | Strategic Commercial Impact |
| :--- | :---: | :---: | :--- |
| **Gross Revenue (GMV)** | **$3,293,892.40** | `SUM(fact_order_items[item_price])` | Baseline gross commercial sales across all processed customer checkouts |
| **Total Order Volume** | **15,670 Orders** | `DISTINCTCOUNT(fact_orders[order_id])` | Validated completed digital storefront transactions |
| **Total Units Shipped** | **62,810 Items** | `SUM(fact_order_items[quantity])` | Total physical merchandise units fulfilled through logistics centers |
| **Active Customer Base** | **1,000 Accounts** | `DISTINCTCOUNT(dim_customers[customer_id])` | Global verified consumer accounts generating recurring transactions |
| **Average Order Value (AOV)** | **$210.20** | `[Total Revenue] / [Total Orders]` | Mean financial basket realization per completed storefront purchase |
| **Average Order Items (AOI)** | **4.01 Items** | `[Total Quantity] / [Total Orders]` | Average merchandise depth per order delivery |
| **Storefront Conversion Rate** | **3.44%** | `[Total Orders] / [Total Sessions]` | End-to-end checkout funnel efficiency from session arrival to completed buy |
| **MoM Order Growth** | **+4.12%** | `DIVIDE([Total Orders] - [SPLM Orders], [SPLM Orders])` | Period-over-period order acceleration benchmark |
| **MoM Revenue Growth** | **+3.85%** | `DIVIDE([Total Revenue] - [SPLM Revenue], [SPLM Revenue])` | Top-line sales trajectory tracked against same period last month |
| **Active Product Catalog** | **50 SKUs** | `DISTINCTCOUNT(dim_products[product_id])` | 5 core categories with tracked inventory velocity |
| **Geographic Markets** | **10 Countries** | `DISTINCTCOUNT(dim_country[country_id])` | International shipping coverage across North America, Europe & APAC |

---

## 👥 Customer Loyalty & RFM Tier Segmentation

The customer portfolio is categorized across automated behavioral value tiers to detect retention risk and unlock cross-sell potential:

| Loyalty Tier | Customer Share | Revenue Contribution | Mean Spend / Customer | Retention & Engagement Strategy |
| :--- | :---: | :---: | :---: | :--- |
| **Platinum (VIP)** | **14.2%** | **$1,185,420 (36.0%)** | **$8,348.00** | Dedicated loyalty concierge, early access drops, zero-fee expedited shipping |
| **Gold (High Value)** | **28.6%** | **$1,054,045 (32.0%)** | **$3,685.50** | Category cross-sell incentives, personalized bundle discounts, quarterly milestones |
| **Silver (Mid Tier)** | **35.4%** | **$757,595 (23.0%)** | **$2,140.10** | Re-engagement automation, basket-building free-shipping threshold prompts |
| **Bronze (Occasional)** | **21.8%** | **$296,832 (9.0%)** | **$1,361.60** | Win-back promotional campaigns, onboarding drip sequences, low-friction entry SKUs |

---

## 🛍️ Product Assortment & Commercial Yield Performance

Catalog distribution reveals revenue concentration across primary merchandise categories:

| Product Category | Revenue Share | Units Sold | Mean Category AOV | Margin Contribution | Key Strategic Dynamic |
| :--- | :---: | :---: | :---: | :---: | :--- |
| **Electronics & Hardware** | **38.4% ($1.26M)** | 14,210 | $285.40 | High | Top GMV generator; drives highest basket values but sensitive to price promos |
| **Fashion & Apparel** | **24.1% ($794K)** | 21,450 | $164.20 | Medium | Highest order velocity and unit throughput; highest repeat replenishment rate |
| **Home & Living** | **18.7% ($616K)** | 11,890 | $215.10 | High | Steady seasonal cadence; strong attachment to bundle promotions |
| **Beauty & Personal Care** | **11.2% ($369K)** | 9,840 | $132.80 | High | Strongest recurring subscription potential; prime candidate for auto-ship programs |
| **Sports & Outdoors** | **7.6% ($250K)** | 5,420 | $188.50 | Medium | High summer/holiday seasonality; strong regional variance in cold vs. warm climates |

---

## 🌍 Geographic Penetration & Global Footprint

Cross-border sales analysis tracks market maturity and expansion runway across 10 regions:

- **United States & Canada:** Anchor market generating **52.3% of cumulative sales**, characterized by high AOV ($234.50) and mature multi-line basket depth.
- **European Region (UK, Germany, France, Netherlands):** Represents **31.8% of GMV**, with Germany and the UK exhibiting the fastest MoM transaction growth (+6.2%).
- **Asia-Pacific & Emerging Markets (Australia, Japan, Singapore, Brazil):** Generates **15.9% of portfolio revenue**, exhibiting high conversion potential (4.1% in Singapore) and prime expansion runway.

---

## 💡 In-Depth Financial Analysis & Key Insights

1. **80/20 Revenue Concentration in Top Tiers:** The combined Platinum and Gold cohorts comprise only **42.8% of the customer base** yet drive **68.0% of total gross sales ($2.24M)**. Safeguarding this segment against attrition is the primary lever for revenue stability.
2. **Basket Density Directly Correlates to Margin Health:** Orders with **4+ line items** generate an average AOV of **$312.40** compared to **$98.50** for single-item checkouts. Implementing threshold-based incentives ("Add $35 for Free Priority Delivery") captures immediate incremental margin.
3. **MoM Rebound Across Core Categories:** Month-over-month order expansion of **+4.12%** outpaced revenue growth (+3.85%), indicating sustained customer acquisition velocity with slight price-mix softening toward entry-level catalog items.
4. **Predictive What-If Sensitivity:** Scenario modeling demonstrates that a **+5.0% lift in storefront conversion** combined with a **+$15 AOV expansion** delivers an estimated **+$246,800.00 in quarterly incremental revenue**.

---

## 📐 Key DAX Measures & Formula Reference

### 1. Volume & Revenue Fundamentals

```dax
Total Revenue = 
SUM(fact_order_items[item_price])
```

```dax
Total Orders = 
DISTINCTCOUNT(fact_orders[order_id])
```

```dax
Total Quantity = 
SUM(fact_order_items[quantity])
```

```dax
Total Items = 
COUNTROWS(fact_order_items)
```

---

### 2. Basket Composition & Efficiency Ratios

```dax
Average Order Value = 
DIVIDE([Total Revenue], [Total Orders], 0)
```

```dax
Average Order Quantity = 
DIVIDE([Total Quantity], [Total Orders], 0)
```

```dax
Average Order Items = 
DIVIDE([Total Items], [Total Orders], 0)
```

---

### 3. Time Intelligence & MoM Dynamics

```dax
SPLM Orders = 
CALCULATE(
    [Total Orders],
    DATEADD(dim_date[Date], -1, MONTH)
)
```

```dax
SPLM Revenue = 
CALCULATE(
    [Total Revenue],
    DATEADD(dim_date[Date], -1, MONTH)
)
```

```dax
Order MoM Growth % = 
DIVIDE([Total Orders] - [SPLM Orders], [SPLM Orders], 0)
```

```dax
Revenue MoM Growth % = 
DIVIDE([Total Revenue] - [SPLM Revenue], [SPLM Revenue], 0)
```

---

### 4. Conversion & Customer Engagement

```dax
Storefront Conversion Rate = 
DIVIDE([Total Orders], [Total Sessions], 0)
```

```dax
Revenue per Customer = 
DIVIDE([Total Revenue], DISTINCTCOUNT(dim_customers[customer_id]), 0)
```

```dax
Regional Share of Wallet % = 
DIVIDE(
    [Total Revenue],
    CALCULATE([Total Revenue], ALL(dim_country)),
    0
)
```

---

### 5. What-If Predictive Simulation Modeling

```dax
Projected Revenue = 
VAR TargetAOV = [Average Order Value] * (1 + 'WhatIf_AOV'[AOV_Value])
VAR TargetOrders = [Total Orders] * (1 + 'WhatIf_Conversion'[Conversion_Value])
RETURN
TargetAOV * TargetOrders
```

```dax
Projected Incremental Gain = 
[Projected Revenue] - [Total Revenue]
```

---

## 🎯 Business Problem & Objectives

- **Fragmented Commercial Visibility:** Prior to this implementation, executive leadership lacked unified visibility across transactional sales, geographic velocity, and product profitability.
- **Customer Segmentation Blind Spots:** Marketing teams were deploying uniform, non-differentiated campaigns without automated behavioral RFM clustering, leading to wasted ad spend.
- **Reactive Financial Planning:** Scenario projections were managed in static offline spreadsheets, preventing live sensitivity analysis of pricing and conversion adjustments.
- **The Solution:** A centralized, multi-page Power BI intelligence system combining automated dimensional modeling, dynamic time intelligence, and real-time parameter simulation.

---

## 🖼️ Dashboard Visual Tour & Storytelling

### 1. Executive Landing & Navigation Hub
The primary portal directing users seamlessly across operational, regional, customer, and predictive views with persistent breadcrumb navigation.
![Executive Landing Page](Dashboard%20Previews/Landing%20Page.png)

---

### 2. Commercial Overview & Executive KPIs
Comprehensive executive scorecard featuring high-level KPIs, revenue trends, period-over-period variances, and category distributions.
![Commercial Overview](Dashboard%20Previews/Overview%20Page.png)

---

### 3. Customer Intelligence & Loyalty Tiers
In-depth cohort analysis classifying customers by RFM scores, lifetime transaction value, repeat order frequency, and retention hazard.
![Customer Intelligence](Dashboard%20Previews/Customer%20Page.png)

---

### 4. Regional & Geographic Penetration
Interactive geospatial intelligence showing cross-border revenue share, local order volume, and international fulfillment velocity across 10 countries.
![Regional Performance](Dashboard%20Previews/Country%20Page.png)

---

### 5. Product Assortment & Yield Performance
SKU-level performance matrix identifying category demand leaders, margin contributors, volume movers, and slow-moving inventory alerts.
![Product Performance](Dashboard%20Previews/Products%20Page.png)

---

### 6. Strategic Recommendations & What-If Simulation
Predictive parameter sliders enabling leadership to test conversion rate uplifts and AOV expansions to project forward-looking revenue impact.
![Recommendation & Simulation](Dashboard%20Previews/Recommendation%20Page.png)

---

### 7. Enterprise Snowflake Schema Data Model
The underlying dimensional schema illustrating fact-to-dimension relationships, cardinality, and cross-filtering design.
![Data Model Schema](Dashboard%20Previews/Model%20Page.png)

---

## 🏗️ Data Architecture & Star Schema

The reporting engine is built on a clean **Snowflake Schema** ensuring 1-to-many unidirectional filtering and optimal VertiPaq compression.

### 📐 Schema Architecture Diagram

```
                             +-------------------+
                             |     dim_date      |
                             +-------------------+
                                       | 1
                                       | 
                                       | *
+------------------+ 1       * +-------------------+ *       1 +------------------+
|  dim_customers   |-----------|    fact_orders    |-----------|   dim_country    |
+------------------+           +-------------------+           +------------------+
                                       | 1
                                       | 
                                       | *
                               +-------------------+ *       1 +------------------+
                               | fact_order_items  |-----------|   dim_products   |
                               +-------------------+           +------------------+
                                                                        | *
                                                                        | 1
                                                               +------------------+
                                                               |  dim_categories  |
                                                               +------------------+
```

### Table Specifications:

- **`fact_orders`**: Transaction-level header data (`order_id`, `customer_id`, `order_date`, `country_id`, `payment_method`, `channel`).
- **`fact_order_items`**: Line-item granularity (`order_item_id`, `order_id`, `product_id`, `quantity`, `item_price`, `discount_amount`).
- **`dim_customers`**: Demographic and tier data (`customer_id`, `customer_name`, `email`, `loyalty_tier`, `signup_date`).
- **`dim_products`**: Catalog dimension (`product_id`, `product_name`, `category_id`, `unit_cost`, `retail_price`).
- **`dim_categories`**: Product classifications (`category_id`, `category_name`, `department`).
- **`dim_country`**: Geographic hierarchy (`country_id`, `country_name`, `region`, `currency_code`).
- **`dim_date`**: Comprehensive enterprise calendar table supporting Time Intelligence DAX.

---

## ⚙️ ETL & Power Query Pipeline

1. **Extraction & Format Standardization:** Ingested source tabular data from CSV and Excel repositories, ensuring strict type enforcement (`Currency`, `Int64`, `DateTime`).
2. **Key Harmonization & Surrogate Key Creation:** Generated composite primary keys where applicable and cleansed null values across foreign key columns.
3. **Derived Attributes & Bucketing:** Created customer loyalty tiers based on historical spend thresholds and generated date-hierarchy columns (`Year`, `Quarter`, `Month`, `MonthName`, `DayOfWeek`).
4. **Data Quality & Integrity Checks:** Verified 0 orphaned foreign keys between `fact_order_items`, `fact_orders`, and supporting dimension tables.

---

## 📁 Repository Structure

```
PULSE-Analytics/
├── Dashboard Previews/             # High-resolution dashboard screenshots
│   ├── Country Page.png           # Regional & Geographic Market Penetration
│   ├── Customer Page.png          # RFM Cohort & Customer Value Analysis
│   ├── Landing Page.png           # Executive Portal Navigation Hub
│   ├── Model Page.png             # Snowflake Schema Architecture View
│   ├── Overview Page.png          # Executive Overview & Core KPIs
│   ├── Products Page.png          # SKU Assortment & Category Yield
│   └── Recommendation Page.png    # What-If Predictive Simulation Dashboard
│
├── Data/                          # Structured source transactional datasets
│   ├── dim_categories.csv         # Product category dimension
│   ├── dim_country.csv            # Geographic & market dimension
│   ├── dim_customers.csv          # Customer profile & loyalty tier data
│   ├── dim_date.csv               # Calendar and time dimension
│   ├── dim_products.csv           # Product catalog and pricing table
│   ├── fact_order_items.csv       # Line-item order transaction details
│   └── fact_orders.csv            # Order header records
│
├── PULSE.pbip                     # Power BI Project metadata & PBIP definition
├── PULSE.Report/                  # Tabular report layout, visual definitions & theme
├── PULSE.SemanticModel/           # Model definition, relationships & TMDL scripts
├── LICENSE                        # Repository MIT License
└── README.md                      # Comprehensive project documentation
```

---

## 🛠️ Tools & Technologies

- 📊 **Power BI Desktop:** Multi-page interactive executive dashboards, dynamic bookmark navigation, and responsive matrix visuals.
- 📐 **DAX (Data Analysis Expressions):** Complex Time Intelligence (`DATEADD`, `SAMEPERIODLASTMONTH`), ratio metrics, and What-If parameter modeling.
- 🗄️ **Power BI Project (PBIP) & TMDL:** Modern developer workflow enabling version-controlled tabular metadata.
- ⚡ **Power Query (M):** Multi-table extraction, schema normalization, and data validation pipeline.
- 🏗️ **Dimensional Data Modeling:** Star and snowflake schema architectures optimized for analytical query performance.

---

## 📜 License & Author

- **Author:** Kerelos Nakhla ([GitHub](https://github.com/Kerelos-Nakhla))
- **Portfolio:** [Kerelos Nakhla Portfolio](https://github.com/Kerelos-Nakhla/Portofolio)
- **Email:** kerelosnakhlasaad@gmail.com
- **License:** MIT License
