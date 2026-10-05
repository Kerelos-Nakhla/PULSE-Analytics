# 📊 PULSE Analytics — E-Commerce Sales & Customer Intelligence System

<p align="center">
  <b>Enterprise E-Commerce Sales Intelligence, Customer RFM Segmentation, Basket Composition & What-If Predictive Simulation in Power BI</b>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black" alt="Power BI" />
  <img src="https://img.shields.io/badge/DAX-Time_Intelligence_&_What--If-blue?style=for-the-badge" alt="DAX" />
  <img src="https://img.shields.io/badge/Data_Modeling-Snowflake_Schema-success?style=for-the-badge" alt="Data Modeling" />
  <img src="https://img.shields.io/badge/Analytics-RFM_Customer_Tiers-orange?style=for-the-badge" alt="RFM Tiers" />
  <img src="https://img.shields.io/badge/Simulation-Parameter_Modeling-brightgreen?style=for-the-badge" alt="Simulation" />
  <img src="https://img.shields.io/badge/License-MIT-green?style=for-the-badge" alt="MIT License" />
</p>

---

## 📌 Executive Overview

The **PULSE Analytics E-Commerce Sales & Customer Intelligence System** is an enterprise-grade commercial decision-support platform engineered in **Microsoft Power BI**. Designed for digital retail executives, commercial strategists, and marketing directors, it translates granular transactional line items, regional sales velocity across West African markets, customer behavioral tiers, and catalog performance into high-impact operational intelligence.

The platform monitors **11,000 distinct orders** comprising **21,931 line items** and **65,713 units sold** across **500 registered customers** in **4 international markets**, governing **$26,549,730.00 (~$26.55M) in gross revenue**. It bridges historical retrospective reporting with forward-looking predictive planning through dynamic What-If parameter simulation.

```
+----------------------------------------------------------------------------------------------------+
|                                    EXECUTIVE PORTFOLIO AT A GLANCE                                 |
+--------------------------+--------------------------+-----------------------+----------------------+
|    $26,549,730.00 Gross  |       11,000 Orders      |     500 Customers     |   $2,413.61 Mean AOV |
|   65,713 Units Shipped   |    5.97 Units / Basket   |   4 Regional Markets  |   17.25% Conversion  |
+--------------------------+--------------------------+-----------------------+----------------------+
```

---

## 📊 Commercial Financial Summary & Core KPIs

The enterprise scorecard synthesizes transactional velocity, monetization ratios, and operational volume derived directly from the underlying data:

| Key Performance Indicator | Portfolio Value | Verified DAX Formula | Strategic Commercial Impact |
| :--- | :---: | :---: | :--- |
| **Gross Total Revenue** | **$26,549,730.00** | `SUM(fact_sales[total_amount])` | Total gross commercial revenue across all completed customer orders |
| **Total Order Volume** | **11,000 Orders** | `DISTINCTCOUNT(fact_sales[order_key])` | Validated completed digital storefront transactions |
| **Total Units Shipped** | **65,713 Units** | `SUM(fact_sales[quantity])` | Total physical merchandise units fulfilled through distribution centers |
| **Total Line Items** | **21,931 Items** | `COUNTROWS(fact_sales)` | Line-item transaction records processed across the catalog |
| **Active Customer Base** | **500 Accounts** | `DISTINCTCOUNT(fact_sales[customer_key])` | Verified accounts generating recurring transactions |
| **Total Customer Visits** | **2,858 Visits** | `SUM(dim_customers[total_visits])` | Aggregate recorded storefront customer engagements |
| **Average Visits / Customer** | **5.72 Visits** | `AVERAGE(dim_customers[total_visits])` | Mean visit frequency per customer profile |
| **Storefront Seen Count** | **63,783.79 Views** | `SUM(fact_sales[seen_count])` | Total catalog and storefront view impressions |
| **Storefront Conversion Rate** | **17.25%** | `DIVIDE([total_order], [seen_count_website])` | Checkout funnel efficiency from storefront impressions to completed order |
| **Average Order Value (AOV)** | **$2,413.61** | `DIVIDE([total_revenue], [total_order])` | Mean gross spend realized per completed customer order |
| **Average Order Quantity (AOQ)** | **5.97 Units** | `DIVIDE([total_quantity], [total_order])` | Average volume of items purchased per basket |
| **Average Order Items (AOI)** | **1.99 Lines** | `DIVIDE([total_items], [total_order])` | Average unique SKU line-item depth per customer basket |
| **Revenue per Customer** | **$53,099.46** | `DIVIDE([total_revenue], [total_customers])` | Lifetime value realization per active customer |
| **Revenue per Visit** | **$9,289.62** | `DIVIDE([total_revenue], [total_visits_customers])` | Revenue yield generated per storefront visit session |
| **Orders per Customer** | **22.00 Orders** | `DIVIDE([total_order], [total_customers])` | High-frequency repeat purchasing velocity across the customer base |

