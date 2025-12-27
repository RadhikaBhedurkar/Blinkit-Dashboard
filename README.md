# Blinkit-Dashboard
A Blinkit Dashboard in Power BI is an interactive business intelligence report designed to visualize and analyze key performance metrics for Blinkit — a quick-commerce grocery delivery platform. Built using Microsoft Power BI, this dashboard transforms raw sales and operational data into meaningful insights to support strategic decision-making.

# Purpose

The main goal of the Blinkit Dashboard is to provide stakeholders (e.g., business analysts, managers, and decision-makers) with an at-a-glance view of business performance, customer behavior, and product trends. It uncovers patterns, highlights opportunities, and enables data-driven decisions for sales optimization, inventory planning, and market expansion.

## 📌 Key Features

### 📊 Summary KPIs
Top cards display:
- 💰 **Total Sales**
- 📈 **Average Sales**
- 🛍️ **Number of Items**
- ⭐ **Average Rating**

### 🧭 Trend & Time Analysis
A trend chart plots **Outlet Establishment Sales** over time, highlighting key milestones and revenue growth.

### 🗂️ Sales Breakdown

#### By Product
- Bar charts for **Item Types** with dollar values.
- Donut charts showing **Fat Content** distribution (Low-Fat vs Regular).

#### By Outlet
- Comparison of fat content contribution per outlet tier.
- **Outlet Location** and **Outlet Size** donut/bullet visuals.

### 🏬 Outlet Type Analytics
Tabular summary showing:
- Total Sales
- No. of Items
- Avg Sales
- Avg Rating
- Item Visibility

For each outlet type such as:
- Supermarket Type 1
- Supermarket Type 2
- Supermarket Type 3
- Grocery Store

### 🔄 Filters
- Outlet Location Type
- Outlet Size
- Item Type  
Used to interactively filter the entire dashboard.

---

## 📁 Files & Structure

📦 blinkit-powerbi-dashboard
┣ 📂 data
┃ ┗ blinkit_sales_data.csv
┣ 📂 reports
┃ ┗ Blinkit_Dashboard.pbix
┣ 📂 visuals
┃ ┗ (image & mockups)
┣ README.md

---

## 🛠 How to Use

1. **Clone the repository**
   ```bash
   git clone https://github.com/<your-username>/blinkit-powerbi-dashboard.git
Open the Power BI File

Load Blinkit_Dashboard.pbix in Microsoft Power BI Desktop.

Load the Data

Ensure the dataset (CSV/SQL) is connected and refreshed.

Interact with Filters & Visuals

Use filter panel to explore different segment combinations and insights.

📊 Data Model
Table	Description
Sales	Transactional sales data by item, outlet, and date
Outlets	Metadata for outlet tiers, size, and location
Products	Product details (Type, Fat Content, Category)

🧮 Measures (Example DAX)
DAX
Copy code
Total Sales = SUM(Sales[SalesAmount])

Avg Sales = AVERAGE(Sales[SalesAmount])

No Of Items = DISTINCTCOUNT(Sales[ItemID])

Avg Rating = AVERAGE(Sales[Rating])
📌 Visuals Used
Card visuals for KPIs

Line charts for trend analysis

Donut & pie charts for distributions

Bar charts for category comparisons

Tables with conditional formatting

📈 Business Value
This dashboard enables:

✔ Quick assessment of Blinkit’s sales performance
✔ Identification of product and outlet strengths & weaknesses
✔ Insight-driven decisions on inventory, promotions, and operations



