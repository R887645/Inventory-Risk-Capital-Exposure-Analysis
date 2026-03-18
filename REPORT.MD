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
- Built dimensional tables:
  - Product
  - Supplier
  - Warehouse
  - Stock Status
- Linked dimension tables to a central fact table
- Created calculated fields for:
  - Portfolio percentage
  - Supplier dependency
  - Risk levels
- Validated formulas to ensure metric accuracy

---

## Wireframing (Figma)

Before building the Excel dashboards, wireframes were designed in Figma to plan the **layout, navigation, and storytelling flow**.

### Wireframe Pages

**Home Page**
- High-level overview of the inventory system
- Navigation buttons to analysis pages

**Table Analysis Page**
- Detailed breakdown of capital exposure by:
  - Product
  - Supplier
  - Warehouse

**Risk Pages**
- Category risk tables
- Supplier dependency flags
- Warehouse risk indicators

Wireframing ensured clarity of design and reduced rework during dashboard implementation.

---

## Table Analysis Page

This page served as the **foundation of the entire analysis**, providing the detailed numerical breakdown supporting the dashboards.

### Key Components

- Total capital exposure by **product**
- Capital exposure by **stock status**
- Supplier dependency indicators
- Warehouse distribution of inventory capital

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

## Dashboard Overview

The Excel dashboards developed for this project include:

### Inventory Capital & Stock Risk
- Total capital exposure
- Product capital breakdown
- Stock status distribution

### Supplier & Warehouse Analysis
- Supplier dependency levels
- Lead time evaluation
- Warehouse capital distribution

### Category Risk Tables
- Portfolio share by category
- Dependency flags
- Risk levels

### Table Analysis Page
- Detailed numeric breakdown supporting dashboard visuals

---

## Limitations

- Dataset represents a **single snapshot** rather than long-term trends
- External market factors such as **seasonality and demand shifts** were not included
- Supplier performance metrics were limited to **dependency and lead time**

---

## Conclusion

This project transformed raw inventory data into clear, actionable insights. By combining **Excel dashboards** with **Figma wireframes**, the analysis revealed significant capital tied up in overstock inventory, supplier dependency risks, and warehouse exposure patterns.

The structured table analysis page and dashboards give management clear visibility to optimize inventory decisions, reduce inefficiencies, and support smarter operational planning.**

---

## About Me

I am **Abdul-Azeez Rofiah Kehinde**, a Data Analyst specializing in **sales, Marketing and Ecommerce analytics**.

In this project, I use **Excel and Figma** to clean, model, and visualize data, delivering dashboards and wireframes that tell a clear business story and empower stakeholders to make confident, data-driven decisions.
