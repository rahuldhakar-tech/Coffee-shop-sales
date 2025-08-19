Coffee Shop Sales Dashboard

An interactive Power BI report for retail sales & operations insights

Short description / purpose

The Coffee Shop Sales Dashboard provides an at-a-glance and drillable view of revenue, orders, and quantities across stores, products, days, and hours. It helps store managers and analysts identify peak times, top-selling items, and month-over-month performance so they can optimize staffing, inventory, and promotions.

Tech stack

📊 Power BI Desktop (.pbix / .pbit) — report development and visuals

🔁 Power Query (M) — data ingestion and transformation

🧠 DAX — calculated measures (KPIs, MoM % change, average daily line, conditional formatting)

🗂️ SQL (T‑SQL / .sql) — ETL / reporting views used to prepare model (see /sql/)

📁 CSV — anonymized sample data for reproducibility

🎥 Demo/Images — exported screenshots, GIF or short video for quick preview

Data source & structure

Source: Point-of-sale (POS) style sales data (anonymized for sharing).
Primary tables:

sales (order_id, store_id, product_id, order_datetime, qty, unit_price, total_amount)

stores (store_id, store_name, city, region)

products (product_id, product_name, category)

calendar (date, day_of_week, month, year, is_weekend)

Scope: Daily and hourly granularity for the selected month with historical months available for MoM comparisons.
Key features / highlights

Top KPIs: Total Sales, Total Orders, Total Quantity (with MoM % and sparkline trend).

Calendar heat map: Dynamic month slicer; days colored by sales volume; tooltips show Sales/Orders/Quantity.

Daily sales trend with average line: Bars for daily sales with dotted average line; bars above/below average visually called out.

Sales by Product Category & Top 10 Products: Ranked bars with MoM change badges to guide promotions and inventory.

Day × Hour heatmap: Visualize hourly demand across weekdays to optimize staffing.

Store-level analytics: MoM comparisons for each store to detect under/over-performance.

Drill-through & filters: Click to drill into transactions or filter across the report by store, product, or date.
Key KPIs (Top Row Cards)

Total Sales: $99K (+29.8% vs LM)

Total Orders: 21,229 (+29.8% vs LM)

Total Quantity Sold: 30,406 (+29.1% vs LM)

Avg Daily Sales: $3,188

Calendar Heatmap (Monthly View)
Interactive monthly calendar highlights daily sales, showing peak vs. low-performing days.

Sales by Weekday vs Weekend (Donut Chart)

Weekday Sales: $73K (74%)

Weekend Sales: $25K (26%)

Sales by Store Location (Bar Chart)
Compares sales performance across branches:

Hell’s Kitchen: $33.1K

Lower Manhattan: $32.8K

Astoria: $32.8K

Sales Trend Over Time (Bar + Line Chart)
Daily sales bars compared against average sales line ($3,188). Identifies days above/below benchmark.

Sales by Product Category (Bar Chart)

Coffee: $38.3K (+30.9%)

Tea: $27.9K (+28.4%)

Bakery: $11.9K (–31.7%)

Drinking Chocolate: $10.2K

Coffee Beans: $5.2K

Top Selling Products (Bar Chart)
Highlights leading items such as:

Barista Espresso: $13.1K (+30.4%)

Brewed Chai Tea: $11.0K (+31.6%)

Hot Chocolate: $10.2K (+26.1%)

Sales by Day & Hour (Heatmap)
Shows hourly sales across weekdays and weekends. Strongest demand between 10 AM–12 PM on weekdays; weaker sales in evenings.

Business Impact & Insights

Revenue Growth Monitoring: Month-over-month increases (+29%) signal effective sales strategies.

Staff Optimization: Peak weekday and morning demand guide smarter scheduling.

Product Mix Strategy: Coffee & Tea drive majority of revenue; bakery decline suggests need for promotion or menu refresh.

Store Performance Benchmarking: Location comparison reveals strong Hell’s Kitchen performance and opportunities to boost Lower Manhattan/Astoria.

Targeted Promotions: Calendar and heatmap insights allow running offers during slow days and evening hours.

