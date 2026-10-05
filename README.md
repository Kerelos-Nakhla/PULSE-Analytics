# 📊 PULSE Analytics — E-Commerce Sales & Customer Intelligence Dashboard

<p align=center>
  <b>Enterprise E-Commerce Sales Intelligence, Customer RFM Segmentation, Basket Composition & What-If Predictive Simulation in Power BI</b>
</p>

<p align=center>
  <img src="https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black" alt="Power BI" />
  <img src="https://img.shields.io/badge/DAX-Time_Intelligence_&_What--If-blue?style=for-the-badge" alt="DAX" />
  <img src="https://img.shields.io/badge/Data_Modeling-Snowflake_Schema-success?style=for-the-badge" alt="Data Modeling" />
  <img src="https://img.shields.io/badge/Analytics-RFM_Customer_Tiers-orange?style=for-the-badge" alt="RFM Tiers" />
  <img src="https://img.shields.io/badge/Simulation-Parameter_Modeling-brightgreen?style=for-the-badge" alt="Simulation" />
</p>

---

## 📌 Executive Overview

The **PULSE Analytics E-Commerce Sales & Customer Intelligence Dashboard** is an enterprise-grade commercial decision-support platform engineered in **Microsoft Power BI**. Designed for digital retail executives, commercial strategists, and marketing directors, it translates granular transactional line items, regional sales across West African markets, customer behavioral tiers, and catalog performance into high-impact operational intelligence.

The platform monitors **11,000 distinct orders** comprising **21,931 line items** and **65,713 units sold** across **500 registered customers** in **4 international markets**, governing **6,549,730.00 (~6.55M) in gross revenue**. It bridges the gap between historical retrospective reporting and proactive predictive planning through dynamic What-If parameter simulation.



---

## 📊 Commercial Financial Summary & Core KPIs

The enterprise scorecard synthesizes transactional velocity, monetization ratios, and operational volume derived directly from the underlying data:

| Key Performance Indicator | Portfolio Value | Verified DAX Formula | Strategic Commercial Impact |
| :--- | :---: | :---: | :--- |
| **Gross Total Revenue** | **6,549,730.00** |  | Total gross commercial revenue across all completed customer orders |
| **Total Order Volume** | **11,000 Orders** |  | Validated completed digital storefront transactions |
| **Total Units Shipped** | **65,713 Units** |  | Total physical merchandise units fulfilled through distribution centers |
| **Total Line Items** | **21,931 Items** |  | Line-item transaction records processed across the catalog |
| **Active Customer Base** | **500 Accounts** |  | Verified accounts generating recurring transactions |
| **Total Customer Visits** | **2,858 Visits** |  | Aggregate recorded storefront customer engagements |
| **Average Visits / Customer** | **5.72 Visits** |  | Mean visit frequency per customer profile |
| **Storefront Seen Count** | **63,783.79 Views** |  | Total catalog and storefront view impressions |
| **Storefront Conversion Rate** | **17.25%** |  | Checkout funnel efficiency from storefront impressions to completed order |
| **Average Order Value (AOV)** | **,413.61** |  | Mean gross spend realized per completed customer order |
| **Average Order Quantity (AOQ)** | **5.97 Units** |  | Average volume of items purchased per basket |
| **Average Order Items (AOI)** | **1.99 Lines** |  | Average unique SKU line-item depth per customer basket |
| **Revenue per Customer** | **3,099.46** |  | Lifetime value realization per active customer |
| **Revenue per Visit** | **,289.62** |  | Revenue yield generated per storefront visit session |
| **Orders per Customer** | **22.00 Orders** |  | High-frequency repeat purchasing velocity across the customer base |

---

## 👥 Customer Loyalty & Behavioral Tier Segmentation

Customers are categorized across automated behavioral value tiers based on order frequency, revealing deep repeat-purchase loyalty:

| Loyalty Tier | Customers | Customer Share | Orders | Gross Revenue | Revenue Share | Mean Spend / Customer | Orders / Customer |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| **Loyal Repeat (22–27 Orders)** | **184** | **36.8%** | 4,460 | **0,799,000.00** | **40.67%** | **8,690.22** | 24.24 |
| **Core Buyer (16–21 Orders)** | **212** | **42.4%** | 4,007 | **,523,690.00** | **35.87%** | **4,923.07** | 18.90 |
| **VIP Champion (28+ Orders)** | **69** | **13.8%** | 2,047 | **,019,180.00** | **18.90%** | **2,741.74** | 29.67 |
| **Occasional (Under 16 Orders)** | **35** | **7.0%** | 486 | **,207,860.00** | **4.55%** | **4,510.29** | 13.89 |
| **Total / Overall** | **500** | **100.0%** | **11,000** | **6,549,730.00** | **100.0%** | **3,099.46** | **22.00** |

### Strategic Tier Insights
1. **High Repeat Engagement:** Over **93% of the customer base** sits in the Core, Loyal Repeat, or VIP tiers (16+ orders), demonstrating exceptional platform stickiness and product retention.
2. **VIP Revenue Powerhouse:** 69 VIP Champions generate **.02M (18.9%)** at an average spend of **2,741.74**, making dedicated retention and high-touch account management paramount.
3. **Core Backbone:** Core Buyers and Loyal Repeat customers represent **76.54% of total revenue (0.32M)** across 8,467 orders.

---

## 🛍️ Product Catalog & Category Performance

The merchandise catalog spans 3 core product categories and 7 high-value SKUs:

| Product Category | Category Key | Gross Revenue | Revenue Share | Line Items | Units Sold | Dominant Driver |
| :--- | :---: | :---: | :---: | :---: | :---: | :--- |
| **Electronics** | 1 | **7,223,650.00** | **64.87%** | 9,257 | 27,839 | Laptop (.26M) & Smartphone (.59M) |
| **Furniture** | 3 | **,765,600.00** | **21.72%** | 6,410 | 19,196 | Table (.85M) & Chair (.91M) |
| **Home Appliance** | 2 | **,560,480.00** | **13.41%** | 6,264 | 18,678 | Microwave (.82M) & Blender (43K) |

### SKU-Level Breakdown

| SKU Name | Key | Unit Price | Units Sold | Line Items | Total Revenue | Seen Count | Purchase Yield |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| **Laptop** | P001 | ,000 | 9,257 | 3,059 | **,257,000.00** | 2,500 | 4.40 |
| **Smartphone** | P005 | 00 | 9,417 | 3,093 | **,591,900.00** | 3,500 | 3.14 |
| **Table** | P007 | 00 | 9,632 | 3,205 | **,852,800.00** | 1,600 | 6.88 |
| **Microwave** | P006 | 00 | 9,392 | 3,157 | **,817,600.00** | 1,000 | 11.00 |
| **Chair** | P004 | 00 | 9,564 | 3,205 | **,912,800.00** | 3,000 | 3.67 |
| **Headphones** | P002 | 50 | 9,165 | 3,105 | **,374,750.00** | 1,800 | 6.11 |
| **Blender** | P003 | 0 | 9,286 | 3,107 | **42,880.00** | 1,200 | 9.17 |

---

## 🌍 Geographic Penetration & Regional Footprint

Regional performance across 4 West African territories shows balanced commercial distribution:

| Country Market | Key | Total Revenue | Revenue Share | Line Items | Orders | Mean Spend / Order |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: |
| **Côte d'Ivoire** | 4 | **,909,980.00** | **26.03%** | 5,685 | ~2,850 | ,424.55 |
| **Ghana** | 1 | **,764,640.00** | **25.48%** | 5,611 | ~2,800 | ,415.94 |
| **Togo** | 3 | **,750,230.00** | **25.42%** | 5,539 | ~2,795 | ,415.11 |
| **Benin** | 2 | **,124,880.00** | **23.07%** | 5,096 | ~2,555 | ,397.21 |

---

## 📈 What-If Predictive Simulation Model

The semantic model includes dynamic parameter tables (, ) and DAX measures calculating scenario revenue impacts:

1481	ext{Projected Revenue} = 	ext{Seen Count} 	imes (	ext{Conversion Rate} + \Delta 	ext{Conversion}) 	imes (	ext{AOV} + \Delta 	ext{AOV})1481

### Baseline vs. What-If Scenario (+1.5% Conversion Lift, +50 AOV Expansion)

| Metric | Baseline Value | Simulation Value | Net Expansion / Lift |
| :--- | :---: | :---: | :---: |
| **Storefront Conversion Rate** | **17.25%** | **18.75%** (+1.50%) | +8.70% relative conversion gain |
| **Projected Orders** | **11,000** | **11,957 Orders** | **+957 Incremental Orders** |
| **Average Order Value (AOV)** | **,413.61** | **,563.61** | **+50.00 / Basket** |
| **Total Gross Revenue** | **6,549,730.00** | **0,652,384.81** | **+,102,654.81 (+15.45%)** |

---

## 📐 Key DAX Measures & Formula Reference

The semantic model () features governed, reusable DAX calculations:

### 1. Core Volume & Monetization Measures


### 2. Funnel Efficiency & Customer Engagement


### 3. Share of Wallet & Benchmarking


### 4. What-If Predictive Simulation


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



### Table Dictionary & Schema Cardinality

| Table Name | Role | Cardinality | Primary / Foreign Keys | Granularity / Attributes |
| :--- | :---: | :---: | :--- | :--- |
| **** | Fact | 21,931 rows | PK: <br>FK: , , Mon Oct  5 18:41:54 UTC 2026 | Transactional sales line items with quantity, unit price, total amount, seen count |
| **** | Dimension | 500 rows | PK: <br>FK:  | Customer profile, total visits, loyalty tier, loyalty sort index |
| **** | Dimension | 7 rows | PK: <br>FK:  | Product SKU name, price, catalog impressions/seen count |
| **** | Dimension | 3 rows | PK:  | Merchandise category classification and media URLs |
| **** | Dimension | 4 rows | PK:  | Regional market naming and national flag assets |
| **** | Dimension | 365 rows | PK:  | Comprehensive date intelligence calendar dimension |
| **** | Parameter | Dynamic | Numeric Series | What-If conversion rate variance slider (+0.0% to +5.0%) |
| **** | Parameter | Dynamic | Numeric Series | What-If AOV variance slider (+bash to +00) |

---

## 🔄 ETL Pipeline & Data Transformation

Data ingestion, sanitization, and shaping were performed through **Power Query (M)**:
1. **Source Connection:** Parametric loading from Excel workbooks preserving strict column data types.
2. **Key Normalization:** Clean surrogate and natural key bindings (, , ).
3. **Data Integrity Verification:** Elimination of nulls and verification that all fact table transactions map 1:1 to parent dimension tables.
4. **Behavioral Tier Construction:** Segmentation of customer base into validated loyalty bands (, , , ).

---

## 📁 Repository Structure



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