---

## 👥 Customer Loyalty & Behavioral Tier Segmentation

Customers are categorized across automated behavioral value tiers based on order frequency, revealing deep repeat-purchase loyalty:

| Loyalty Tier | Customers | Customer Share | Orders | Gross Revenue | Revenue Share | Mean Spend / Customer | Orders / Customer |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| **Loyal Repeat (22–27 Orders)** | **184** | **36.8%** | 4,460 | **$10,799,000.00** | **40.67%** | **$58,690.22** | 24.24 |
| **Core Buyer (16–21 Orders)** | **212** | **42.4%** | 4,007 | **$9,523,690.00** | **35.87%** | **$44,923.07** | 18.90 |
| **VIP Champion (28+ Orders)** | **69** | **13.8%** | 2,047 | **$5,019,180.00** | **18.90%** | **$72,741.74** | 29.67 |
| **Occasional (Under 16 Orders)** | **35** | **7.0%** | 486 | **$1,207,860.00** | **4.55%** | **$34,510.29** | 13.89 |
| **Total / Overall** | **500** | **100.0%** | **11,000** | **$26,549,730.00** | **100.0%** | **$53,099.46** | **22.00** |

### Strategic Tier Insights
1. **High Repeat Engagement:** Over **93% of the customer base** sits in the Core, Loyal Repeat, or VIP tiers (16+ orders), demonstrating exceptional platform stickiness and product retention.
2. **VIP Revenue Powerhouse:** 69 VIP Champions generate **$5.02M (18.9%)** at an average spend of **$72,741.74**, making dedicated retention and high-touch account management paramount.
3. **Core Backbone:** Core Buyers and Loyal Repeat customers represent **76.54% of total revenue ($20.32M)** across 8,467 orders.

---

## 🛍️ Product Catalog & Category Performance

The merchandise catalog spans 3 core product categories and 7 high-value SKUs:

| Product Category | Category Key | Gross Revenue | Revenue Share | Line Items | Units Sold | Dominant Driver |
| :--- | :---: | :---: | :---: | :---: | :---: | :--- |
| **Electronics** | 1 | **$17,223,650.00** | **64.87%** | 9,257 | 27,839 | Laptop ($9.26M) & Smartphone ($6.59M) |
| **Furniture** | 3 | **$5,765,600.00** | **21.72%** | 6,410 | 19,196 | Table ($3.85M) & Chair ($1.91M) |
| **Home Appliance** | 2 | **$3,560,480.00** | **13.41%** | 6,264 | 18,678 | Microwave ($2.82M) & Blender ($743K) |

### SKU-Level Breakdown

| SKU Name | Key | Unit Price | Units Sold | Line Items | Total Revenue | Seen Count | Purchase Yield |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| **Laptop** | P001 | $1,000 | 9,257 | 3,059 | **$9,257,000.00** | 2,500 | 4.40 |
| **Smartphone** | P005 | $700 | 9,417 | 3,093 | **$6,591,900.00** | 3,500 | 3.14 |
| **Table** | P007 | $400 | 9,632 | 3,205 | **$3,852,800.00** | 1,600 | 6.88 |
| **Microwave** | P006 | $300 | 9,392 | 3,157 | **$2,817,600.00** | 1,000 | 11.00 |
| **Chair** | P004 | $200 | 9,564 | 3,205 | **$1,912,800.00** | 3,000 | 3.67 |
| **Headphones** | P002 | $150 | 9,165 | 3,105 | **$1,374,750.00** | 1,800 | 6.11 |
| **Blender** | P003 | $80 | 9,286 | 3,107 | **$742,880.00** | 1,200 | 9.17 |

---

## 🌍 Geographic Penetration & Regional Footprint

Regional performance across 4 West African territories shows balanced commercial distribution:

