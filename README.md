# Build-a-Dynamic-5-Year-Financial-Model-in-Excel-with-Scenario-Analysis
 how to build a dynamic 5-year financial model for an e-commerce business using Excel. We’ll walk through revenue forecasting, cost assumptions, income statement creation, and a powerful scenario analysis feature all within one interactive Excel model.

Step 1: Set Up Revenue Assumptions

➤ Assumptions to Forecast Revenue
Define:

Number of Orders (starting point: e.g., 3,000)

Average Order Value (fixed across 5 years: e.g., $39.95)

Growth Rates by year (e.g., 100%, 75%, 50%, 35%)


➤ Formula:
Use a compound growth formula: = Previous Year Orders * (1 + Growth Rate)


➤ Calculate Revenue: = Number of Orders * Average Order Value

Step 2: Estimate Fixed and Variable Expenses
➤ Variable Costs (per order):
Manufacturing (e.g., $6.50 per order)

Fulfillment (e.g., $2.50 per order)

Optionally, reduce per-unit costs over time to simulate economies of scale.

➤ Fixed Costs:
Warehouse Rent

Salaries

Marketing

Other (e.g., legal, accounting)

These are usually constant but can be scaled as business grows.


Step 3: Build the Income Statement
➤ Sections:
Revenue (calculated earlier)

Cost of Goods Sold (COGS): = Orders * Manufacturing Cost + Orders * Fulfillment Cost

Gross Profit: = Revenue - COGS

Operating Expenses (sum of fixed costs)

Operating Profit: = Gross Profit - Operating Expenses

Tax: = IF(Operating Profit < 0, "N/A", Operating Profit * Tax Rate)
Net Profit: = IFERROR(Operating Profit - Tax, Operating Profit)

 4: Add Scenario Analysis with a Toggle
➤ Create 3 Sets of Assumptions:
Live Case

Scenario 1 (Optimistic)

Scenario 2 (Pessimistic)

Each should have different values for:

Orders

Growth

Order Value

Manufacturing Cost

Tax Rate

➤ Use CHOOSE Formula: = CHOOSE(ScenarioCell, Scenario1Value, Scenario2Value)
This allows switching assumptions dynamically.

➤ Add Data Validation:
Limit the input cell to only 1 or 2:

Go to Data > Data Validation > List > Enter 1,2


Step 5: Test and Use the Model
Now try toggling the scenario between 1 and 2. Watch how the financials change dynamically—this helps decision-makers simulate real-world outcomes with a single click.


Conclusion
You've now created a professional, dynamic Excel-based financial model in under an hour. This skill is crucial whether you're launching a startup, pitching to investors, or building financial acumen.

