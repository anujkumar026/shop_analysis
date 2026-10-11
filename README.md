
# SmartShop Analytics Dashboard

An interactive **Power BI** dashboard that tracks sales, stock, profit and customer payment behaviour for a retail shop. It helps a shop owner see what sells, when it sells, and how customers pay, all on one page.

![SmartShop Analytics Dashboard](images/dashboard.png)

## Project Objective

Turn raw shop transaction data into a clear, filterable report that answers:

- How much are we selling, and is it rising or falling month to month?
- Which products and categories drive the most revenue?
- How do customers pay (cash vs online)?
- Which sales channel (direct, online, wholesale) performs best?
- What is the overall profit and profit margin?

## Key Metrics (KPIs)

| Metric | Value |
|---|---|
| Total Sales | 367K |
| Stock (units/items) | 132 |
| Profit | 8,703 |
| Profit % | 3% |

## Dashboard Features

- **Slicers / filters:** Year, Month, Sale Type (Direct Sales / Online / Wholesaler), Payment Mode (Cash / Online)
- **Sales by Months:** monthly sales with profit overlay
- **Daily Sale:** day-wise sales trend to spot peaks and dips
- **Payment Mode:** cash vs online split (donut chart)
- **Sale Type:** share of direct, online and wholesale sales (donut chart)
- **Sales by Product:** top products by revenue (bar chart)
- **Sales by Category:** category contribution (treemap)

## Key Insights

- **Monthly sales trend downward** across the period shown, from about 39K in the highest month to about 25K in the lowest.
- **Top categories:** Personal Care (86K), Household (85K) and Beverages (85K) are close to each other, followed by Grocery (63K) and Furnishing.
- **Top products:** Plastic Mat (22K) and Carpet Roll (21K) lead, followed by Rubber Mat and Silk Fabric (19K each).
- **Payment mode is split almost evenly** between online and cash.
- **Direct sales are the largest channel**, followed by online, with wholesale the smallest share.
- **Profit margin is thin (about 3%)**, which suggests a review of pricing and costs would help.

## Tools & Skills Used

- **Power BI Desktop**
- **Power Query** for data cleaning and transformation
- **Data modeling** (`MasterData` table)
- **DAX** for measures (total sales, profit, profit %)
- Visuals: cards, slicers, column/bar charts, line/area chart, donut charts, treemap

## Project Structure

```
SmartShop-Analytics/
├── SmartShop_Analytics.pbix    # Power BI dashboard file
├── data/
│   └── SmartShop_Data.xlsx     # Source dataset
├── images/
│   └── dashboard.png           # Dashboard screenshot
└── README.md
```

## How to Use

1. Download or clone this repository.
2. Open `SmartShop_Analytics.pbix` in **Power BI Desktop**.
3. If prompted, point the data source to `data/SmartShop_Data.xlsx` (Home → Transform data → Data source settings).
4. Use the slicers (Year, Month, Sale Type, Payment Mode) to explore the data.

## Data Preparation (summary)

- Removed duplicates and fixed data types
- Handled missing / inconsistent values
- Built a master table combining product, category, sale type and payment details
- Created calculated measures for sales, profit and profit %

## Author

**Anuj Kumar**
BCA, Swami Vivekanand Subharti University
[LinkedIn](https://linkedin.com/in/anuj-kumar-ssm) | Instagram: [@data.analysis2026](https://instagram.com/data.analysis2026)

If you found this project useful, feel free to star the repo.
