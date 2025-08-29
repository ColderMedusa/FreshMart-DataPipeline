# FreshMart-DataPipeline
First ETL pipeline for the freshmart database

First create a reader for the freshmart_products_csv file to read all the data in the csv file 

After creating the reader, we first displayed the first 5 rows to make sure that the readre was working well and then after making sure that the first 5 lines, I checked for any empty lines in the database and tried to fill those in so that further data processing would not be messed up by those empty values.

I also created a new column named StockValue using the StockQuantity and Price columns to test out my data manipulation.

I aslo looked at the average prices as well as the total stock quantity

Next up was creating the cennection between PostGRESQL and python using psycopg2 as well as a few commands like the insert_data, fetch_data, create_table, create_connection and close_connection and I tested out the commands through fetching specific data such as the items in the Dairy category and the items where the stock quantity would be less than 50, displaying the results in both python as well as in PostGreSQL
