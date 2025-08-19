# Coffee Shop Sales Dashboard

**Overview**

The **Coffee Shop Sales Dashboard** provides an at-a-glance, drill-down view of revenue, orders, and quantities across stores, products, days, and hours. Designed for store managers and analysts, the dashboard helps uncover peak times, best-selling items, and month-over-month performance, enabling optimized staffing, inventory, and promotions.

**Tech Stack**

- **Power BI Desktop** (`.pbix` / `.pbit`) – report development and visuals  
- **Power Query (M)** – data ingestion and transformation  
- **DAX** – calculated measures (KPIs, MoM % change, average daily line, conditional formatting)  
- **SQL (T-SQL / `.sql`)** – ETL and reporting views to prepare the data model (`/sql/`)  
- **CSV** – anonymized sample data for reproducibility  
- **Demo / Images** – exported screenshots, GIFs, or short video for quick preview

**Data Source & Structure**

- **Source**: Anonymized POS-style sales data  
- **Tables**:  
  - `sales` (`order_id`, `store_id`, `product_id`, `order_datetime`, `qty`, `unit_price`, `total_amount`)  
  - `stores` (`store_id`, `store_name`, `city`, `region`)  
  - `products` (`product_id`, `product_name`, `category`)  
  - `calendar` (`date`, `day_of_week`, `month`, `year`, `is_weekend`)  
- **Scope**: Daily and hourly granularity for the selected month, with historical months for MoM comparisons

**Key Features & Visuals**

- **Top KPIs**: Total Sales, Total Orders, Total Quantity (with MoM %, sparklines)  
- **Calendar Heatmap**: Monthly slicer with days colored by sales volume, plus detailed tooltips  
- **Daily Trend Chart**: Bars of daily sales with a dotted average line; color-coded above/below average  
- **Sales by Category & Top 10 Products**: Ranked bar charts with MoM change badges for insights into promotions and inventory  
- **Day × Hour Heatmap**: Hourly demand across weekdays—ideal for staffing optimization  
- **Store-level Analytics**: MoM comparisons per store to spotlight performance deviations  
- **Drill-through & Filtering**: Click to explore transactions or filter by store, product, or date

**Walkthrough Snapshot**

- **Key KPIs (Cards)**  
  - Total Sales: $99K (+29.8% vs LM)  
  - Total Orders: 21,229 (+29.8%)  
  - Total Quantity Sold: 30,406 (+29.1%)  
  - Avg Daily Sales: $3,188

- **Calendar Heatmap** – Shows daily variance in sales performance  
- **Sales: Weekday vs. Weekend** (Donut Chart):  
  - Weekday: $73K (74%)  
  - Weekend: $25K (26%)

- **Sales by Store** (Bar Chart):  
  - Hell’s Kitchen: $33.1K  
  - Lower Manhattan: $32.8K  
  - Astoria: $32.8K

- **Trend Over Time** – Daily bars vs. average line ($3,188) spotlighting any deviations  
- **Sales by Category**:  
  - Coffee: $38.3K (+30.9%)  
  - Tea: $27.9K (+28.4%)  
  - Bakery: $11.9K (–31.7%)  
  - Drinking Chocolate: $10.2K  
  - Coffee Beans: $5.2K

- **Top Products**:  
  - Barista Espresso: $13.1K (+30.4%)  
  - Brewed Chai Tea: $11.0K (+31.6%)  
  - Hot Chocolate: $10.2K (+26.1%)

- **Day × Hour Heatmap** – Highlights peak demand between 10 AM–12 PM on weekdays; reduced evening activity

**Business Impact & Insights**

- **Revenue Growth**: +29% MoM indicates strong sales strategy  
- **Staff Optimization**: Morning weekday highs guide staffing decisions  
- **Product Mix Strategy**: Coffee & tea lead revenue; bakery’s decline suggests a promotion or refresh opportunity

 **ScreenShot**
[![Dashboard Snapshot](https://raw.githubusercontent.com/rahuldhakar-tech/Coffee-shop-sales/main/Snapshot%20coffee%20sales.PNG)](https://github.com/rahuldhakar-tech/Coffee-shop-sales/blob/main/Snapshot%20coffee%20sales.PNG)

