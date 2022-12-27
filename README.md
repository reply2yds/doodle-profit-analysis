# Adventure Works Cycles - Profit Analysis

 
## Overview of Business Problem
**Adventure Works Cycles**, a large wholesaler of bicycles in the US and Europe, has noticed that their total profits have been declining over the last few months. The company’s IT department has provided you with the company’s sales data over the last few years.

## Assumptions:
1. The sales amount is in **USD**
2. The company bears the cost of transport. Thus, Unit_Freight_Cost adds into the overall cost of the product from the perspective of the company.
3. As all rows in *OrderDate* have data only to 01 of Month, *OrderDate* has monthly granularity i.e., it represents month and year on which the order was placed

## Data Understanding
 - The data is at purchase item level i.e., a single *SalesOrderNumber* can contains multiple *LineItem_Id*
 - Each _LineItem_Id_ represents a product sold by the company to customer. Furthermore, same products are combined to single line item if customer has ordered multiple quantities of product as part of sales.
 - *Unit_Cost* represents how much money the company spend to deliver one unit of product i.e., cost price of a single product
 - *UnitPrice* refers to how much money the company charge customers for each item sold i.e., selling price of a single product
 - *UnitPriceDiscount* indicates how much discount on the purchased product has been offfered by the Sales Rep
 - *OrderQty* shows how much quantity of the product the customer ordered
 - *Unit_Freight_Cost* determine the cost of shiping a product from warehouse to customer
 
 ## Steps
1. Create a virtual environment, named as venv.
`python3 -m venv venv`

2. Activate the created virtual environment
`source ./venv/bin/activate`

3. Install the required libraries and dependencies from requirements.txt
`pip install -r requirements.txt`

4. Run the `ProfitAnalysis.ipynb` to perfrom data analysis