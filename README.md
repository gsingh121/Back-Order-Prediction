# Back-Order-Prediction
To build a model which will be able to predict whether an order for a given product can go on backorder or not.  A backorder is the order which could not be fulfilled by the company. Due to high demand of a product, the company was not able to keep up with the delivery of the order.

Data Description

The client will send data in multiple sets of files in batches at a given location. Data will contain 24 columns: 
sku – 		 	Random ID for the product
national_inv –   	Current inventory level for the part
lead_time – 	 	Transit time for product (if available)
in_transit_qty – 	Amount of product in transit from source
forecast_3_month – 	Forecast sales for the next 3 months
forecast_6_month – 	Forecast sales for the next 6 months
forecast_9_month – 	Forecast sales for the next 9 months
sales_1_month – 	Sales quantity for the prior 1 month time period
sales_3_month – 	Sales quantity for the prior 3 month time period
sales_6_month – 	Sales quantity for the prior 6 month time period
sales_9_month – 	Sales quantity for the prior 9 month time period
min_bank – 		Minimum recommend amount to stock
potential_issue – 	Source issue for part identified
pieces_past_due – 	Parts overdue from source
perf_6_month_avg – 	Source performance for prior 6 month period
perf_12_month_avg – 	Source performance for prior 12 month period
local_bo_qty – 		Amount of stock orders overdue
deck_risk – 		Part risk flag
oe_constraint – 	Part risk flag
ppap_risk – 		Part risk flag
stop_auto_buy – 	Part risk flag
rev_stop – 		Part risk flag
went_on_backorder – 	Product actually went on backorder. This is the target value.

Apart from training files, we also require a "schema" file from the client, which contains all the relevant information about the training files such as:
Name of the files, Length of Date value in FileName, Length of Time value in FileName, Number of Columns, Name of the Columns, and their datatype.
