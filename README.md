# KPI-For-Superstore
Basic Sales Summary
•	Overview
This project contains a processed, dynamic sales dashboard constructed using a global corporate transactions ledger. The workspace uses analytical cards and an integrated Pivot Table breakdown to provide structural transparency into localized sales parameters, transaction volumes, and average pricing variables.
Workbook Architecture
The workspace consists of a dual-layered reporting design structured as follows:
•	Summary Sheet (Active View): A clean, dashboard reporting interface stripped of default background gridlines. It presents executive KPI blocks alongside a localized regional distribution grid.
•	Sales Data (Data Tier): The underlying master transaction log housing multi-row item entries
•	Identified Key Performance Indicators (KPIs)
The dashboard isolates four primary tracking metrics styled inside distinct visual cards:
•	TOTAL SALES: $ 12,642,501.91
Calculates cumulative baseline revenue across all recorded entries.
•	AVERAGE SALES: $ 246.49
Calculates the mean gross revenue value generated per individual transaction line-item.
•	TRANSACTION COUNT: $ 51,290.00 (Note: Currently formatted as currency)
Counts the total volume of discrete product sales line-items processed.
•	Order Count: $ 51,291.00 (Note: Currently formatted as currency)
Monitors distinct tracking tags using target index values.
•	Regional Pivot Breakdown Matrix
The workspace contains an embedded regional operational table breaking down metrics across 22 unique geographic territories (e.g., Canada, Caribbean, Central America, Central Asia, Eastern Africa, etc.) displaying the following matrix columns:
1.	Row Labels: Lists unique geographical regions parsed out from the core dataset.
2.	Total Revenue: Tracks localized aggregate sales totals matching the core $12,642,501.91 Grand Total.
3.	Count of Order ID: Measures discrete identifier values per territory (Grand Total: 51,290).
4.	Count of Sales: Aggregates processed inventory records per territory (Grand Total: 51,290).

•	Formulas & Logical Configurations
To reproduce or scale this dashboard framework, ensure the following syntax parameters are mapped to your Sales Data ledger:
•	Total Sales Card Formula:
=SUM('Sales Data'!S:S)
•	Average Sales Card Formula:
=AVERAGE('Sales Data'!S:S)
•	Transaction Volume Card Formula:
=COUNT('Sales Data'!S:S)
•	Regional Summation Pivot Logic:
=SUMIF('Sales Data'!M:M, [RegionCell], 'Sales Data'!S:S)


