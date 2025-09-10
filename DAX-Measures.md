## DAX Code Used

```DAX
% Weekend Transactions = DIVIDE([Weekend Transactions],[Total Transaction])

60-Day Revenue = CALCULATE([Total Revenue], DATESINPERIOD('Calendar'[date],MAX('Calendar'[date]),-60,DAY))

All Returns = CALCULATE([Total Returns],ALL(Return_Data))

All Transactions = CALCULATE([Total Transaction],ALL(Transaction_Data))

Last Month Profit = CALCULATE([Total Profit] , DATEADD('Calendar'[date], -1 ,MONTH))

Last Month Returns = CALCULATE([Total Returns], DATEADD('Calendar'[date],-1,MONTH))

Last Month Revenue = CALCULATE([Total Revenue] , DATEADD('Calendar'[date],-1,MONTH))

Last Month Transactions = CALCULATE([Total Transaction],DATEADD('Calendar'[date],-1,MONTH))

Price Margin = SUM('Products'[product_retail_price]) - SUM('Products'[product_cost])

Profit Margin = (DIVIDE([Total Profit],[Total Revenue]))

Quantity Returned = SUM(Return_Data[quantity])

Quantity Sold = SUM(Transaction_Data[quantity])

Return Rate = DIVIDE(SUM(Return_Data[quantity]) , SUM(Transaction_Data[quantity]))

Revenue Target = [Last Month Revenue] * 1.05

Revenue vs Profit Share Gap (pp) = [Total Revenue % by Brand] - [Total Profit % By Brand]

Total Cost = SUMX(Transaction_Data, (Transaction_Data[quantity] * RELATED(Products[product_cost])))

Total Customers = COUNT(Customers[customer_id]) 

Total Profit = [Total Revenue] - [Total Cost]

Total Profit % By Brand = DIVIDE([Total Profit],CALCULATE([Total Profit],all(Products[product_brand])))

Total Returns = COUNTA(Return_Data[quantity])

Total Revenue = SUMX(Transaction_Data,(Transaction_Data[quantity]*RELATED(Products[product_retail_price])))

Total Revenue % by Brand = DIVIDE([Total Revenue],CALCULATE([Total Revenue],ALL(Products[product_brand])))

Total Transaction = COUNTA(Transaction_Data[quantity]) 

Transaction Target = [Last Month Transactions]*1.05

Unique Products = DISTINCTCOUNT(Products[product_name])

Weekend Transactions = CALCULATE([Total Transaction], 'Calendar'[Weekend] = "Y")

YTD Revenue = CALCULATE([Total Revenue],DATESYTD('Calendar'[date]))
















