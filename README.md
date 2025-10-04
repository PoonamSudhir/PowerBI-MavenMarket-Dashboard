# 📊 Maven Market Power BI Project

## Objective  
Designed and developed an interactive Power BI report for **Maven Market** to analyze sales, returns, customer demographics, and store performance across multiple regions and years.  
The goal was to build a robust data model and deliver **executive-level insights** on topline performance, profitability, and return trends.  

---

## 🔹 Key Steps & Deliverables  

### 1. Data Preparation & Cleaning (Power Query)  
- Imported and transformed multiple CSV sources (Customers, Products, Stores, Regions, Calendar, Returns, Transactions).  
- Ensured correct data types (IDs as whole numbers, prices as decimals, etc.).  
- Created calculated columns (e.g., `full_name`, `birth_year`, `has_children`, `discount_price`, `full_address`, `area_code`, `Price_Tier`).  
- Handled missing values (replaced nulls with zeros for product attributes).  
- Combined multi-year transaction files into a single **Transaction_Data fact table**.  

### 2. Data Modeling  
- Built a **star schema** with fact tables (Transactions & Returns) connected to lookup tables (Customers, Products, Stores, Calendar, Regions).  
- Enforced **one-to-many relationships** with single filter direction.  
- Implemented **snowflake schema** for Stores → Regions.  
- Hid foreign keys and optimized field categories (City, Country, Postal Code, Address, etc.).  

### 3. Calculations (DAX)  
Created KPI measures such as:  
- Quantity Sold: **833,489**  
- Quantity Returned: **8,289**  
- Return Rate: **0.99%**  
- Total Revenue: **$1.76M**  
- Total Profit: **$1.05M**  
- Profit Margin: **59.7%**  
- Weekend Transactions: **28.4% of total**  
- YTD Revenue and 60-Day Rolling Revenue  
- Prior-month benchmarks for Transactions, Revenue, Profit, and Returns  
- Revenue Target based on **+5% MoM growth**  

### 4. Report Development (Power BI)  
- Designed a **Topline Performance dashboard** with:  
  - Matrix of Profitability & Returns by Product Brand (Top 30) with conditional formatting  
  - KPI Cards for Transactions, Profit, and Returns vs. last month  
  - Map & Treemap visuals for store and regional performance  
  - Weekly Revenue Trending chart (1998 focus)  
  - Gauge Chart showing Revenue vs. Target  
- Added slicers, drill-downs, bookmarks, and buttons for **interactive storytelling** (e.g., “Portland hits 1,000 sales in December”).  

---

## 🔹 Outcome & Insights  
- Delivered a **clean, scalable data model** supporting historical analysis across 2 years.  
- Identified **high-margin product brands** and **return hotspots**.  
- Demonstrated that **weekend sales accounted for 28%** of total transactions and **profit margins averaged nearly 60%**.  
- Enabled executives to track revenue against monthly targets and quickly identify underperforming regions or products.  

---

## ✅ Skills Used  
**Power BI Desktop**, **Power Query**, **DAX**, **Data Modeling (Star Schema)**, **KPI Development**, **Bookmarks**, **Report Design**, **Data Storytelling**.  

---

## 📂 Files in this Repository  
- `MavenMarket_Dashboard.pbix` → Power BI report file  
- `Screenshots/` → Dashboard visuals  
- `README.md` → Project documentation  

---

📈 *Created as part of the Maven Analytics “Power BI for Business Intelligence” course project.*  

