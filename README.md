# 📊 Sales Performance Dashboard – Superstore Dataset
_Interactive Excel-based Sales Performance Dashboard that transforms 9,994 raw transactions into actionable business intelligence with dynamic slicers, KPIs, trends, and geographic insights._

---
## 📌 Table of Contents
- <a href="#overview">Overview</a>
- <a href="#business-problem">Business Problem</a>
- <a href="#dataset">Dataset</a>
- <a href="#tools--technologies">Tools & Technologies</a>
- <a href="#project-structure">Project Structure</a>
- <a href="#data-cleaning--preparation">Data Cleaning & Preparation</a>
- <a href="#exploratory-data-analysis-eda">Exploratory Data Analysis (EDA)</a>
- <a href="#research-questions--key-findings">Research Questions & Key Findings</a>
- <a href="#dashboard">Dashboard</a>
- <a href="#how-to-run-this-project">How to Run This Project</a>
- <a href="#Future Work">Future Work</a>
- <a href="#author--contact">Author & Contact</a>

---

<h2><a class="anchor" id="overview"></a>Overview</h2>

This end-to-end project delivers a fully interactive **Sales Performance Dashboard** built entirely in Microsoft Excel for the Superstore retail dataset (2014–2017). The dashboard provides a single-page view of total sales, profit, category performance, monthly trends, geographic distribution, top customers, and products — all with dynamic filtering via slicers.

Built 100% natively in Excel (no Power BI or Tableau), it demonstrates advanced PivotTables, charts, slicers, and dashboard design skills while turning static reports into self-service business intelligence.

---

<h2><a class="anchor" id="business-problem"></a>Business Problem</h2>

The fictional Superstore client relied on static Excel spreadsheets that required manual updates every month. Key business challenges included:

- No single view to track overall sales and profit performance
- Difficulty comparing category-wise and region-wise performance
- No clear visibility into monthly/yearly sales trends
- Inability to quickly identify top customers and products
- Time-consuming manual analysis and reporting

**Goal**: Build one interactive Excel dashboard that combines all critical metrics, enables dynamic filtering by year and category, and supports faster, data-driven decision-making.

---

<h2><a class="anchor" id="dataset"></a>Dataset</h2>

- **Source**: Superstore Sales Dataset (retail transactions 2014–2017)
- **Raw Data File**: `data/sales_dataset.xlsx`
- **Total Records**: 9,994 transactions
- **Key Columns**: Order ID, Order Date, Customer Name, State, Category, Sub-Category, Product Name, Sales, Profit, Quantity, Discount
- **Time Period**: 2014 to 2017 (4 years)

---

<h2><a class="anchor" id="tools--technologies"></a>Tools & Technologies</h2>

- **Primary Tool**: Microsoft Excel (Advanced PivotTables, Charts, Slicers, Conditional Formatting, Dashboard Layout)
- **Data Processing**: Excel formulas, PivotTable calculations, Power Query (import & cleaning)
- **Visualization**: Bar charts, Line charts, Pie charts, Filled Maps (heat-map style), Tables
- **Interactivity**: Slicers for Year and Category
- **Documentation**: Sales Dashboard Report.docx
- **GitHub**

No external BI tools were used — keeping the solution lightweight and fully Excel-native.

---

<h2><a class="anchor" id="project-structure"></a>Project Structure</h2>

    sales-dashboard-excel/

    ├── README.md

    ├── Sales data/
     |└── Sales Dashboard Data.xlsx

    ├── Sales report/
     |└── Sales Dashboard report.pdf

    ├── Dashboard/
     |└── Sales dashboard.png
    
    ├── Images/
     | └──  Category Sales Mix.png
     |└──  Customer Count.png
     |└──  Customer Distribution by Category.png
     |└──  Monthly Sales.png
     |└──  Profit Gained Over Time.png
     |└──  Sales and Profit Over Time by year.png
     |└──  Sales By Category.png
     |└──  Sales By State.png
     |└──  Sales vs Profit by category.png
     |└──  Top 5 customers making profit.png
     |└──  Top 10 products by Total sales.png

---


<h2><a class="anchor" id="data-cleaning--preparation"></a>Data Cleaning & Preparation</h2>

