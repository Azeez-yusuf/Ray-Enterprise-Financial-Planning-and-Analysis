# Ray-Enterprise-Financial-Planning-and-Analysis
A Deep Dive into detailed Business Intelligence of Financial Health of Ray Enterprise and its Future Projection
Ray Enterprise: A small scaled business investment, where i worked as an outsourced Business Intelligence Officer

## Project Overview
This Project is for didactic purpose to give comprehensive detail of my new role to aspiring friends, classmates and former workplace colleagues as requested, as it aim Exploration of the Financial Health Analysis of Ray Enterprise and Future Projection

## The Raw Data
The Data source was prepared by the Data Entry Clarks in the respective branches. Although, all Drivers remain untampered, all key values have been altered by Me for Privacy purposes. This data only ivolve components of Income Statement

## Data Preparation
Various additions and multiplications were done to arrive at individual basic components of the Income Statement which span through 2021 to 2025, and also are divided into Quarters

### Tool Used
•	EXCEL; Used for:
1. Data loading and inspection
2. Data manipulations
3. Handling missing values,
4. Cleaning and
5. Formatting
6. Analysis
7. Visualization


### Challenges Encountered include
1. Minor improper casing of alphabets: Code used is; =Proper()
2. A lttle of misspellings
3. Duplicate Entry 
3. values errors, nulls and missing values were observed in the raw dataset.

### Profferred Solution:
1. One on One Conversation with the Data Entry Clark, and Other personnel to confirm missing values
2. Various Senior senior colleagues were also contacted at my Primary place of work, for review and constructive critisms
3. I use MS EXCEL to perform data manipulations, transformations, cleaning and formatting


## STEPS INVOLVED IN THE EXCEL ANALYSIS
### STEPS OVERVIEW
A.	We collect the actuals expenses of each department
B.  Financial Health Analysis of Ray Enterprise Income Statement
C.	We forecast the future months using excel forecasting tool
D.	We create different scenarios: Best case, Worst Case and Base Case
E.	Profit and Loss Statement to see the forecast affects our profitability 

### STEP A: INCOME STATEMENT SHEET
1. Consolidation of quarterly expenses and income, to regularize with income Statement Format such as;
   i.  Revenue from Sales
   ii. Cost of Goods From direct expenses
   iii. Selling, General, and Administrative Expenses; viz salaries, sales commisions, travel expenses, rents, insurance, etc.
   iv. And many others  

2. Normal Balancing of Income Statement

### STEP B: FINANCIAL HEALTH ANALYSIS SHEET
1.	Organic growth was calculated: = current year minus previous year /current year * 100
2.	Gross Profit Margin Stability:  = Gross Profit/Revenue
3.	Operating Income Growth: = current year minus previous year /current year * 100
4.  Net Income Trend= current year minus previous year /current year * 100