| Country Market | Key | Total Revenue | Revenue Share | Customers | Total Orders | Line Items | Units Sold | Mean AOV |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| **Côte d'Ivoire** | 4 | **$6,909,980.00** | **26.03%** | 130 | 2,849 | 5,685 | 17,062 | $2,425.41 |
| **Ghana** | 1 | **$6,764,640.00** | **25.48%** | 126 | 2,826 | 5,611 | 16,903 | $2,393.72 |
| **Togo** | 3 | **$6,750,230.00** | **25.42%** | 126 | 2,754 | 5,539 | 16,581 | $2,451.06 |
| **Benin** | 2 | **$6,124,880.00** | **23.07%** | 118 | 2,571 | 5,096 | 15,167 | $2,382.29 |

---

## 📅 Monthly Commercial Cadence & Trend Analysis (2024)

| Month | Gross Revenue | Total Orders | Units Shipped | Mean AOV | MoM Revenue Growth | MoM Order Growth |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: |
| **January** | $2,244,190.00 | 945 | 5,659 | $2,374.80 | Baseline | Baseline |
| **February** | $2,067,030.00 | 867 | 5,086 | $2,384.12 | -7.89% | -8.25% |
| **March** | $2,503,530.00 | 1,016 | 6,236 | $2,464.10 | **+21.12%** | **+17.19%** |
| **April** | $2,168,120.00 | 906 | 5,460 | $2,393.07 | -13.40% | -10.83% |
| **May** | $2,320,220.00 | 974 | 5,702 | $2,382.16 | **+7.02%** | **+7.51%** |
| **June** | $2,237,400.00 | 897 | 5,479 | $2,494.31 | -3.57% | -7.91% |
| **July** | $2,277,050.00 | 940 | 5,587 | $2,422.39 | **+1.77%** | **+4.79%** |
| **August** | $2,268,030.00 | 960 | 5,686 | $2,362.53 | -0.40% | **+2.13%** |
| **September** | $2,015,550.00 | 854 | 4,996 | $2,360.13 | -11.13% | -11.04% |
| **October** | $2,257,870.00 | 905 | 5,443 | $2,494.88 | **+12.02%** | **+5.97%** |
| **November** | $2,142,940.00 | 888 | 5,285 | $2,413.22 | -5.09% | -1.88% |
| **December** | $2,047,800.00 | 848 | 5,094 | $2,414.86 | -4.44% | -4.50% |

---

## 📈 What-If Predictive Simulation Model

The semantic model includes dynamic parameter tables (`conversion_lift`, `aov_lift`) and DAX measures calculating scenario revenue impacts:

$$\text{Projected Revenue} = \text{Seen Count} \times (\text{Conversion Rate} + \Delta \text{Conversion}) \times (\text{AOV} + \Delta \text{AOV})$$

### Baseline vs. What-If Scenario (+1.5% Conversion Lift, +$150 AOV Expansion)

| Metric | Baseline Value | Simulation Value | Net Expansion / Lift |
| :--- | :---: | :---: | :---: |
| **Storefront Conversion Rate** | **17.25%** | **18.75%** (+1.50%) | +8.70% relative conversion gain |
| **Projected Orders** | **11,000** | **11,957 Orders** | **+957 Incremental Orders** |
| **Average Order Value (AOV)** | **$2,413.61** | **$2,563.61** | **+$150.00 / Basket** |
| **Total Gross Revenue** | **$26,549,730.00** | **$30,652,384.81** | **+$4,102,654.81 (+15.45%)** |

---

## 📐 Key DAX Measures & Formula Reference

The semantic model (`c_measures`) features 26 governed, reusable DAX calculations:

### 1. Volume & Core Monetization Measures
```dax
total_order = DISTINCTCOUNT(fact_sales[order_key])

total_quantity = SUM(fact_sales[quantity])

total_revenue = SUM(fact_sales[total_amount])

total_items = COUNTROWS(fact_sales)

aoq = DIVIDE([total_quantity], [total_order])

aov = DIVIDE([total_revenue], [total_order])

aoi = DIVIDE([total_items], [total_order])
```

### 2. Time Intelligence & Period-Over-Period Growth
```dax
splm_total_order = CALCULATE([total_order], DATEADD(dim_date[Date], -1, MONTH))

splm_total_revenue = CALCULATE([total_revenue], DATEADD(dim_date[Date], -1, MONTH))

splm_total_quantity = CALCULATE([total_quantity], DATEADD(dim_date[Date], -1, MONTH))

growth_revenue = DIVIDE([total_revenue] - [splm_total_revenue], [splm_total_revenue])

growth_order = DIVIDE([total_order] - [splm_total_order], [splm_total_order])
```

