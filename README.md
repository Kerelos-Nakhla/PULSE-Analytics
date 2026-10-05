# 📊 PULSE Analytics — E-Commerce Sales & Customer Intelligence Dashboard

<p align="center">
  <b>Enterprise E-Commerce Intelligence, Omnichannel Performance Modeling & What-If Revenue Simulation in Power BI</b>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black" alt="Power BI" />
  <img src="https://img.shields.io/badge/DAX-Commercial_Intelligence-blue?style=for-the-badge" alt="DAX" />
  <img src="https://img.shields.io/badge/Data_Modeling-Snowflake_Schema-success?style=for-the-badge" alt="Snowflake Schema" />
  <img src="https://img.shields.io/badge/Simulation-What--If_Parameters-critical?style=for-the-badge" alt="What-If" />
  <img src="https://img.shields.io/badge/License-MIT-lightgrey?style=for-the-badge" alt="License" />
</p>

---

## 📌 Executive Overview

**PULSE Analytics** is an enterprise-grade commercial intelligence and customer behavior dashboard built in Microsoft Power BI. The solution models **11,000 transactions** generating **$26.55M in gross revenue** across **500 verified accounts**, spanning 4 international country markets and 3 product categories over a full fiscal operating year.

Designed around a scalable **Snowflake Schema** and powered by advanced **DAX measures**, the dashboard translates granular session and sales interactions into high-impact operational insights. It features interactive navigation, dynamic MoM (Month-over-Month) growth analysis, basket yield metrics (AOV, AOQ, AOI), customer loyalty tier segmentation, and an interactive **What-If Revenue Simulation Engine** that empowers executives to project bottom-line revenue lift based on targeted conversion and basket-size improvements.

---

## 📊 Executive Scorecard & Core Portfolio Metrics

| Metric Dimension | Value | Business Definition & Strategic Context |
| :--- | :---: | :--- |
| **Gross Revenue** | **$26.55M** | Total settled transaction value across all product categories (`$26,549,730`) |
| **Total Orders** | **11,000** | Distinct completed transaction order count |
| **Total Units Sold** | **65,713** | Cumulative product volume dispatched across all order line items |
| **Average Order Value (AOV)** | **$2,413.61** | Mean gross transaction revenue per completed order |
| **Average Order Quantity (AOQ)** | **5.97** | Average units bundled per checkout order |
| **Average Order Items (AOI)** | **1.99** | Average distinct line-item product depth per transaction |
| **Unique Customer Accounts** | **500** | Transacting commercial accounts tracked across customer profiles |
| **Total Customer Visits** | **2,858** | Cumulative authenticated storefront engagement sessions |
| **Website Seen Count** | **63,784** | Aggregated storefront traffic impressions recorded across sessions |
| **Conversion Yield %** | **17.25%** | Aggregate conversion yield from storefront impressions to confirmed orders |
| **Revenue per Customer** | **$53,099** | Mean customer annual revenue contribution across the portfolio |
| **Revenue per Visit** | **$9,289.62** | Mean realized revenue generated per authenticated site visit |

---

## 🧭 Multi-Page Analytical Framework & Visual Tour

### 1. Executive Landing Portal (`Landing Page.png`)
* **Purpose**: Serves as the high-impact gateway into the analytics suite, establishing clear user context, navigation pathways, and analytical scope.
* **Key Components**: Clean dark-themed aesthetic, executive branding, direct jump-links to all analytical modules, and project metadata.

<p align="center">
  <img src="Dashboard%20Previews/Landing%20Page.png" alt="Executive Landing Portal" width="900" />
</p>

---

### 2. Commercial Overview & Executive KPIs (`Overview Page.png`)
* **Purpose**: Synthesizes top-line commercial health, volume growth, and category revenue distribution.
* **Key Visuals & Findings**:
  * **KPI Summary Cards**: Real-time tracking of Total Revenue ($26.55M), Total Orders (11.00K), AOV ($2,414), AOQ (5.97), AOI (1.99), and Storefront Conversion Rate (17.25%).
  * **Month-over-Month (MoM) Growth Engine**: DAX time-intelligence comparing current month performance against Same Period Last Month (`SPLM`).
  * **Category Contribution Mix**: Revenue breakdown showing product category share and contribution margin across top product families.

<p align="center">
  <img src="Dashboard%20Previews/Overview%20Page.png" alt="Commercial Overview" width="900" />
