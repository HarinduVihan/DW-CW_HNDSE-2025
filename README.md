**Students Details   ![](Aspose.Words.fe96fbbb-d53f-436d-9d51-dc3e5de24310.001.png)![](Aspose.Words.fe96fbbb-d53f-436d-9d51-dc3e5de24310.002.png)![](Aspose.Words.fe96fbbb-d53f-436d-9d51-dc3e5de24310.003.png)**

**Module Name:**  Software Engineering  **Module Lecturer/** 

l.S. Chathurika **Course Coordinator:** 

**Department:**  School of Computing **Submission Due on:**  13th July ,2025 

**Type of Coursework:**  Report 

**Title of the Coursework:**  Data Warehouse and Business Intelligence 

1 

***Students Details: ![](Aspose.Words.fe96fbbb-d53f-436d-9d51-dc3e5de24310.004.png)***

**Student No.** 

01  COHNDSE24.2F - 026 

02  COHNDSE24.2F - 005 03  COHNDSE24.2F - 040 04  COHNDSE24.2F - 008 05  COHNDSE24.2F - 085 

**Student Name** P H N Sethulya 

M K D Gangadara ![](Aspose.Words.fe96fbbb-d53f-436d-9d51-dc3e5de24310.005.png)

W A U S Weerasooriya A H V M Jayaratine 

P K P C P Kapuge 


|**Office use only:** |
| - |
|***Date Stamp Required of the Department***|

**Table of Contents** 

[**Chapter 1: Introduction** 	 4 ](#_page3_x69.00_y72.00)

1. [**Overview of the Business** 	 4 ](#_page3_x69.00_y98.00)
1. [**Importance of  having Data Warehousing and BI in Retails** 	 4 ](#_page3_x69.00_y363.00)
1. [**Project Goal** 	 5 ](#_page4_x69.00_y72.00)
1. [**Tools and Technologies**	 5 ](#_page4_x69.00_y265.00)

[**Chapter 2: Data Sources** 	 6 ](#_page5_x69.00_y72.00)

1. [**CSV Files** 	 6 ](#_page5_x69.00_y220.00)
1. [**SQL Files** 	 7 ](#_page6_x69.00_y72.00)
1. [**JSON Files** 	 7 ](#_page6_x69.00_y372.00)
1. [**Sample Tables and Screenshots** 	 7 ](#_page6_x69.00_y528.00)

[**Chapter 3: Data Warehouse Design** 	 9 ](#_page8_x69.00_y72.00)

1. [**Facts and Dimensions Tables** 	 9 ](#_page8_x69.00_y98.00)
1. [**Galaxy Schema** 	 10 ](#_page9_x69.00_y72.00)

[**Chapter 4: ETL Process** 	 11 ](#_page10_x69.00_y72.00)

1. [**Data Extraction** 	 11 ](#_page10_x69.00_y98.00)
1. [**Data Transformation** 	 11 ](#_page10_x69.00_y434.00)
1. [**Data Loading** 	 12 ](#_page11_x69.00_y174.00)
1. [**ETL Sample Workflows** 	 12 ](#_page11_x69.00_y321.00)

[**Chapter 5: Data Visualization** 	 15 ](#_page14_x69.00_y72.00)

1. [**Connection between the Data Warehouse & Power BI** 	 15 ](#_page14_x69.00_y98.00)
1. [**Dashboard Design** 	 15 ](#_page14_x69.00_y303.00)

[**Chapter 6: Analysis & Insights** 	 18 ](#_page17_x69.00_y72.00)

[**Chapter 7: Conclusion**	 18 ](#_page17_x69.00_y391.00)

**Roles and Contributions** 



|**Index No** |**Contribution** |
| - | - |
|**COHNDSE24.2F – 005** |<p>- Found Data sources and gathered Data, suitable for the business. ![](Aspose.Words.fe96fbbb-d53f-436d-9d51-dc3e5de24310.006.png)</p><p>- Using Apache Hop, extracted data and added validations, transformed data </p>|
|**COHNDSE24.2F – 008** |<p>- Found Data sources and gathered Data, suitable for the business. </p><p>- Designed the Galaxy Schema,  </p><p>- Load data to Power bi and Transform data  and Add connections </p>|
|**COHNDSE24.2F – 026** |<p>- Created the report and presentation </p><p>- Design Power BI Dashboards ![](Aspose.Words.fe96fbbb-d53f-436d-9d51-dc3e5de24310.007.png)</p><p>- Identifying Business Problems in the domain and Solutions using the Data (Dashboard) </p>|
|**COHNDSE24.2F – 040** |<p>- Found Data sources and gathered Data, suitable for the business. </p><p>- Designed the Galaxy Schema,  </p><p>- Using Apache Hop, extracted data and added validations, transformed data. </p><p>- Data warehouse implementation.  </p>|
|**COHNDSE24.2F – 085** |<p>￿  Using Talend, did the ETL transformation and loaded </p><p>data. </p>|

<a name="_page3_x69.00_y72.00"></a>**Chapter 1: Introduction** 

1. **Overview<a name="_page3_x69.00_y98.00"></a> of the Business**  

E - commerce products are amongst the most dynamic product categories in the modern retail business  due  to  the  high  consumer  demand  and  rapid  development  of  technology. A  retail establishment that sells electrical products, such as televisions, refrigerators, washing machines, mobile devices, and related accessories, is the business domain that we have selected. Customers from all around the world purchase these goods, which are available for purchase both online and in store. 

The business generates massive amounts of data every day, including customer information, product  details,  reviews,  ratings,  and  sales  transactions.  With  careful  analysis,  this  data's informative  information  can  help  guide  strategic  decisions  regarding  product  performance, inventory management, marketing, and customer targeting. 

2. **Importance<a name="_page3_x69.00_y363.00"></a> of  having Data Warehousing and BI in Retails** 

Business intelligence (BI) and data warehousing (DW) are important for turning operational data into insights that can be used in the retail industry. Data from multiple sources are collected, transformed, and stored in a structured format for analysis and reporting in a data warehouse, that acts as a central repository. 

DW and BI allow electrical retail shops to: 

- Analysis of sales trends by product, area, or time 
- Monitoring consumer behavior for tailored advertising 
- Analyzing product performance with sales and review data 
- Forecasting inventory and demand 

Retailers may improve decision-making and performance by visualizing these insights through interactive dashboards and reports using BI. 

3. **Project<a name="_page4_x69.00_y72.00"></a> Goal**  

This project’s objective is to use industry level tools and techniques to build and implement a working data warehousing solution. 

- Collecting data from multiple sources (CSV files, Excel, SQL, JSON) 
- Designing a Galaxy Schema with fact and dimension tables 
- Implementing ETL processes using Talend to extract, transform, and load data into the data warehouse 
- Creating a Power BI dashboard for visualizing business insights and trends. 
4. **Tools<a name="_page4_x69.00_y265.00"></a> and Technologies**  
- MySQL - For creating and managing the data warehouse schema (database structure and queries) 
- Apache Hop & Talend Open Studio - For performing ETL operations (data extraction, transformation, and loading) 
- Microsoft Power BI - For data visualization, dashboard creation, and insight analysis 
- Excel / SQL / JSON / CSV files - Used as source data formats for products, customers, reviews, and sales 

<a name="_page5_x69.00_y72.00"></a>**Chapter 2: Data Sources** 

We are using three types of data sources to get data for this data warehouse . The three types of data are:  

- CSV Files 
- Json Files 
- SQL Files 
1. **CSV<a name="_page5_x69.00_y220.00"></a> Files** 

The data that was taken from CSV Files 



|**File Name** |**Description** |**Key Fields Included** |
| - | - | - |
|**Customers.csv** |Customer data with IDs and demographics |CustomerID, First Name, Last Name, City, Country, Phone, Email |
|**Geography.csv** |Location info for customers and stores |GeographyID, Country, City, Postal Code |
|**Product. Csv** |Product master list |ProductID, Name, Category, Price, Discounts, Decriptions, Images|
|**Rating. Csv** |Customer product ratings |RatingID, ProductID, CustomerID, RatingValue, RatingCount |
|**Shipping Carrier. csv** |Shipping service providers |CarrierID, CarrierName, Hotline, Website, Email |

2. **SQL<a name="_page6_x69.00_y72.00"></a> Files** 

The following are the SQL Data Sources that we gathered  



|**File Name** |**Description** |**Key Fields Included** |
| - | - | - |
|**Inventory.sql** |Stock levels for products in warehouses |InventoryID, ProductID, StockLevel, LastUpdateDate |
|**Sales.sql** |Transaction-level sales data |OrderID, ProductID, CustomerID, Quantity, Price, Date, BillAmount |
|**Shipping data.sql** |Shipment records |ShipmentID, ShippingCost, Quantit |
|**Supplier data.sql** |Supplier information |SupplierID, Name, Address, City, PostalCode, Email, Phone |

3. **JSON<a name="_page6_x69.00_y372.00"></a> Files** 

The JSON formatted data we gathered 



|**File Name** |**Description** |**Key Fields Included** |
| - | - | - |
|**Reviews.json** |Product reviews by customers |ReviewID, ProductID, CustomerID, ReviewContent, ReviewTitle |

4. **Sample<a name="_page6_x69.00_y528.00"></a> Tables and Screenshots** 

Customer Data 

![](Aspose.Words.fe96fbbb-d53f-436d-9d51-dc3e5de24310.008.png)

Geography Data  

![](Aspose.Words.fe96fbbb-d53f-436d-9d51-dc3e5de24310.009.png)

Product Data 

![](Aspose.Words.fe96fbbb-d53f-436d-9d51-dc3e5de24310.010.png)

Rating Data 

![](Aspose.Words.fe96fbbb-d53f-436d-9d51-dc3e5de24310.011.png)

Shipping Carrier Data 

![](Aspose.Words.fe96fbbb-d53f-436d-9d51-dc3e5de24310.012.png)

Review Data 

![](Aspose.Words.fe96fbbb-d53f-436d-9d51-dc3e5de24310.013.png)

<a name="_page8_x69.00_y72.00"></a>**Chapter 3: Data Warehouse Design** 

1. **Facts<a name="_page8_x69.00_y98.00"></a> and Dimensions Tables** 

The data warehouse is designed using a Galaxy Schema that includes multiple fact tables and shared dimension tables. 

**Fact Tables** 

- **Sales Fact** – Stores information about customer purchases, including quantity sold and total amount. 
- **Rating Fact** – Records customer ratings for products along with the date and review link. 
- **Inventory Fact** – Tracks product stock movement (in/out) and current stock levels over time. 
- **Shipping Fact** – Contains shipment details such as delivery status, shipping date, and associated customer/product. 

**Dimensions Table** 

- **Customer  Dimension**  –  Contains  customer  profile  data  such  as  name,  contact  info, address, and city.** 
- **Product Dimension** – Includes product attributes like name, category, pricing, discounts, and descriptions.** 
- **Date Dimension** – Stores time-related attributes like day, month, year, quarter, weekday, and weekend flag.** 
- **Review Dimension** – Contains the title and content of customer reviews linked to ratings and products.** 
- **Supplier Dimension** – Includes supplier details such as name, contact, and geographical location.** 
- **Geography Dimension** – Captures geographic data such as city, state/province, region, and country for location-based analysis. 
- **Shipping Carrier Dimension** – Contains information about third-party shipping services used for delivering products. 
2. **Galaxy<a name="_page9_x69.00_y72.00"></a> Schema** 

![](Aspose.Words.fe96fbbb-d53f-436d-9d51-dc3e5de24310.014.jpeg)

<a name="_page10_x69.00_y72.00"></a>**Chapter 4: ETL Process** 

1. **Data<a name="_page10_x69.00_y98.00"></a> Extraction** 

For the ETL process, we used Talaend Open Studio, an open-source data integration tool. **Tools & Components** 

- File Input - To extract data from CSV and SQL sources (e.g., customer, product, review datasets). 
- Table Input - Used to extract data from existing relational databases. 
- Data Grid - Used to create sample static data for testing small segments (e.g., date\_dim values). 

**Data Sources** 

- CSV Files – customer.csv, product.cs 
- SQL Files – sales.sql 
- Json Files – review.json 
- Oracle Database: Used for storing the final data warehouse schema 
2. **Data<a name="_page10_x69.00_y434.00"></a> Transformation** 

**Cleaning & Formatting** 

- Handled null values with default values. 
- Corrected data types (e.g., converting string dates to date format). 
- Formatted dates to match the warehouse schema using Talend’s date functions. 

**Business Rules** 

- Discounted Price calculation using Calculator or Modified JavaScript Value transform. 
- Customer Full Name applied using String Operations or Modified JavaScript Value step. 

**Extra Logic** 

- Duplicate removal with Unique Rows step 
- Column renaming using Select Values 
- Trimming whitespace 
3. **Data<a name="_page11_x69.00_y174.00"></a> Loading** 

After data transformation, data will be loaded to MySQL datawarehouse.  

- First, the Dimension tables will load 
- Then the Fact tables will be loaded. 

Reason: Integrating by loading referenced data first into the data warehouse. 

4. **ETL<a name="_page11_x69.00_y321.00"></a> Sample Workflows**  

Reviews Data 

![](Aspose.Words.fe96fbbb-d53f-436d-9d51-dc3e5de24310.015.png)

Customer Data 

![](Aspose.Words.fe96fbbb-d53f-436d-9d51-dc3e5de24310.016.png)

Date Data 

![](Aspose.Words.fe96fbbb-d53f-436d-9d51-dc3e5de24310.017.png)

Geography Data 

![](Aspose.Words.fe96fbbb-d53f-436d-9d51-dc3e5de24310.018.png)

Product Data 

![](Aspose.Words.fe96fbbb-d53f-436d-9d51-dc3e5de24310.019.png)

Shipping Carrier Data 

![](Aspose.Words.fe96fbbb-d53f-436d-9d51-dc3e5de24310.020.png)

Sales Data 

![](Aspose.Words.fe96fbbb-d53f-436d-9d51-dc3e5de24310.021.png)

Ratings Data 

![](Aspose.Words.fe96fbbb-d53f-436d-9d51-dc3e5de24310.022.png)

Supplier Data 

![](Aspose.Words.fe96fbbb-d53f-436d-9d51-dc3e5de24310.023.png)

Inventory Data 

![](Aspose.Words.fe96fbbb-d53f-436d-9d51-dc3e5de24310.024.png)

Shipping Data 

![](Aspose.Words.fe96fbbb-d53f-436d-9d51-dc3e5de24310.025.png)

<a name="_page14_x69.00_y72.00"></a>**Chapter 5: Data Visualization** 

1. **Connection<a name="_page14_x69.00_y98.00"></a> between the Data Warehouse & Power BI**  

We used Power BI to vosialize the data to get analysis, therefore, we connected it to the MySQL data warehouse that we created for the e-commerce retail company.  

- First, the data source selection was done, and the database credentials were added to congifured with read access. 
- The necessary facts and dimensions tables were connected.  
- In the data model view, we mapped the relationship between the tables based on foreign keys. 
2. **Dashboard<a name="_page14_x69.00_y303.00"></a> Design**  

The following is our Power BI dashboard 

1. Homepage 

![](Aspose.Words.fe96fbbb-d53f-436d-9d51-dc3e5de24310.026.jpeg)

2. Sales Performance & Profitability Overview  

![](Aspose.Words.fe96fbbb-d53f-436d-9d51-dc3e5de24310.027.jpeg)

3. Customer & Discount Insights 

![](Aspose.Words.fe96fbbb-d53f-436d-9d51-dc3e5de24310.028.jpeg)

4. Operational & Seasonal Insights 

![](Aspose.Words.fe96fbbb-d53f-436d-9d51-dc3e5de24310.029.jpeg)

<a name="_page17_x69.00_y72.00"></a>**Chapter 6: Analysis & Insights** 

This chapter represents the main insights discovered by the dashboard.  

- Able to figure out top selling and lowest sales products  
- Helps managements to focus on restocking based on the customer demand, manage pricing and promotions.  
- Find which regions have more demand 
- Helps with target marketing, according to lowest sales regions and improve rest and have more strategies.  
- Comparison between sales and customer ratings 
- High ratings might lead to better performance but may not as well. Analytics will help to figure pros and cons.  
- Uncovering top performing products, categories and vice versa, identifying profit margins and support better pricing. 

<a name="_page17_x69.00_y391.00"></a>**Chapter 7: Conclusion**  

The design and construction of a data warehouse for an e-commerce company, a growing retailer of electrical items, is well demonstrated by this project. By merging data from multiple sources, including Excel spreadsheets, SQL dump files, and a JSON document, we were able to mimic real corporate data infrastructures.  

The ETL procedure, which included extracting, cleaning, transforming, and loading the data into a structured Galaxy Schema, was carried out using Talend Open Studio. This schema architecture allowed for the effective organization of many fact tables, such as sales, inventory, and shipping, by  utilizing  shared  dimension  tables  for  customers,  goods,  location,  and  time. We were able to overcome obstacles including inconsistent data formats, missing values, and the difficulty of schema mapping by using appropriate. 
18 