### STEP C: OPEN ANOTHER SHEET AND FORECAST SHEET
1.	Move to the Forecast sheet
2.	Bring all the expenses in the IS Sheet to Forecast sheet as Actual, and duplicate it 3 times, labelled them, Live Case, Scenario 2 as Base Case, Scenario 1 as Worse, and Scenario 3 as Best 
3.	Do (2) to base, worst, and best case
4.	Use the Edate formula to project 12 months  on base, best, and worst case
5.	For base case : Use forecast ets to make forecast, Because this formula take into first the latest data. E.g  =FORECAST.ETS(I$14,$E15:H15,$E$14:H$14)
6.	For best case: first base case forecast cell, use the for: =the cell *(1-30% cell[ lock with f4 absolute reference)
7.	For worse case: first base case forecast cell, use the for: =the cell *(1+30% cell[ lock with f4 absolute reference)
	
STEP C
1.	Move to the Income Statement
2.	Join the expenses in Forecast to that of income statement using unique formula
3.	We link the date too
4.	Move back to forecast to recreate another case called Live Case, just copy  one the case and paste directly, it doesn’t matter. Then rename to  Live Case, Do (2)
5.	We use the formula =CHOOSE('Income Statement'!$C$2,Forecast!I18,Forecast!I29,Forecast!I40), to connect our scenario using operating scenario in income statement. Please Note; C2 is the Scenario Case
6.	Link the forecast figures in Forecast to  IS Forecast
7.	Then we sum to get the total operating expense

   
STEP D: Moving to IS Forecast
1.	Our assumptions include; Customers Acquisition Cost, Price, COGS % of Revenue, Interest Expense Net % of COGS, Interest Income Net % of Revenue, Other Non -Operating Income Expenses, Net % of COGS
2.	Customers Acquisition Cost: We started with 600, along the way business technique got better, the cost decline, to 500
3.	Our Selling Price: Price of our good increase probably due to inflation and some other factors, from 2400 to 3500
4.	I imagined 35%, which is below the 50% Good Status Threshold, Universally

STEP E: Still on IS Forecast
1.	 We calculate Unit sold by =   Selling and Marketing Expenses / Price
2.	Revenue = Unit Sold *price
3.	COGS = COGS % of Revenue * Revenue
4.	Interest Expense = COGS * Interest Expense Net % of COGS
5.	Interest Income = Revenue * Interest Income Net % of Revenue
6.	Other Non -Operating Income Expenses = COGS * Other Non -Operating Income Expenses, Net % of COGS
7.	Point to Note: If you are successfully following the analysis, you would notice that in the Forecast IS, some of our Pre-Tax Income is negative. I mean, there is no point paying Tax when your Pre-Tax Income is negative (i.e you suffered loss). So we use an IF Statement  to wrap the formula. =IF(E29>0,E29*E62,0)
8.	In STEP C section 5; C2 which is the Scenario Case, I added data validation. The steps includes; click on cell c2  Alt A V V  List  since our scenario is 3, I typed (1,2,3) in the list  Error Msg [Input Error Check the List]

NOTE:  Different companies has different ways/approach in the use of different drivers and assumptions


## Financial Health Insights from Quarterly Income Statements
#### 1.	Organic Growth and Organic Growth % : 
a.	Period of extreme Volatility: The company has experienced highly volatile organic growth over the past several years, oscillating between significant positive growth and substantial declines. While there was a strong recovery in Q3 2023, the subsequent quarters (Q4 2023 to Q2 2025) have shown a concerning return to negative growth, with the most recent quarter (Q2 2025) at -5%. This indicates a lack of consistent, sustainable organic growth and suggests underlying challenges in the business model or market conditions

Implication and Recommendation: This volatility makes forecasting extremely difficult and suggests that the company's revenue streams are either highly susceptible to external factors, or there are significant internal operational inefficiencies or one-off events distorting the true underlying performance
		
b.	Period of Strong Decline (Q2 2022 and Q3 2022): The company experienced a sharp decline in organic growth from Q2 2022 to Q3 2022, with values of −26,910.0 (-10%) and −112,570.0 (-71%) respectively.

Implication and Recommendation: This period likely indicates a significant business challenge, such as a loss of key customers, a major market downturn, increased competition, or issues with product/service offerings

c.	Brief Recovery and Peak (Q1 2023 - Q3 2023): Following the steep decline, there was a period of recovery culminating in a remarkable 73% growth in Q3 2023 (540,500.0).

Insight: This suggests that the company was able to address some of its previous issues or capitalize on a specific market opportunity. However, given the subsequent performance, this peak appears to be an outlier rather than a sustainable trend. It's crucial to understand what drove this spike (e.g., a large one-time contract, a successful product launch, or a favorable market condition that has since changed)
d.	Concerning Return to Negative Growth (Q4 2023 - Q2 2025): Post Q3 2023, the organic growth has largely turned negative or remained low, culminating in another significant decline of -305% in Q4 2024 and continuing with -11% in Q1 2025 and -5% in Q2 2025

Insight: This trend is highly concerning. It suggests that the factors driving the Q3 2023 peak were not sustainable, and the company is reverting to a pattern of decline. The -305% in Q4 2024 is particularly alarming and requires immediate deep dive.
Further Analysis is required to answer the following Question: Was this a massive contract cancellation, a significant write-off, or an accounting adjustment.
#### 2.	Consistently High Gross Profit Margins (Excluding Anomaly): Apart from the anomalous Q3 2021 (62%), the Gross Profit Margin (Gross Profit / Total Revenue) generally remains robust, often above 90% (e.g., 92% in Q4 2021, 94% in Q1 2022, 93% in Q2 2022, and so on). This indicates strong pricing power or efficient cost of revenue management during most periods, suggesting a high-margin business model.
#### 3.	Operating Income Growth and Net Income growth and their respective Percentage trend: 
The company's operating income and net income trends mirror each other almost perfectly, exhibiting extreme volatility with significant swings between strong positive growth and substantial declines. While there was a remarkable rebound in Q3 2023, the subsequent quarters (Q4 2023 to Q2 2025) indicate a worrying return to negative growth, with Q2 2025 showing -9% for both metrics. The absolute alignment of operating and net income suggests either a very stable non-operating income/expense profile or, more likely, a direct correlation where core operating performance heavily dictates the bottom line. This volatility signals underlying instability in the business model or external market factors

a.	Minimal Impact of Non-Operating Items: This strong correlation suggests that the company's financial health is almost entirely dependent on its core operations. Any issues at the operating level directly translate to the net income.

b.	Extreme Volatility in Profitability: As observed from +72% (Q3 2023) to -327% (Q4 2024), and periods of strong growth immediately followed by sharp declines

Deduction: This high volatility indicates a significant lack of predictability and stability in the company's profitability. It makes financial planning, budgeting, and valuation incredibly challenging. It also raises questions about the sustainability of any positive growth periods. Further In-depth analysis is recommended

c.	Periods of Significant Decline: Q2 2022 and Q3 2022, Both operating and net income experienced sharp declines of -11% and -76% respectively. This suggests a period of significant operational distress, possibly due to declining sales and costs.
And Q3 2024, A catastrophic decline of -327% in both operating and net income (absolute values of 551,424.0 and 413,180.25 respectively). This is an alarmingly large negative figure and percentage

Deduction: This demonstrates the company's capacity to rebound. However, given the subsequent performance, this recovery appears to be an anomaly or driven by non-recurring factors rather than a sustainable change in performance. It's crucial to understand the drivers of this rebound

d.	Negative Trend (Q4 2023 - Q2 2025): Post the Q3 2023, which is the peak, profitability has largely returned to negative or low single-digit growth, culminating in -9% for both metrics in Q2 2025. This shows a clear lack of sustained positive momentum.

Deduction: The company is struggling to maintain consistent profitability. The recent negative trend indicates that the issues causing volatility are persistent or have re-emerged



## Questions for Further Investigation
•	What are the absolute revenue figures that correspond to these income numbers? Understanding the base revenue is crucial to assess the scale and impact of these fluctuations.
•	What caused the catastrophic -327% decline in Q4 2024? This is the most critical question. Was it a specific event, a change in accounting policy, or a fundamental deterioration of the business?
•	What factors drove the significant recovery in Q3 2023? Were these sustainable drivers or one-time events?
•	Breakdown of Operating Expenses: What are the major components of operating expenses (e.g., Cost of Goods Sold, SG&A, R&D)? How have these changed relative to revenue during periods of high and low profitability?
•	Is there any seasonality in the business that explains some of the volatility?
•	What is the company's capital structure and interest expense profile? This would help confirm why net income tracks operating income so closely.
•	What is the tax rate applied to net income? Are there any deferred tax assets/liabilities or unusual tax events impacting the net income trend?
•	What are the company's strategies for cost control and revenue generation to stabilize profitability?

## Recommendations
1.	Immediate Deep Dive into Q4 2024: Prioritize understanding the exact reasons for the -327% decline. This is likely an extraordinary event that needs to be fully understood to assess future risk.
2.	Focus on Profitability Stabilization: The company needs to implement strategies to reduce income volatility. This could involve: 
 o	Re-evaluating pricing strategies and cost structures.
 o	Diversifying customer base or product lines to reduce dependence on a few large contracts.
 o	Improving operational efficiency and expense management.
3.	Enhance Financial Planning & Forecasting: Develop more robust models that account for significant swings and incorporate scenario analysis to better prepare for potential downturns.
4.	Strategic Review: Conduct a comprehensive strategic review of the business model to identify systemic issues contributing to volatility and to develop a path towards more consistent and sustainable profitability.


   
