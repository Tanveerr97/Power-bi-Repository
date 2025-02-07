*Power BI Report Summary* -Sales Analysis
This Power BI report is designed to track and analyze sales data for the project across different metrics, including Revenue, Profit, Country, Reason, and Sales Year. The goal is to provide a clear, interactive, and insightful view of the project's performance over time.

* summarized description of the data columns:-
Sales Year: The year when the sale occurred.
Revenue: The total sales income from all sources (e.g., merchandise, albums, concert tickets).
Country: The country where the sale took place.
Reason: The cause of the sale (e.g., album release, concert, merchandise sale).
Profit: The net profit after deducting the costs from the revenue.
Item Type: The category of the sold item (e.g., product, album, ticket).
Order Priority: The urgency or importance of the order (e.g., High, Low, Medium).
Order Date: The date when the order was placed.
Shipment Date: The date when the item was shipped to the customer.

*Key Metrics Summary:-
Revenue: Total sales generated from all sources.
Profit: Net profit after deducting costs from total revenue.
Country: Sales performance by different countries.
Top 5 Item Types: The five most sold or profitable items.
Country-wise Item Priority: Distribution of item priority across countries.

*Key DAX Measures:-
The report uses DAX (Data Analysis Expressions) to calculate key performance metrics:
Total Revenue = SUM(Sales[Revenue])
Total Profit = SUM(Sales[Profit])
Profit Margin = DIVIDE(SUM(Sales[Profit]), SUM(Sales[Revenue]), 0)
Column formula:
MONTH = '1000000 Sales Records'[Order Date].[Month]
YEAR = '1000000 Sales Records'[Order Date].[YEAR]

*Visualizations:-
donut chart showing the sum of total revenue by item type
matrix table that shows the sum of total revenue and total profit by month
 a stacked bar chart showing the top 5 items based on either total revenue or total profit
matrix table where the rows represent items (such as item types), and the columns represent months (showing total Revenue and Profit for each item type by month)
total revenue by country using Azure Maps
line chart that shows two lines: Total Revenue and Total Cost by Month
Decomposition Tree show Item-wise Order Priority
Interactivity and Filters: filters (slicers) by Month, Year, Item Type, Region, and Country

*Formatting and Customization:-
To improve clarity and readability
Conditional Formatting is applied to Profit Margin and Revenue to highlight positive and negative trends.
Titles, Labels, and Tooltips are added to every visual to ensure that all data points are easy to interpret.
Colors are customized to differentiate between Revenue and Profit and to highlight key data.

<!-- Uploading "Sales report.pdf"... -->
