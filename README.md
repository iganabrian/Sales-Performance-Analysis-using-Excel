# Sales Performance Analysis using Excel

I recreated a sales Performance Dashboard by Freedom Oboh on Youtube. 

## Key features I used:

-Pivot Tables & Pivot charts

-Slicers & Filters

-Current Time and Date Function

-Text Function to extract month and year

Interactive Dashboard with Navigation links to calculation, dataset and back to the dashboard

## Data Dictionary 

- Order ID – The uniques No. of every transaction 

- Date - The date in which a product was purchased 

- Product - The name of the product bought 

- Category - The group under which a product falls into

- Region - The region where a product was sold 

- Sale - The selling price 

- Quantity - The number of items sold/bought under the order ID

- Cost 

## Data Cleaning and Preparation
- I created a copy of the provided sales dataset to maintaing the original dataset and work on my own data.

- I tuned the dataset into a table by pressing **CTRL + T**. After which I went removed duplicate data under the Data Tab-I pickked the product column.

- The data did not need much cleaning and was ready for enrichment. 

## Data Enrichment
I created the following additional columns using the text function:

-Month column 

-Year column 

```excel
=TEXT([@Date],"yyyy")
```

<img src="./Text function.jpg" alt="Text Function">

## Key Performace Indicators and Pivot Tables
I created pivot to analise data based on 

- Total sales

- Quantity

- Cost

- Profit using calculated filed (Total sales - Cost)

- Year on Year Sales (YoY) using If function:
```excel 
=IF(F13>=0,"▲","▼")&TEXT(ABS(F13),"0%")& "VS LY"
```

- Sales trend quaterly

- Regional Sales Distribution

- Product-wise Sales Breakdown 

- Montly Revenue Trend 2023 Vs 2024

Below is an snipset of the pivot tables in a separet sheet. 

<img src="./Pivot tables.png">

## Dashboard Design

Below is the final Sales Dasboard.  

<img src="./Sales-Dashboard.png">

## Final Remark
This project was a refresher for me in using the if function, text, dashboard design and creating navigation links in excel. 





