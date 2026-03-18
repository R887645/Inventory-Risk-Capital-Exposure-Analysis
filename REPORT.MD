# Inventory Risk & Capital Exposure Analysis  
## Managing Exposure Across Products, Suppliers & Warehouses

---

## Business Problem / Objective

A distribution company managing inventory across multiple warehouses suspected several operational risks:

- Excessive capital tied up in inventory
- Overstock and understock imbalances across products
- Rising supplier dependence creates risk
- Warehouse concentration exposes vulnerabilities

The objective of this analysis was to interrogate raw inventory data, identify risk areas, and present **actionable insights to management for smarter stock decisions and reduced inefficiencies.**

---

## Dataset Overview

**Source:** Raw inventory dataset provided by EasyTech Challenge  

**Time Period:** Current warehouse snapshot  

**Coverage:** Multi-warehouse, multi-supplier distribution network  

**Data Type:** Inventory records  

### Key Columns

- Product Name
- Stock Status *(Overstock, Understock, Safe Zone, Out of Stock)*
- Capital Exposure (₦)
- Supplier Name
- Warehouse Location
- Inventory Value
- Dependency & Risk Level

![My Image](https://github.com/R887645/Inventory-Risk-Capital-Exposure-Analysis/blob/main/Inventory%20Dataset_Raw.png?raw=true)

---

## Tools Used

**Excel**

- Data cleaning
- Pivot tables
- Calculations
- Dashboard creation

**Figma**

- Wireframing dashboard layouts before building in Excel
- Structuring the storytelling flow of the report

---

## Data Cleaning & Preparation

Several data preparation steps were performed to ensure reliable analysis:

- Removed duplicate records
- Standardized product, supplier, and warehouse naming
- Converted capital exposure into numeric fields

![My Image](https://github.com/R887645/Inventory-Risk-Capital-Exposure-Analysis/blob/main/inventory_Before%20Cleaning.png?raw=true)


![My Image](https://github.com/R887645/Inventory-Risk-Capital-Exposure-Analysis/blob/main/Inventory_data%20cleaning.png?raw=true)

- Built dimensional tables:
  - Product
  - Supplier
  - Warehouse
  - date
- Linked dimension tables to a central fact table
- Created calculated fields for:
  - Stock Status
- Validated formulas to ensure metric accuracy

![My Image](https://github.com/R887645/Inventory-Risk-Capital-Exposure-Analysis/blob/main/inventory_data%20modelling.png?raw=true)

- Created DAX Measures to ensure accurate Analysis
- Total Capital Exposure
- Total Inventory Value
- Understock Product Count
- Overstocked Counts
-Total SKUs and lots more

![My Image](https://github.com/R887645/Inventory-Risk-Capital-Exposure-Analysis/blob/main/Inventory_DAX.png?raw=true)

---

## Pivot Table
The pivot tables were used to summarize and break down the inventory data into clear, actionable views. They allow quick comparisons across product categories, suppliers, and warehouses, showing where capital is concentrated and where risks such as overstock or stockouts are most severe. By grouping and filtering the data, the pivot tables highlight patterns that are not immediately visible in raw records, making it easier for management to detect inefficiencies, monitor exposure, and focus on the areas that require urgent attention.

![My Image](https://github.com/R887645/Inventory-Risk-Capital-Exposure-Analysis/blob/main/inventory_Pivot%20Table%201.png?raw=true)

## Wireframing (Figma)

Before building the Excel dashboards, wireframes were designed in Figma to plan the **layout, navigation, and storytelling flow**.

### Wireframe Pages

**Capital & Stock Risk Analysis + Supplier & Warehouse Conc Analysis**
- High-level overview of the inventory system
- Navigation buttons to analysis pages


Wireframing ensured clarity of design and reduced rework during dashboard implementation.

![My Image](https://github.com/R887645/Inventory-Risk-Capital-Exposure-Analysis/blob/main/Inventory_WIREFRAMING.png?raw=true)

---

## Dashboard Overview

The Excel dashboards developed for this project include:

### Inventory Capital & Stock Risk
- Total capital exposure
- Product capital breakdown
- Stock status distribution

![My Image](https://github.com/R887645/Inventory-Risk-Capital-Exposure-Analysis/blob/main/Capital%20and%20Stock%20isk%20Analysis.png?raw=true)

### Supplier & Warehouse Concentration Analysis
- Supplier dependency levels
- Lead time evaluation
- Warehouse capital distribution
![My Image](https://github.com/R887645/Inventory-Risk-Capital-Exposure-Analysis/blob/main/Supplier%20and%20Warehouse%20Conc%20Analysis.png?raw=true)

### Category Risk Tables
- Portfolio share by category
- Dependency flags
- Risk levels

---
## Table Analysis Page

This page served as the **foundation of the entire analysis**, providing the detailed numerical breakdown supporting the dashboards.

**Table Analysis Page**
- Detailed breakdown of capital exposure by:
  - Category
  - Supplier
  - Warehouse

![My Image](https://github.com/R887645/Inventory-Risk-Capital-Exposure-Analysis/blob/main/Table%20Analysis.png?raw=true)

## Inventory Risk Insights

### Category Risk

All categories show **High Risk**, driven by the following factors:

- **Overstock dominance:** Each category has **430+ overstocked items**
- **Stockouts present:** Even **1–2 out-of-stock items** trigger risk flags
- **Weak Safe Zone:** Safe stock items range between **61–89**, far below overstock levels
- **Balanced Portfolio Share:** `%Portfolio` ranges from **19–21%**, therefore **Dependency = Medium**

**Insight:**  
Even distribution of capital across categories does **not reduce risk** — overall inventory health is poor across all categories.

---

### Supplier Risk

All suppliers are flagged **High Risk**, due to:

- **Overstock counts:** Between **432–667 items**
- **Stockouts present:** **4 out of 5 suppliers** show stockouts
- **Safe Zone levels:** Safe stock is significantly lower than overstock levels
- **Portfolio Share:** `%Portfolio` ranges from **19–22%**, resulting in **Dependency = Medium**

**Insight:**  
No supplier dominates the portfolio, but **all suppliers carry unhealthy stock mixes**.  
**MegaBuild Ltd** is particularly risky with **667 overstocked items**.

---

### Warehouse Risk

All warehouses are correctly flagged **High Risk**:

- **Overstock ratios exceed 60%** in every warehouse
- **Stockouts exist** across locations (**1–5 items**)
- **Safe Zone counts** are lower than overstock
- **Capital Share:** `%Share` is evenly split (**33–34%**), meaning **Dependency = Balanced**

**Insight:**  
Despite balanced distribution across warehouses, **excess stock concentration is driving operational risk** and increasing inventory carrying costs.

![My Image](https://github.com/R887645/Inventory-Risk-Capital-Exposure-Analysis/blob/main/Table%20Analysis.png?raw=true)


### Key Components

- Total capital exposure by **product**
- Capital exposure by **stock status**
- Supplier dependency indicators
- Warehouse distribution of inventory capital

![My Image](https://github.com/R887645/Inventory-Risk-Capital-Exposure-Analysis/blob/main/Inventory_WIREFRAMING.png?raw=true)

### Key Findings

- Overstock dominates the inventory portfolio  
- Approximately **₦167.9M (~60%)** of total inventory is tied up in overstock
- Around **₦5M** of capital is exposed to stockout risk

---

## Key Business Questions

The analysis aimed to answer the following questions:

1. Which products tie up the most capital in overstock?
2. How much capital is exposed to stockout risk?
3. Which suppliers show high dependency and risk concentration?
4. How balanced is capital exposure across warehouses?
5. Which product categories contribute most to portfolio risk?

---

## Key Insights

- **₦187.4M** total inventory value across all warehouses
- **₦167.9M** locked in overstock inventory
- Supplier dependency flagged as **High** across multiple product categories
- Warehouse capital share appears balanced (~33% each), but **product mix drives risk**
- Lead time analysis suggests potential **restocking delays**

**[View My Full Slides](https://drive.google.com/file/d/1HdGUN9Lbn6HIDUbpL_MXwLSa3Md0T3oI/view?usp=sharing)**
---

## Recommendations

### 1. Reduce Overstock
Adjust procurement quantities and restocking cycles to free up capital currently tied in excess inventory.

### 2. Diversify Suppliers
Reduce dependency risk by expanding the supplier base for critical products.

### 3. Monitor Understock
Track low-stock products closely to prevent lost sales and operational disruption.

### 4. Balance Warehouse Mix
Distribute product categories more evenly across warehouses to minimize exposure concentration.

### 5. Implement Predictive Restock Modeling
Introduce trend-based restocking models to anticipate demand and reduce inventory risk early.

---


## Limitations

- Dataset represents a **single snapshot** rather than long-term trends
- External market factors such as **seasonality and demand shifts** were not included
- Supplier performance metrics were limited to **dependency and lead time**

---

## Conclusion

This project transformed raw inventory data into clear, actionable insights. By combining **Excel dashboards** with **Figma wireframes**, the analysis revealed significant capital tied up in overstock inventory, supplier dependency risks, and warehouse exposure patterns.

The structured table analysis page and dashboards give management clear visibility into optimizing inventory decisions, reducing inefficiencies, and supporting smarter operational planning.**

---

## About Me

I am **Abdul-Azeez Rofiah Kehinde**, a Data Analyst specializing in **sales, Marketing and Ecommerce analytics**.

In this project, I use **Excel and Figma** to clean, model, and visualize data, delivering dashboards and wireframes that tell a clear business story and empower stakeholders to make confident, data-driven decisions.