</p>

---

### 3. Customer Intelligence & Loyalty Tiers (`Customer Page.png`)
* **Purpose**: Decodes buyer behavior, session frequency, and value concentration across customer loyalty cohorts.
* **Key Visuals & Findings**:
  * **Cohort Analysis**: Deep dive into customer visit velocity, repeat order behavior, and orders per customer (`22.0 orders/customer`).
  * **Loyalty Tier Distribution**: Performance breakdown across **Platinum**, **Gold**, and **Silver** tiers to identify high-value accounts.
  * **Traffic Monetization**: Comparative matrix evaluating `Revenue per Visit` ($9,290) and `Order per Visit` (3.85) against engagement depth.

<p align="center">
  <img src="Dashboard%20Previews/Customer%20Page.png" alt="Customer Intelligence" width="900" />
</p>

---

### 4. Regional & Geographic Penetration (`Country Page.png`)
* **Purpose**: Evaluates market expansion and regional revenue contribution across international territories.
* **Key Visuals & Findings**:
  * **Territory Breakdown**: Comparative performance across sovereign markets (United Kingdom, Germany, France, and United States).
  * **Regional Revenue Share**: Dynamic allocation measuring market concentration and localized conversion effectiveness.
  * **Order Density by Geography**: Cross-market comparison of Average Order Values and basket compositions.

<p align="center">
  <img src="Dashboard%20Previews/Country%20Page.png" alt="Country Analysis" width="900" />
</p>

---

### 5. Product Assortment & Yield Performance (`Products Page.png`)
* **Purpose**: Scrutinizes catalog velocity, price elasticity, and product discovery yield.
* **Key Visuals & Findings**:
  * **Product Yield Matrix**: Measures `Purchase Yield` (`Orders / Product Seen Count`) to evaluate which items drive high-intent conversion vs. passive browsing.
  * **Catalog Revenue Contribution**: Pareto distribution isolating hero SKUs from long-tail inventory.
  * **Volume vs. Price Analysis**: Evaluation of item pricing tiers against units dispatched and re-order rates.

<p align="center">
  <img src="Dashboard%20Previews/Products%20Page.png" alt="Products Analysis" width="900" />
</p>

---

### 6. Strategic Recommendations & What-If Simulation (`Recommendation Page.png`)
* **Purpose**: Bridges descriptive analytics and strategic action through an interactive what-if simulation model.
* **Key Visuals & Findings**:
  * **Dynamic What-If Sliders**: Real-time parameters allowing leadership to test scenarios for **Conversion Rate Lift** (+0.5% to +5.0%) and **AOV Expansion** (+$50 to +$300).
  * **Projected Revenue Impact**: Instant calculation of `Projected Revenue` and `Incremental Revenue Gain` unlocked through targeted commercial initiatives.
  * **Strategic Action Playbooks**: Prescriptive recommendations targeting checkout friction, cross-selling incentives, and customer re-engagement.

<p align="center">
  <img src="Dashboard%20Previews/Recommendation%20Page.png" alt="Recommendations & What-If Simulation" width="900" />
</p>

---

### 7. Data Architecture & Schema Diagram (`Model Page.png`)
* **Purpose**: Full architectural transparency demonstrating strict normalization, star-to-snowflake relationships, and 1-to-many cardinality integrity.

<p align="center">
  <img src="Dashboard%20Previews/Model%20Page.png" alt="Data Model Architecture" width="900" />
</p>

---

## 📐 Core DAX Measures & Formulas Reference

All business logic and KPI calculations are centralized within a dedicated measure table (`c_measures`), formatted with standard casing and documentation annotations.

### 1. Volume & Revenue Fundamentals

#### Total Revenue
```dax
total_revenue = SUM(fact_sales[total_amount])
```
*Calculates gross recognized revenue across all completed sales transactions.*

#### Total Orders
```dax
total_order = DISTINCTCOUNT(fact_sales[order_key])
```
*Counts distinct order transactions, preventing duplication across multi-item line rows.*

#### Total Quantity & Total Items
```dax
total_quantity = SUM(fact_sales[quantity])

total_items = COUNTROWS(fact_sales)
```
*Tracks total physical unit volume and distinct line-item records logged in the fact table.*

---

### 2. Basket Composition & Efficiency Ratios

