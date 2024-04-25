# Consumer Goods PowerBI Project

## Files Information :

1. PowerBI Dashboard in PDF format: [Consumer_Goods_PowerBI_Dashboard_PDF.pdf](https://github.com/surbhi66581/Consumer-Goods-PowerBI-Project/blob/382f793602c7f9ecdd3003649e083ed892ef0023/Consumer_Goods_PowerBI_Dashboard_PDF.pdf)
2. PowerBI Dashboard in PBIX format: [Consumer_Goods_PowerBI_Dashboard.pbix](https://github.com/surbhi66581/Consumer-Goods-PowerBI-Project/blob/cc887495c674e41ea4798f7458d043590ed81eae/Consumer_Goods_PowerBI_Dashboard.pbix)
3. Consumer Insight Presentation: [Consumer_Goods_Presentation.pdf](https://github.com/surbhi66581/Consumer-Goods-PowerBI-Project/blob/382f793602c7f9ecdd3003649e083ed892ef0023/Consumer_Goods_Presentation.pdf)
4. SQL Queries used for BI: [BI_SQL_Queries.txt](https://github.com/surbhi66581/Consumer-Goods-PowerBI-Project/blob/cc887495c674e41ea4798f7458d043590ed81eae/BI_SQL_Queries.txt)


## Challenge: Data-Driven Decisions for a Consumer Goods Leader
A leading consumer goods company struggles to translate data into actionable insights. Their current approach hinders strategic decision-making, making it difficult to react quickly to market trends.


## Solution: Business Intelligence with Power BI
By implementing a Business Intelligence (BI) solution built on Microsoft Power BI, we can empower this company to unlock the potential of their data. Power BI will provide them with the tools to:

Gain Insights: Analyze trends, identify customer preferences, and understand product performance.

Visualize Data: Create interactive dashboards and reports for clear and concise communication of findings.

Drive Actionable Decisions: Equip leadership with the data-driven insights they need to make informed strategic choices.

This BI solution will transform the way the company uses data, enabling them to make faster, more effective decisions and gain a competitive edge in the consumer goods market.


## Metadata

I have used a database that includes information from six main tables:

1. dim_customer: contains customer-related data
2. dim_product: contains product-related data
3. fact_gross_price: contains gross price information for each product
4. fact_manufacturing_cost: contains the cost incurred in the production of each product
5. fact_pre_invoice_deductions: contains pre-invoice deductions information for each product
6. fact_sales_monthly: contains monthly sales data for each product.



Column Description for dim_customer table:

1. customer_code: The 'customer_code' column features unique identification codes for every customer in the dataset. These codes can be used to track a customer's sales 		history, demographic information, and other relevant details. For example, the codes could look like '70002017', '90005160', and '80007195' respectively.

2. customer: The 'customer' column lists the names of customers, for example 'Atliq Exclusive', 'Flipkart', and 'Surface Stores' etc.

3. platform: The 'platform' column identifies the means by which a company's products or services are sold. "Brick & Mortar" represents the physical store/location, and 			"E-Commerce" represents online platforms.

4. channel: The 'channel' column reflects the distribution methods used to sell a product. These methods include "Retailers", "Direct", and "Distributors". Retailers 				refer to physical or online stores that sell products to consumers. Direct sales refer to sales made directly to consumers through a company's website or other direct means, and distributors refer to intermediaries or middlemen between the manufacturer and retailer or end consumers.

5. market: The 'market' column lists the countries in which the customer is located.

6. region: The 'region' column categorizes countries according to their geographic location, including "APAC" (Asia Pacific), "EU" (Europe), "NA" (North America), and 			    "LATAM" (Latin America).

7. sub_zone: "The 'sub_zone' column further breaks down the regions into sub-regions, such as "India", "ROA" (Rest of Asia), "ANZ" (Australia and New Zealand), "SE" 				  Southeast Asia), "NE" (Northeast Asia), "NA" (North America), and "LATAM" (Latin America)."




Column Description for dim_product table:

1. product_code: The 'product_code' column features unique identification codes for each product, serving as a means to track and distinguish individual products within a 		database or system.

2. division: The 'division' column categorizes products into groups such as "P & A" (Peripherals and Accessories), "N & S" (Network and Storage) and "PC" (Personal 				 Computer).

3. segment: The 'segment' column categorizes products further within the division, such as "Peripherals" (keyboard, mouse, monitor, etc.), "Accessories" (cases, cooling 			solutions, power supplies), "Notebook" (laptops), "Desktop" (desktops, all-in-one PCs, etc), "Storage" (hard disks, SSDs, external storage), and "Networking" (routers, switches, modems, etc.).

4. category: The 'category' column classifies products into specific subcategories within the segment.

5. product: The 'product' column lists the names of individual products, corresponding to the unique identification codes found in the 'product_code' column.

6. variant: The "variant" column classifies products according to their features, prices, and other characteristics. The column includes variants such as "Standard", 				"Plus", "Premium" that represent different versions of the same product.



Column Description for fact_gross_price table:

1. product_code: The 'product_code' column features unique identification codes for each product.

2. fiscal_year: The 'fiscal_year' column contains the fiscal period in which the product sale was recorded. A fiscal year is a 12-month period that is used for accounting 			purposes and often differs from the calendar year. For Atliq Hardware, the fiscal year starts in September. The data available in this column covers the 				fiscal years 2020 and 2021.

3. gross_price: The 'gross_price' column holds the initial price of a product, prior to any reductions or taxes. It is the original selling price of the product.


Column Description for fact_manufacturing_cost:
1. product_code: The 'product_code' column features unique identification codes for each product

2. cost_year: The "cost_year" column contains the fiscal year in which the product was manufactured.

3. manufacturing_cost: The "manufacturing_cost" column contains the total cost incurred for the production of a product. This cost includes direct costs like
raw materials, labor, and overhead expenses that are directly associated with the production process.


Column Description for fact_pre_invoice_deductions:

1. customer_code: The 'customer_code' column features unique identification codes for every customer in the dataset. These codes can be used to track a customer's sales history, demographic information, and other relevant details. For example, the codes could look like '70002017', '90005160', and '80007195' respectively.

2. fiscal_year: The "fiscal_year" column holds the fiscal period when the sale of a product occurred.

3. pre_invoice_discount_pct: The "pre_invoice_discount_pct" column contains the percentage of pre-invoice deductions for each product. Pre-invoice deductions are 
discounts that are applied to the gross price of a product before the invoice is generated, and typically applied to large orders or long-term contracts.

Column Description for fact_sales_monthly:

1. date: The "date" column contains the date when the sale of a product was made, in a monthly format for 2020 and 2021 fiscal years. This information can be used
to understand the sales performance of products over time.

2. product_code: The "product_code" column contains a unique identification code for each product. This code is used to track and differentiate individual 
products within a database or system.

3. customer_code: The 'customer_code' column features unique identification codes for every customer in the dataset. These codes can be used to track a customer's sales 			history, demographic information, and other relevant details. For example, the codes could look like '70002017', '90005160', and '80007195' respectively.

4. sold_quantity: The "sold_quantity" column contains the number of units of a product that were sold. This information can be used to understand the sales volume ofproducts and to compare the sales volume of different products or variants.

5. fiscal_year: The "fiscal_year" column holds the fiscal period when the sale of a product occurred.
   

