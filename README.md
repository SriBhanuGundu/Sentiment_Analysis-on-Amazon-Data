# Sentiment_Analysis-on-Amazon-Data
Analyzing Customer satisfaction, opinion and expectations on products

## Project Overview
In this project, we use Sentimental Analysis to predict whether a review is 'Positive,' 'Neutral,' or 'Negative' based on reviews on a million goods from Amazon's products, Amazon sentiment dataset and Amazon Electronics datasets.

To better understand the Amazon data, we analysed 3 datasets -

Amazon 2022 products
Amazon Electronics Products
Amazon Sentiment Dataset
Intially we are starting with Amazon products dataset and we used tools like MongoDB to store the data into 3 different databases. We are accessing the data with the help of SparkSQl into the Spark dataframe using pyspark on the jupyter notebook.

The first dataset - Amazon Product Dataset has products like Toys, Vehicles, Jewellery etc. We have performed the Extract, Transform and Loading operations on this dataset and made the data feasible for Exploratory Data Analysis. After further analysis and cleaning, storing the data into the .csv file using the pandas library.

### Source of Dataset
https://www.kaggle.com/nguyenngocphung/10000-amazon-products-dataset
https://data.world/datafiniti/amazon-and-best-buy-electronics
https://www.kaggle.com/datasets/bittlingmayer/amazonreviews

## Problem Statement
Amazon Reviews will be misleading as the content may be subjective(positive or negative) and sometimes may lack the information. Finding out whether the review is positive, negative or neutral is a critical task.

## Bigdata Tools
We have used the following bigdata tools:

MongoDB
Apache Spark
QlikSense
Tableau
Anaconda Navigator

### Steps to run the file
We have 2 files to run -

With a sentiment dataset and word cloud visualizations - This can be executed as normal .ipynb file named "Data603_Final_Project_Amazon_Data_Gundu_Kavali_wordclouds.ipynb"
Second file is required to have MongoDb connection as the data is retrieved from MongoDb in the notebook. This notebook will also need Apache Spark as it is coded in Apache Spark named "Data603_Final_Project_Amazon_Data_Gundu_Kavali.ipynb"
Initially with csv file "Amazon_Products.csv", create database: "AmazonReviews" with Collection: "Products" 
later, through code, cleaned dataset with columns with proper datatypes for modeling is created then stored in database with csv file "Amazon_2022.csv"(which is created in the path in which this jupyter notebook is running.
Later, with this file database is created in mongo db with database: "Amazon_2022" and collection: "Review_ml", as it is created twice becasue most of the data needs ETL operations on columns as it contained several special characters which are not feasible for working on ml models.
with csv file "DatafinitiElectronicsProductData.csv", third database is created, in which database: "Amazon_2018" and collection: "reviews".
Later csv files "DatafinitiElectronicsProductData.csv" , "Amazon_Products.csv" and "test.csv" ("train.csv") stored in the path as per the code.

## Conclusion:
Obtained Customer opinions on several products and we detected sentiment for various reviews by the customers and made it feasible for both customers and retailers for their benefits.
