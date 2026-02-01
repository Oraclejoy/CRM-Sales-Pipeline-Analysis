1. Introduction
This report presents an in-depth analysis of a CRM sales opportunities dataset from a fictitious B2B company specializing in computer hardware sales. The dataset captures the end-to-end sales pipeline, including accounts, products, sales teams, regions, sectors, deal stages, engagement dates, close dates, and deal values.
The objective of this analysis is to evaluate sales performance, efficiency, and trends across sales agents, managers, products, accounts, regions, office locations, and sectors. The insights generated aim to support data-driven decision-making, improve sales effectiveness, and enhance future revenue forecasting.

2. Dataset Overview
The dataset is structured into multiple interconnected tables representing key business dimensions:
•	Accounts – Company-level details such as sector, location, and account performance.
•	Products – Product names, product series, and pricing.
•	Sales Teams – Sales agents, managers, and office locations.
•	Sales Pipeline – Individual sales opportunities, including deal stage, engagement date, close date, and deal value.
The sales pipeline follows a standard B2B lifecycle:
Prospecting → Engaging → Closed (Won or Lost)

3. Data Preparation & Cleaning
To ensure analytical accuracy and reliability, the following steps were taken:
3.1 Header Standardization
Across all sheets, the first row was converted into column headers to enable consistent referencing, relationship modeling, and accurate calculations.

3.2 Handling Missing Values
In the Sales Pipeline table, missing values were observed in:
•	Account
•	Close Date
•	Close Value
These records were not deleted because:
•	They belonged to Prospecting or Engaging deal stages.
•	Missing close dates and values are expected for open deals.
Actions taken:
•	Open deals were retained for pipeline visibility and forecasting.
•	Revenue, win rate, and sales cycle metrics were calculated only for closed deals.
This approach preserved data completeness while preventing distorted performance metrics.

3.3 Derived Columns
Several calculated fields were added:
a) Won Deal Flag
•	1 = Closed Won
•	0 = Closed Lost or Open
b) Win Rate
Calculated using:
SUM(Deal Won) / COUNT(Opportunity ID)
c) Sales Cycle Duration
Sales Cycle (Days) = Close Date – Engage Date
Applied only to closed deals.

3.4 Data Relationships
Relationships were established between:
•	Sales Pipeline ↔ Accounts
•	Sales Pipeline ↔ Products
•	Sales Pipeline ↔ Sales Teams
This enabled multi-dimensional analysis without duplication.
 

3.5 Data Validation
•	Revenue calculations restricted to Closed Won deals.
•	Pipeline analysis included open deals.
•	All calculated metrics were validated using pivot tables.
 

4. Sales Performance Analysis
 
Key Findings
•	Total Revenue: $10,005,534
•	Won Deals: 4238
•	Average Sales Cycle: 48 days
•	Top Sales Agent: Darcel Schlecht ($1,153,214)
•	Lowest Sales Agent: Violet McClelland ($123,431)
•	Top Manager: Melvin Marxen

Problems Identified
1.	Uneven agent performance – Large revenue gaps indicate skill, territory, or opportunity imbalance.
2.	Moderate-to-long sales cycle – 48 days may slow revenue realization.
3.	Revenue concentration risk – Heavy reliance on a few top performers.

Recommendations
•	Replicate top-agent best practices through mentoring and coaching.
•	Provide targeted training for underperforming agents.
•	Improve deal qualification to shorten sales cycles.
•	Leverage high-performing managers for performance reviews and pipeline oversight.
________________________________________
Future Outlook
•	Balanced agent performance will increase total revenue.
•	Reduced sales cycles will accelerate deal closures.
•	Stronger pipeline management will improve forecast accuracy.

4.	Product Performance Analysis
 
Key Metrics Used
•	Total Revenue
•	Average Deal Value
•	Number of Won Deals

Key Findings
•	GTX Plus Pro is the top-performing product with $2,629,651 in revenue.
•	MG Special is the lowest-performing product.
•	The GTX Series generates the highest overall revenue.
•	June recorded the highest monthly revenue.

Insights
•	Lower prices do not guarantee higher revenue.
•	High-priced products like GTX Plus Pro still perform exceptionally well.
•	Null revenue values for GTX Plus Pro reflect open pipeline deals, not poor performance.
Problems Identified
•	Heavy reliance on the GTX product line.
•	Weak contribution from underperforming products.
•	Risk of pipeline deals not converting into revenue.

Recommendations
•	Prioritize high-value GTX Plus Pro opportunities.
•	Reevaluate pricing and positioning of low-performing products.
•	Maintain value-based pricing strategies.
•	Use weighted pipeline forecasting for better accuracy.

Future Outlook
•	Strong pipeline for GTX Plus Pro signals future revenue growth.
•	Product diversification can reduce dependency risk.
•	Improved conversion rates will stabilize revenue streams.

6. Account Performance Analysis
 
Key Findings
•	Top Account: Kan-code ($341,455), followed by Konex and Condax.
•	East Region has the highest win rate.
•	High deal volume does not equal high revenue:
o	Hottechi recorded many deals but did not rank among top revenue accounts.

Sector & Location Insights
•	Retail sector generated the highest revenue, making it the most profitable customer segment.
•	United States recorded the highest revenue by office location.
•	Romania generated the lowest revenue.

Business Implications
•	Revenue dependency on a few key accounts increases risk.
•	Sales effort may be misallocated to low-value, high-activity accounts.
•	High-performing regions and sectors reveal replicable success strategies.

Recommendations
•	Prioritize strategic, high-value accounts with dedicated relationship management.
•	Reassess high-activity but low-revenue accounts.
•	Replicate East region sales strategies across other regions.
•	Increase focus on the Retail sector through targeted campaigns and tailored solutions.

Future Outlook
By shifting focus from deal quantity to deal quality, strengthening high-performing sectors and regions, and optimizing account strategies, the company can achieve sustainable growth, higher revenue efficiency, and reduced dependency risks.


