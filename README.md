# Market Basket Analysis

## Description

Instacart is a grocery delivery and pick-up service that is available in the United States of America and Canada. The company's services can be accessed through a website and a mobile application. The data was collected anonymously and contained a sample of over 3 million grocery orders from over 200,000 Instacart consumers.

The company also provides the week, hour, and day of the order, as well as the time interval between orders to their customers. The tables, are included in this dataset, and a description of each row is provided below:

Dataset description:

Orders CSV: Consists of 3-4 million rows
Products CSV: 50 thousand rows
Aisles CSV: 134 rows
Departments CSV: 21 rows
order_products__SET: 30 million rows where SET is defined as:
order_products _prior csv: 3-2 million previous orders
order_products_train csv: 3-2 million order information

Data can be found at https://www.kaggle.com/c/instacart-market-basket-analysis/data.

### Objective:

To analyze company data in order to assist businesses in identifying the day when the most orders were placed in order to provide deals for that day
To determine which department is responsible for the most product launches
Steps to be performed:

Step 1: Upload the “insta-cart” file to the HDFS

1.1 Download the relevant dataset from the "Course Resources" section or the project description
1.2 Upload the dataset to the “FTP” lab from your local system
1.3 To move the dataset to “HDFS” from the “Webconsole” use the put command

Step 2: Perform the below tasks on the uploaded dataset using PySpark:

Login to the Pyspark shell
Explore the orders CSV file and create a DataFrame
Read the orders data as a DataFrame in PySpark
                  Note: The column “days_since_prior_order” may contain NULL values

Display the data up to 10 rows
 

Replace all null values with a dummy “999“ value in the DataFrame that was created in task 1
Examine the orders CSV file and find the busiest day of the week by reading the data as a PySpark DataFrame
Hint:The column “order_dow” represents the day of the week   

Wherein:

Day 0 is Sunday

Day 6 is Saturday, and so on

Display the result that contains the total orders placed on each day of the week (Monday to Sunday)
Example:

Total Orders	Day of the Week
600905	Sunday
587578	Monday
Give a breakdown of orders by the hour and identify the busiest hour
Select the number of order IDs as “Total_Orders” and the hour at which the order was placed
Display the result that contains total orders and the hour
