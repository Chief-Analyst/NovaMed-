# NovaMed-
NovaMed Pharmaceuticals Ltd is a fictitious mid-sized pharmaceutical company operating across five regions in Nigeria. The company manufactures and distributes ten product lines spanning antibiotics, cardiovascular drugs, antidiabetics, antimalarials and several other therapeutic categories.
This project simulates a real-world data analytics engagement; from receiving raw, messy transactional data through cleaning, analysis and the delivery of actionable business intelligence via a Power BI dashboard.

  Project Objectives
•	Identify the company's best-performing products, regions and sales channels by revenue and gross profit.
•	Analyse sales trends over the two-year period and detect seasonality patterns.
•	Evaluate gross margin performance across product categories.
•	Rank sales representatives by revenue contribution.
•	Deliver a clean, interactive Power BI dashboard for management decision-making.

DATASET DESCRIPTION  
The raw dataset contained 1,550 sales transaction records covering the period January 2024 to December 2025, across 5 regions, 12 states, 10 products, 5 sales channels and 15 sales representatives.

Columns in Raw Dataset
Column	                Data Type          	                      Description
transaction_id	        String	                            Unique identifier for each transaction
date	               String (mixed format)	                 Transaction date — mixed DD/MM/YYYY and YYYY-MM-DD
product_name	        String	                              Name of pharmaceutical product sold
category	            String	                              Therapeutic category of the product
region	              String	                              Geographic region of sale
state	                String	                                State within the region
sales_rep	            String	                            Name of sales representative (40 missing)
channel	              String	                                Sales channel (30 missing)
quantity_sold	         Integer	                            Number of units sold (15 negative values)
unit_price_ngn	      Float	                                  Selling price per unit in Naira
unit_cost_ngn	        Integer	                                  Cost of goods per unit in Naira
discount_pct	        Float	                                    Discount percentage applied (27 missing)
revenue_ngn	          Float	                                    Total revenue (10 zero-value records)
cogs_ngn	            Integer	                                    Cost of goods sold
gross_profit_ngn	    Float	                                    Gross profit per transaction

DATA CLEANING 
All cleaning was performed in Python using the pandas library. Each step is documented below with the rationale and code used

KEY FINDINGS & INSIGHTS  
•	Revenue growth: Total 2025 revenue was ₦236.1M vs ₦225.6M in 2024 — a year-on-year growth of 4.7%, indicating steady upward momentum.
•	Highest margin product: PainEase 200mg at 47.4% gross margin — despite being the 10th-ranked product by revenue, its profitability per unit is the strongest in the portfolio.
•	Regional gap: The West region generates 69% more revenue than the South region despite both having similar sales team sizes. This suggests a structural or market access issue in the South.
•	Seasonality: Revenue peaks were observed in February and May — likely linked to post-New Year restocking (Feb) and pre-rainy season stockpiling (May). September through November shows consistent growth.
•	Channel opportunity: Online sales are comparable to Hospital and Clinic channels. As digital health adoption grows in Nigeria, this channel has the highest growth potential and should receive dedicated investment.
•	Distributor dependency: 25% of revenue flows through the Distributor channel which is a concentration risk. If major distributors renegotiate terms or switch to competitors, significant revenue is at risk.
•	Data integrity: 6.3% of raw records had quality issues. Investing in better CRM/ERP data entry validation at source would eliminate most of these issues upstream.