### 3. Funnel Efficiency & Customer Engagement
```dax
seen_count_website = SUM(fact_sales[seen_count])

conversion_rate = DIVIDE([total_order], [seen_count_website])

total_customers = DISTINCTCOUNT(fact_sales[customer_key])

total_visits_customers = SUM(dim_customers[total_visits])

avg_visits = AVERAGE(dim_customers[total_visits])

revenue_per_visit = DIVIDE([total_revenue], [total_visits_customers])

order_per_customer = DIVIDE([total_order], [total_customers])

order_per_visit = DIVIDE([total_order], [total_visits_customers])

revenue_per_customer = DIVIDE([total_revenue], [total_customers])

customer_per_visit = DIVIDE([total_customers], [total_visits_customers])
```

### 4. Share of Wallet & Catalog Yield
```dax
category_rev_share = 
DIVIDE(
    [total_revenue], 
    CALCULATE([total_revenue], ALLSELECTED(dim_category))
)

country_rev_share = 
DIVIDE(
    [total_revenue], 
    CALCULATE([total_revenue], ALLSELECTED(dim_country))
)

seen_count_products = SUM(dim_products[seen_count])

purchase_yield = DIVIDE([total_order], [seen_count_products])
```

### 5. What-If Predictive Simulation
```dax
projected_revenue = 
VAR _ConversionLift = DIVIDE(SELECTEDVALUE('conversion_lift'[Value], 1.5), 100)
VAR _AOVLift = SELECTEDVALUE(aov_lift[Value], 150)
VAR _ProjectedOrders = [seen_count_website] * ([conversion_rate] + _ConversionLift)
RETURN
    _ProjectedOrders * ([aov] + _AOVLift)

projected_incremental_revenue = [projected_revenue] - [total_revenue]
```

---

## 🖼️ Dashboard Architecture & Visual Tour

| Page No. | Report Canvas | Strategic Business Focus |
| :---: | :--- | :--- |
| **01** | **Landing Page** | Executive portal navigation, thematic brand styling, and platform architecture overview |
| **02** | **Overview Page** | Macro financial performance, KPI scorecards (GMV, AOV, Orders), and MoM growth trajectories |
| **03** | **Customer Page** | Customer loyalty tier distribution, visit frequency, lifetime spend, and repeat order analysis |
| **04** | **Country Page** | Regional market contribution, international territory ranking, and geographic expansion metrics |
| **05** | **Products Page** | Category mix, SKU-level price realization, catalog view-to-order yield, and volume velocity |
| **06** | **Recommendation Page**| What-If predictive simulation sliders (Conversion Lift, AOV Expansion) & incremental revenue |
| **07** | **Model Page** | Entity-Relationship Diagram (Snowflake Schema), cardinalities, and data dictionary |

### Visual Gallery

<div align="center">
  <p><b>01 — Landing Page</b></p>
  <img src="Dashboard%20Previews/Landing%20Page.png" alt="PULSE Analytics - Landing Page" width="850" />
  <br/><br/>
  <p><b>02 — Executive Overview Page</b></p>
  <img src="Dashboard%20Previews/Overview%20Page.png" alt="PULSE Analytics - Overview Page" width="850" />
  <br/><br/>
  <p><b>03 — Customer Intelligence Page</b></p>
  <img src="Dashboard%20Previews/Customer%20Page.png" alt="PULSE Analytics - Customer Page" width="850" />
  <br/><br/>
  <p><b>04 — Country & Geographic Performance Page</b></p>
  <img src="Dashboard%20Previews/Country%20Page.png" alt="PULSE Analytics - Country Page" width="850" />
  <br/><br/>
  <p><b>05 — Product Assortment & Yield Page</b></p>
  <img src="Dashboard%20Previews/Products%20Page.png" alt="PULSE Analytics - Products Page" width="850" />
  <br/><br/>
  <p><b>06 — Recommendation & What-If Simulation Page</b></p>
  <img src="Dashboard%20Previews/Recommendation%20Page.png" alt="PULSE Analytics - Recommendation Page" width="850" />
  <br/><br/>
  <p><b>07 — Data Model Architecture</b></p>
  <img src="Dashboard%20Previews/Model%20Page.png" alt="PULSE Analytics - Model Page" width="850" />
</div>

---

## 🏗️ Data Architecture & Snowflake Schema

The data model is structured as an optimized **Snowflake Schema** centered on transactional sales events:

