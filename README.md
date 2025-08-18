### Adventure Works Analysis

### Project Overview

This data analysis project aims to evaluate AdventureWorks’ performance from 2005 to 2008. The study will assess overall profitability, analyze profit distribution across various countries, and identify the most profitable products during this period. Additionally, it will provide insights into customer profiles, enabling AdventureWorks to better understand its customer base and tailor its strategies more effectively.

### Data Source
AdventureWorks Data: The primary dataset used for this analysis is the "AdventureWorks.xlsx: file. It contains detailed order information, product information, territory information, date information, customer information, geography information.

### Tools Used
Excel
Power Query(Data Cleaning and Preparation)
Pivot Tables(Charts, Measures)
Data model(Data modelling and creating relationships)
Simple Macro/VBA

### Data model
<img width="1655" height="759" alt="image" src="https://github.com/user-attachments/assets/6aae04e4-58e7-4740-a27b-8b5e35c3bb92" />

### Data Cleaning and Preparation
1. Data Loading and Inspection
2. Check for row duplicates
3. Replace "NA" for colours to "Unspecified"
4. Create New Columns to assist with Analysis:
- Full Name (Merging columns)
- Age
- Age Group (Conditional Column)
- Total Revenue
- Costs Of Goods Sold
- Total Profit
5. Added a measures table to group all the measures


### Some Measures Used
Average Customer Age =AVERAGE(DimCustomer[Customer Age])
Number_Of_Transaction =COUNTROWS(FactInternetSales)
Sold Products =DISTINCTCOUNT(FactInternetSales[ProductKey])
Unsold Products =[All Products]-[Sold Products]
% Profit Margin =DIVIDE([Sum of Total Profit],[Sum of Total Revenue],0)

### Key Takeaways
1. 67.1% of profit came from 2007($42.55 Million) and 2008($42.16 Million).

2. Although the percentage growth across all measures—Quantity, Cost of Goods Sold, Total Revenue, Total Profit, and Profit Margin—from 2005 to 2006 is the highest among all years, this growth should be interpreted with caution. The 2005 data only starts from July, whereas data for subsequent years covers the full calendar year starting in January. Therefore, using the growth from 2005 to 2006 as a comparative benchmark may be misleading due to the partial data in 2005. Otherwise, the largest growth in these measures happens from 2006 to 2007.
   
3. Profit is the greatest in 2007 but the profit drop in 2008. In both years the Cost Of Goods and Total Revenue made are relatively similar.

4.  In general, weekdays make up 72.0% of the total profit. Wednesday, Thursday, and Friday contribute to 43.8% of the total profit.
   
5. In general, profit is the highest during the second quarter, accounting for 31% of total profits throughout the years
  
6. The profit made in the United States is the greatest, making AdventureWorks a profit of $40.54 Million and contributing to 62.7% of the profit from 2005 to 2008.

7. The top 5 profitable products account for 24.8% of total profit.

8. The top 5 customers contribute to 0.3% of total profit.

9. There are 448 unsold products out of 606 available products

10. The profit made by female and male customers are relatively similar.
    
11.  The average customer age is 45 and the 50+ age group contributes 49.2% of the total profit.

### Summary
There is a significant portion of unsold products as compared to sold products. Therefore, AdventureWorks should re-evaluate the unsold products and remove those that are not making much profit. 

AdventureWorks can also take into consideration the top 5 most popular products and sell products similar to the top 5 products.

Since almost half of their profits are from 50+ age group, AdventureWorks should cater more towards these customers.

To continue growing its profits, AdventureWorks should try to lower its cost of goods and increase its sales by promoting products that are more favoured by its customers.