#### Average Order Value (AOV)
```dax
aov = DIVIDE([total_revenue], [total_order])
```
*Measures average revenue yield per transaction. Benchmark: `$2,413.61`.*

#### Average Order Quantity (AOQ)
```dax
aoq = DIVIDE([total_quantity], [total_order])
```
*Measures units packed per order. Benchmark: `5.97 units/order`.*

#### Average Order Items (AOI)
```dax
aoi = DIVIDE([total_items], [total_order])
```
*Measures distinct SKU breadth per transaction. Benchmark: `1.99 items/order`.*

---

### 3. Time Intelligence & MoM Dynamics

#### Same Period Last Month (SPLM) Orders & Revenue
```dax
splm_total_order = 
CALCULATE(
    [total_order], 
    DATEADD(dim_date[Date], -1, MONTH)
)

splm_total_revenue = 
CALCULATE(
    [total_revenue], 
    DATEADD(dim_date[Date], -1, MONTH)
)
```
*Shifts evaluation context back by one complete calendar month using standard Gregorian date dimensions.*

#### Month-over-Month Growth %
```dax
growth_revenue = 
DIVIDE(
    [total_revenue] - [splm_total_revenue], 
    [splm_total_revenue]
)

growth_order = 
DIVIDE(
    [total_order] - [splm_total_order], 
    [splm_total_order]
)
```
*Computes relative revenue and order momentum month-over-month.*

---

### 4. Conversion & Customer Engagement

#### Storefront Conversion Rate
```dax
seen_count_website = SUM(fact_sales[seen_count])

conversion_rate = DIVIDE([total_order], [seen_count_website])
```
*Measures transaction completion efficiency against recorded website traffic. Overall baseline: `17.25%`.*

#### Customer Value & Engagement Intensity
```dax
total_customers = DISTINCTCOUNT(fact_sales[customer_key])

revenue_per_customer = DIVIDE([total_revenue], [total_customers])

order_per_customer = DIVIDE([total_order], [total_customers])

revenue_per_visit = DIVIDE([total_revenue], [total_visits_customers])

order_per_visit = DIVIDE([total_order], [total_visits_customers])
```
*Quantifies customer-centric monetization, tracking annual revenue per account ($53.1K) and visit conversion.*

#### Share of Wallet / Regional Share
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
```
*Calculates relative percentage contribution against selected category and country benchmarks.*

---

### 5. What-If Predictive Simulation Modeling

The recommendation engine implements decoupled parameter tables (`conversion_lift` and `aov_lift`) generated via `GENERATESERIES`, allowing users to adjust expected conversion and AOV increases dynamically.

#### Projected Revenue
```dax
projected_revenue = 
VAR _ConversionLift = DIVIDE(SELECTEDVALUE('conversion_lift'[Value], 1.5), 100)
VAR _AOVLift = SELECTEDVALUE(aov_lift[Value], 150)
VAR _ProjectedOrders = [seen_count_website] * ([conversion_rate] + _ConversionLift)
RETURN 
    _ProjectedOrders * ([aov] + _AOVLift)
```

#### Projected Incremental Revenue Gain
```dax
projected_incremental_revenue = [projected_revenue] - [total_revenue]
```
*Instantly isolates the net-new dollar value generated strictly by conversion and basket enhancements.*

---

## 🏗️ Data Architecture & Snowflake Schema Design

The semantic model follows an optimized **Snowflake Schema** design, eliminating data redundancy while maintaining high query performance in Power BI's VertiPaq engine.

```
       +--------------------+
       |    dim_category    |
       +--------------------+
                 | (1:N)
       +--------------------+          +--------------------+
       |    dim_products    |          |    dim_country     |
       +--------------------+          +--------------------+
                 |                              | (1:N)
                 | (1:N)               +--------------------+
                 |                     |   dim_customers    |
                 |                     +--------------------+
                 |                              | (1:N)
                 +------------+   +-------------+
                              |   |
                       +-----------------+          +-----------------+
                       |   fact_sales    | -------- |    dim_date     |
                       +-----------------+  (N:1)   +-----------------+