```
           +--------------------+
           |    dim_category    |
           +---------+----------+
                     | 1
                     |
                     | *
           +---------+----------+         +------------------+
           |    dim_products    |         |     dim_date     |
           +---------+----------+         +--------+---------+
                     | 1                           | 1
                     |                             |
                     | *                         * |
                +----+-----------------------------+----+
                |                   fact_sales          |
                +----+-----------------------------+----+
                     | *                         * |
                     |                             |
                     | 1                           | 1
           +---------+----------+         +--------+---------+
           |   dim_customers    |---------|   dim_country    |
           +--------------------+ *      1+------------------+
```

### Table Dictionary & Schema Cardinality

| Table Name | Role | Cardinality | Primary / Foreign Keys | Granularity / Attributes |
| :--- | :---: | :---: | :--- | :--- |
| **`fact_sales`** | Fact | 21,931 rows | PK: `sales_key`<br>FK: `product_key`, `customer_key`, `date` | Transactional sales line items with quantity, unit price, total amount, seen count |
| **`dim_customers`** | Dimension | 500 rows | PK: `customer_key`<br>FK: `country_key` | Customer profile, total visits, loyalty tier, loyalty sort index |
| **`dim_products`** | Dimension | 7 rows | PK: `product_key`<br>FK: `category_key` | Product SKU name, price, catalog impressions/seen count |
| **`dim_category`** | Dimension | 3 rows | PK: `category_key` | Merchandise category classification and media URLs |
| **`dim_country`** | Dimension | 4 rows | PK: `country_key` | Regional market naming and national flag assets |
| **`dim_date`** | Dimension | 365 rows | PK: `Date` | Comprehensive date intelligence calendar dimension |
| **`conversion_lift`** | Parameter | Dynamic | Numeric Series | What-If conversion rate variance slider (+0.0% to +5.0%) |
| **`aov_lift`** | Parameter | Dynamic | Numeric Series | What-If AOV variance slider (+$0 to +$500) |

---

## 🔄 ETL Pipeline & Data Transformation

Data ingestion, sanitization, and shaping were performed through **Power Query (M)**:
1. **Source Connection:** Parametric loading from Excel workbooks preserving strict column data types.
2. **Key Normalization:** Clean surrogate and natural key bindings (`order_key`, `customer_key`, `product_key`).
3. **Data Integrity Verification:** Elimination of nulls and verification that all fact table transactions map 1:1 to parent dimension tables.
4. **Behavioral Tier Construction:** Segmentation of customer base into validated loyalty bands (`VIP Champion`, `Loyal Repeat`, `Core Buyer`, `Occasional`).

---

## 📁 Repository Structure

```
PULSE-Analytics/
├── Assets/                                # Thematic UI assets and design components
├── Dashboard Previews/                    # High-resolution dashboard page screenshots
│   ├── Landing Page.png
│   ├── Overview Page.png
│   ├── Customer Page.png
│   ├── Country Page.png
│   ├── Products Page.png
│   ├── Recommendation Page.png
│   └── Model Page.png
├── Data/                                  # Source datasets
│   ├── dim_category.xlsx
│   ├── dim_country.xlsx
│   ├── dim_customer.xlsx
│   ├── dim_date.xlsx
│   ├── dim_product.xlsx
│   └── fact_sales.xlsx
├── LICENSE                                # MIT License
├── PULSE Analytics.pbix                   # Production Power BI desktop report
└── README.md                              # Technical documentation & project portfolio
```

---

## 🛠️ Technology Stack & Analytical Tooling

- **Microsoft Power BI Desktop:** Visual orchestration, interactive drill-through, UI/UX architecture.
- **DAX (Data Analysis Expressions):** Time-intelligence, scalar ratios, What-If parameter modeling.
- **Power Query / M Engine:** Data shaping, type coercion, and star/snowflake modeling.
- **Microsoft Excel / Python (Pandas & NumPy):** Pre-ingestion validation and metric benchmarking.
- **Figma:** Canvas wireframing, card grid layout, and executive dashboard iconography.

---

## 👤 Author & Professional Links

**Kerelos Nakhla** — *Data Analyst & BI Developer*  
- 💼 **LinkedIn:** [linkedin.com/in/kerelos-nakhla](https://www.linkedin.com/in/kerelos-nakhla/)  
- 🐙 **GitHub:** [github.com/Kerelos-Nakhla](https://github.com/Kerelos-Nakhla)  
- 🌐 **Portfolio Website:** [kerelos-nakhla.github.io/Portofolio](https://kerelos-nakhla.github.io/Portofolio/)  
- 📧 **Email:** [kerelosnakhlasaad@gmail.com](mailto:kerelosnakhlasaad@gmail.com)

---

## 📄 License

This project is open-source and licensed under the [MIT License](LICENSE).
