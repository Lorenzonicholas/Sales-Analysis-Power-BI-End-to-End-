## DAX Code Used

% Weekend Transactions = DIVIDE([Weekend Transactions],[Total Transaction])

60-Day Revenue = CALCULATE([Total Revenue], DATESINPERIOD('Calendar'[date],MAX('Calendar'[date]),-60,DAY))

All Returns = CALCULATE([Total Returns],ALL(Return_Data))

```DAX
Total Revenue =
SUMX(Transaction_Data, Transaction_Data[quantity] * RELATED(Products[product_retail_price])