```

### Table Specifications:

| Table Name | Type | Key Fields | Row Count | Description |
| :--- | :--- | :--- | :---: | :--- |
| **`fact_sales`** | Fact Table | `sales_key` (PK), `order_key`, `product_key` (FK), `customer_key` (FK), `date` (FK) | 21,931 | Granular sales transactions containing quantity, total amount, and seen impressions |
| **`dim_customers`** | Dimension | `customer_key` (PK), `country_key` (FK), `loyalty_tier` | 500 | Account profiles, total engagement visits, and loyalty classification |
| **`dim_products`** | Dimension | `product_key` (PK), `category_key` (FK), `price` | 7 | Catalog items with base price points and cumulative product view impressions |
| **`dim_category`** | Dimension (Outrigger) | `category_key` (PK), `category`, `category_url_pic` | 3 | High-level product categorization outrigger table |
| **`dim_country`** | Dimension (Outrigger) | `country_key` (PK), `country`, `flag_url_pic` | 4 | Geographic dimension containing national markets and flag image assets |
| **`dim_date`** | Dimension | `Date` (PK), `year`, `month_num`, `quarter`, `day_name` | 365 | Comprehensive calendar dimension supporting time intelligence operations |
| **`c_measures`** | Calculation Group | N/A | Measure Store | Centralized measure home containing 25+ DAX calculations |
| **`conversion_lift`** | Parameter Table | `Value` (`0.5` to `5.0` step `0.5`) | 10 | Disconnected calculated table driving what-if conversion sliders |
| **`aov_lift`** | Parameter Table | `Value` (`50` to `300` step `50`) | 6 | Disconnected calculated table driving what-if basket lift sliders |

---

## ⚙️ ETL & Power Query Pipeline

1. **Source Ingestion**:
   * Data extracted from clean normalized Excel workbooks residing in the `Data/` repository folder.
2. **Type Enforcement & Integrity**:
   * Numeric values converted to fixed currency/integer types; transaction dates cast to strict ISO standard format.
3. **Outrigger Normalization**:
   * Normalized `dim_products` into `dim_category` and `dim_customers` into `dim_country` to optimize VertiPaq dictionary compression.
4. **Metadata & URL Annotations**:
   * Flag and category image URLs annotated as `Image URL` data categories for dynamic rendering in table visuals and card headers.

---

## 📁 Repository Structure

```text
PULSE-Analytics/
│
├── Dashboard Previews/             # High-resolution dashboard screenshots
│   ├── Landing Page.png            # Executive landing portal
│   ├── Overview Page.png           # Executive overview & KPIs
│   ├── Customer Page.png           # Customer intelligence & loyalty
│   ├── Country Page.png            # Geographic & market share
│   ├── Products Page.png           # Product catalog & purchase yield
│   ├── Recommendation Page.png     # What-if simulation & recommendations
│   └── Model Page.png              # Snowflake data schema diagram
│
├── Data/                           # Source datasets (Excel workbooks)
│   ├── fact_sales.xlsx             # 21,931 sales transaction records
│   ├── dim_customer.xlsx           # 500 customer profiles & visits
│   ├── dim_product.xlsx            # Product catalog & pricing
│   ├── dim_category.xlsx           # Category reference outrigger
│   ├── dim_country.xlsx            # Country & flag URL outrigger
│   └── dim_date.xlsx               # Calendar table (365 days)
│
├── Assets/                         # Multimedia assets
│   └── Landing Page.mp4            # Showcase video animation
│
├── PULSE Analytics.pbix            # Production Power BI desktop file
├── LICENSE                         # MIT License
└── README.md                       # Comprehensive case study documentation
```

---

## 🛠️ Tools & Technologies

* **Microsoft Power BI Desktop**: Report authoring, visual design, and canvas layouts.
* **DAX (Data Analysis Expressions)**: Dynamic time intelligence, ranking, customer monetization ratios, and what-if simulation logic.
* **Power Query (M Language)**: Automated ETL, data schema structuring, and type transformation.
* **Figma**: Custom UI layout design, background grids, and modern dark-mode canvas framing.
* **Git / GitHub**: Version control and PBIP source asset management.

---

## 👤 Author & Contact

**Kerelos Nakhla**  
*Power BI Developer & Business Intelligence Analyst*  
* **GitHub**: [@Kerelos-Nakhla](https://github.com/Kerelos-Nakhla)  
* **Portfolio**: [Kerelos Nakhla Data Portfolio](https://github.com/Kerelos-Nakhla/Portofolio)

---

## 📜 License

This project is open-source and licensed under the **MIT License**. See the [LICENSE](LICENSE) file for complete details.
