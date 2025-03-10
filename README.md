# POWER-BI-PROJECTS
# Measure Table used created
Under it using DAX We created Quantity sold, Sum of Net Sales, Total Profit

Quantity Sold = CALCULATE(SUM('Fact Table'[Units Sold]),all('Date Table 1'),USERELATIONSHIP('Date Table 2'[Date],'Fact Table'[Date (dd/mm/yyyy)]))

Sum of Net Sales = CALCULATE(SUM('Fact Table'[Net Sales  ]),all('Date Table 1'),USERELATIONSHIP('Date Table 2'[Date],'Fact Table'[Date (dd/mm/yyyy)]))

Total Profit = CALCULATE(SUM('Fact Table'[Profit]),ALL('Date Table 1'),USERELATIONSHIP('Date Table 2'[Date],'Fact Table'[Date (dd/mm/yyyy)]))

#These measures are built using DAX functions such as CALCULATE, SUM, USERELATIONSHIP, and ALL to customize the calculations based on specific relationships and filters, helping you analyze data with time-based granularity and specific filters in Power BI.