- Removed duplicates and standardized date/category formats
- Handled missing values and calculated profit margins
- Created multiple summary sheets using PivotTables:
  - Sales by Category
  - Profit over Time (by Category)
  - Monthly Sales
  - Top Customers by Profit
  - Sales by State
  - Category Sales Mix
  - Top 10 Products by Sales
- All data was validated to ensure dashboard numbers match the raw dataset exactly.

---

<h2><a class="anchor" id="exploratory-data-analysis-eda"></a>Exploratory Data Analysis (EDA)</h2>

**Key Observations:**
- Technology category showed highest sales and profit
- Negative profit values detected in several high-discount transactions
- Strong seasonal peaks in Q4 (November & December)
- High concentration of sales in California, New York, and Washington
- Customer concentration: Top 5 customers contributed significantly to profit

**Summary Statistics (from PivotTables):**
- Total Sales growth: 51% from 2014 to 2017
- Peak sales months: November, September, December
- Geographic contribution: Top 3 states ≈ 48% of revenue

---

<h2><a class="anchor" id="research-questions--key-findings"></a>Research Questions & Key Findings</h2>

1. **Category Performance** — Which category drives the most profit?  
   → Technology generated the highest sales ($836K) and profit ($145K).
2. **Year-over-Year Growth** — How has performance evolved?  
   → Sales increased 51% (2014: $484K → 2017: $733K). Profit improved 88%.
3. **Seasonality** — When do sales peak?  
   → Strong holiday effect in November, September, and December.
4. **Geographic Concentration** — Where is revenue focused?  
   → California, New York, and Washington account for nearly 48% of total revenue.
5. **Customer & Product Insights** — Who and what matter most?  
   → Top 5 customers generated over $32K in profit. Canon imageCLASS 2200 Advanced Copier was the top product ($61K).
6. **Profitability Risks** — Any red flags?  
   → Several high-discount items showed negative profit — pricing/discount strategy review recommended.

---

<h2><a class="anchor" id="dashboard"></a>Dashboard</h2>

The final deliverable is a **single-page interactive Excel dashboard** featuring:

- Sales by Category Bar Chart (Phones, Chairs, Storage leading)
- Monthly Sales Trend Line Chart
- Profit by Category & Year (stacked column)
- Sales by State (heat-map style table)
- Top 5 Customers by Profit ranking
- Category Sales Mix (pie chart)
- Top 10 Products by sales value
- **Slicers**: Year and Category (all visuals update instantly)

![Sales Dashboard](Dashboard/Sales%20Dashboard.png)

---


<h2><a class="anchor" id="how-to-run-this-project"></a>How to Run This Project</h2>

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/sales-dashboard-excel.git
   cd sales-dashboard-excel
2. Open the dashboard file:
Double-click dashboard/sales_dashboard.xlsx (or Sales Dashboard.xlsx at root)
3. Interact with the dashboard:
- Use the Year and Category slicers
- All charts and KPIs update automatically
- No installation or coding required — works in Excel 2016+
4. View the project report:
- Open Sales Dashboard Report.docx

---

<h2><a class="anchor" id="Future Work"></a>Future Work</h2>
 
- Migrate the dashboard to Power BI or Tableau for enhanced interactivity and mobile responsiveness
- Add forecasting models (using Excel’s built-in Forecast Sheet or Python integration)
- Implement drill-down functionality and more advanced KPIs (e.g., profit margin %, customer lifetime value)
- Integrate with a live database (SQL) for real-time updates
- Add what-if analysis for pricing and discount scenarios
- Create a version with Power Query automation for monthly data refresh

---

<h2><a class="anchor" id="author--contact"></a>Author & Contact</h2>

Abhisek Chandra Sen Gupta

Data Analyst

📧 Email: abhisekchandrasengupta@gmail.com

🔗 Linkedin: https://www.linkedin.com/in/abhisek-chandra-sen-gupta-573987289?utm_source=share_via&utm_content=profile&utm_medium=member_android

📍 Location: Siliguri, West Bengal, India

Feel free to connect or reach out for collaboration, feedback, or questions about the project!
 




