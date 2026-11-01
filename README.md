# Vendor Performance Analysis

**An end-to-end data analytics project analysing vendor performance, procurement efficiency, inventory turnover, brand profitability, and business insights.**

## 1. Overview

Vendor Performance Analysis evaluates vendor and brand performance using purchasing, sales, pricing, and inventory data.

The project combines Python-based exploratory data analysis, SQL queries, statistical analysis, and Power BI visualisation to identify high-performing vendors, procurement concentration, slow-moving inventory, and opportunities for cost optimization.

## 2. Key Features

- Vendor-wise and brand-wise sales performance analysis.
- Vendor contribution to total purchase dollars.
- Pareto analysis of procurement dependency.
- Bulk purchasing and unit price relationship analysis.
- Identification of vendors with low inventory turnover.
- 95% confidence interval analysis of profit margins.
- Hypothesis testing to compare vendor profitability.
- Interactive Power BI dashboard.

## 3. Business Questions

1. Which vendors and brands demonstrate the highest performance?
2. Which vendor contributes the most to total purchase dollars?
3. How much of total procurement is dependent on top vendors?
4. Does purchasing in bulk reduce unit price, and what is the optimal purchase volume for cost savings?
5. Which vendors have low inventory turnover, indicating excess stock and slow-moving products?
6. What is the 95% confidence interval for profit margins of top-performing and low-performing vendors?
7. Is there a significant difference in profit margins between top-performing and low-performing vendors?

## 4. Datasets

The datasets used in this project are available below:

1. [Purchase Prices Dataset (CSV)](https://github.com/rajkashyap03/Vendor-Performance-Dashboard/blob/main/purchase_prices.csv)
2. [Purchase Dataset (CSV)](https://github.com/rajkashyap03/Vendor-Performance-Dashboard/blob/main/purchase.csv)
3. 

## 5. Tech Stack

| Technology | Purpose |
|---|---|
| Python | Data analysis and preparation |
| Pandas & NumPy | Data manipulation |
| Matplotlib & Seaborn | Exploratory data visualisation |
| SQL | Data extraction and aggregation |
| SQLite | Database management |
| Jupyter Notebook | Analysis environment |
| Power BI | Interactive dashboard |
| DAX | Measures and calculated tables |

## 6. Installation and Setup

**Prerequisites:** Python, Jupyter Notebook, and Power BI Desktop.

### Step 1: Install dependencies

```bash
pip install pandas numpy matplotlib seaborn scipy sqlalchemy jupyter
```

### Step 2: Configure the database

Place the `inventory.db` database file inside the project's `data` directory.

```python
import sqlite3

conn = sqlite3.connect("data/inventory.db")
```

### Step 3: Run the analysis

```bash
jupyter notebook
```

Open the analysis notebook and execute the cells.

### Step 4: Open the dashboard

Open the Power BI `.pbix` report using Power BI Desktop. Refresh the database connection if required.

## 7. Key Findings and Business Insights

### 7.1 Vendor Procurement Contribution

The Pareto analysis identifies the following leading vendors:

| Vendor | Purchase Contribution |
|---|---:|
| MARTIGNETTI COMPANIES | 10.68% |
| CONSTELLATION BRANDS INC. | 9.49% |
| DIAGEO NORTH AMERICA INC. | 9.05% |
| E & J GALLO WINERY | 5.81% |
| BACARDI USA INC. | 5.06% |
| **Combined contribution** | **40.09%** |

**Business Insight:** The top five vendors account for approximately 40.09% of total procurement in the displayed analysis. This indicates supplier concentration and highlights the importance of monitoring supplier dependency, negotiating purchasing terms, and maintaining alternative sourcing options.

### 7.2 Overall Financial Performance

The Power BI dashboard displays the following KPI values:

| KPI | Dashboard Value |
|---|---:|
| Total Sales | 305.79M |
| Total Purchase | 321.90M |
| Gross Profit | 329.49K |
| Unsold Capital | 111.00M |
| Additional Sales Card | 22.43M |

**Business Insight:** The dashboard indicates substantial purchasing and sales activity, alongside significant capital represented by unsold inventory. The displayed unsold capital of 111.00M makes inventory movement and stock optimization important areas for further investigation.

*Note: The dashboard contains two sales-related cards with different values. Their underlying calculations and filter contexts should be verified before treating them as separate financial metrics.*

### 7.3 Brand Performance

The dashboard highlights the following leading brands in its sales analysis:

- Jack Daniels No. 7 Black
- Tito's Handmade Vodka
- Grey Goose Vodka
- Absolut 80 Proof
- Captain Morgan Spiced Rum

**Business Insight:** These brands are prominent in the displayed sales analysis. Their individual profitability and sales contribution should be considered together when evaluating brand performance.

### 7.4 Inventory Turnover

Vendor-level average stock turnover is used to identify potentially slow-moving inventory.

**Business Insight:** Vendors with lower stock turnover may be associated with slower inventory movement and capital tied up in stock. These vendors should be investigated further using purchase frequency, sales demand, and inventory levels.

### 7.5 Bulk Purchasing Analysis

Purchase quantity is compared against unit purchase price to investigate whether larger purchase volumes are associated with lower unit costs.

**Business Insight:** This analysis can help identify potential economies of scale and purchase-volume ranges that may improve procurement efficiency. The optimal volume should be determined from the observed price-quantity relationship rather than assumed in advance.

### 7.6 Statistical Profitability Analysis

The project evaluates profitability differences between top-performing and low-performing vendor groups using:

- 95% confidence intervals.
- Hypothesis testing.
- Statistical significance assessment.

**Business Insight:** Confidence intervals help estimate the range of plausible average profit margins, while hypothesis testing determines whether the observed difference between vendor groups is statistically significant.

*The actual confidence intervals, test statistics, p-values, and final statistical conclusions are not included because their verified numerical outputs are not yet available.*

## 8. Conclusion

The analysis highlights the importance of vendor concentration, purchasing efficiency, inventory movement, and brand profitability in business performance.

The Pareto results show that the top five vendors contribute approximately 40.09% of total procurement, demonstrating a meaningful level of supplier concentration. The Power BI dashboard also reports 111.00M in unsold capital, making inventory optimization an important area for management attention.

By combining Python, SQL, statistical analysis, and Power BI, this project demonstrates an end-to-end approach to transforming raw purchasing and sales data into meaningful business insights.

**Overall, the project provides a data-driven framework for improving procurement decisions, monitoring vendor performance, and identifying opportunities to optimize inventory and profitability.**

## 9. Future Improvements

- Automate data ingestion and dashboard refresh.
- Add monthly and quarterly performance trends.
- Develop a comprehensive vendor scoring model.
- Include supplier delivery and defect performance.
- Improve inventory forecasting and reorder recommendations.

## 10. Contributing

Suggestions and contributions are welcome. Contributions can be made through improvements to the analysis, visualisations, documentation, or project functionality.

## 11. License

No license has been specified for this project.

## 12. Author

GitHub: rajkashyap03
Email: rituraj010304@gmail.com



