# 📊 Company Financials Performance Dashboard

A Power BI dashboard project showcasing detailed analysis and KPIs based on a global financial dataset. The data includes sales, profit, cost, discount, and segment details by region and time.

---

## 📅 Dataset Overview

**Filename:** `Company Financials Dataset`  
**Source:** Provided internally (simulated company data)  
**Rows:** ~7,000 records  
**Fields:**
- `Date`
- `Segment`
- `Country`
- `Product`
- `Units Sold`
- `Manufacturing Price`
- `Sale Price`
- `Gross Sales`
- `Discounts`
- `Sales`
- `COGS`
- `Profit`

---

## ✅ Objective

To design an interactive Power BI dashboard that provides actionable business insights through:
- Executive KPIs
- Segment analysis
- Regional performance
- Time-based sales & profit trends

---

## 💰 Key Performance Indicators (KPIs)

| KPI                        | Description                                                  | Formula                                          |
|---------------------------|--------------------------------------------------------------|--------------------------------------------------|
| Total Sales               | Total revenue generated from all transactions               | `SUM(Sales)`                                     |
| Total Profit              | Total earnings after COGS and discounts                     | `SUM(Profit)`                                    |
| Profit Margin (%)         | % of profit retained from revenue                           | `(Total Profit / Total Sales) * 100`             |
| Units Sold                | Total quantity of products sold                             | `SUM(Units Sold)`                                |
| Discount Impact           | Total value of discounts offered                            | `SUM(Discounts)`                                 |
| Cost of Goods Sold (COGS) | Production and delivery costs of the sold units             | `SUM(COGS)`                                      |
| Top 5 Countries by Sales  | Regions generating the most revenue                         | `TOPN(5, SUM(Sales) BY Country)`                 |
| Top 5 Countries by Profit | Regions contributing most to profit                         | `TOPN(5, SUM(Profit) BY Country)`                |
| Monthly Sales Trend       | Line graph showing monthly sales over time                  | `Sales by Month`                                 |
| Sales vs. Profit by Segment| Compare revenue and margin across market segments           | `Bar/Column Chart`                               |

---

## 📈 Visualizations in Power BI

| Section                  | Visual Type        | Description                                                  |
|--------------------------|--------------------|--------------------------------------------------------------|
| Header                   | Text Box           | Dashboard title + refresh date                               |
| Executive KPIs           | Cards              | Total Sales, Profit, Margin, Units Sold, Discounts, COGS     |
| Regional Performance     | Filled Map         | Sales by Country/Region                                      |
| Segment Breakdown        | Stacked Column     | Sales vs. Profit by Segment                                  |
| Monthly Trends           | Line Chart         | Sales & Profit by Month                                      |
| Top Countries            | Bar Charts         | Top 5 by Sales / Profit                                      |
| Filters/Slicers          | Slicers            | Segment, Country, Date Range                                 |

---

## 🧰 Tools Used

- **Excel**: For initial data exploration, data cleaning, and formatting  
- **Power BI**: For building interactive dashboards, creating DAX measures, and designing visuals

---

## ⚖️ Data Cleaning & Preparation

Performed in Excel prior to loading into Power BI:
- Removed currency symbols (`$`), commas (`,`), and dashes (`-`)
- Converted numerical columns from string to `float`
- Parsed `Date` column to datetime format
- Created `Profit Margin` as a new calculated field

---

## 🚀 How to Use

1. Clone the repository
2. Open `Company Financials Dataset` in Power BI
3. Open the provided `Company Financials Dataset.pbix` file
4. Adjust slicers to explore trends and insights

---

## 📚 Use Cases

- Executive reporting
- Market segment performance
- Business planning and forecasting
- Monthly/Quarterly business reviews

---

## ✍️ Author

**Gabriel Makinde**  
Business & Data Analyst  
[LinkedIn Profile](https://linkedin.com/in/gabrielmakinde)  
Email: gabrielmakinde@gmail.com

---

## 🌐 License

This project is licensed under the MIT License. Feel free to fork, customize, and use it for learning or business analysis.
