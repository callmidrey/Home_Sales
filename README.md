# Home_Sales
This is my module 22 Challnge

# Overview
This project analyzes home sales data to gain insights into the real estate market. The dataset used in this analysis contains information about various aspects of home sales, including sale prices, location, size, and other relevant attributes.

# Dataset
The dataset used in this project is sourced from "https://2u-data-curriculum-team.s3.amazonaws.com/dataviz-classroom/v1.2/22-big-data/home_sales_revised.csv", and it comprises a number of  observations and 11 features. Below are the key features included in the dataset:

    id - refers to the uniqe identity number of the property
    date - refers to the date property was put up for sale
    date_built - refers to the date the property was built
    price - refers to the Sale price
    bedrooms - refers to the number of bedrooms
    bathrooms - refers to the number of bathrooms
    sqft_living - refers to the living area/size (square footage) on the property  
    sqft_lot - refers to the actual property size (square footage) 
    floors - refers to the number of floors in the properties 
    waterfront - refers to if the property os located at a waterfront or not
    view - number of views the property has


# Analysis
The analysis performed on the home sales data includes the following steps and techniques:

Data Cleaning and Preprocessing: 
    This dataset was pretty descent and clean. It needed no cleaning as it was already clean and ready for analytical use.

Exploratory Data Analysis (EDA)
    This was the mail objective of this challenge to finnd the following:
    - the average price for a four bedroom house sold in each year rounded to two decimal places
![Alt text](<Screenshot 2024-02-02 111403.png>)

    - the average price of a home for each year the home was built that have 3 bedrooms and 3 bathrooms rounded to two decimal places
![Alt text](<Screenshot 2024-02-02 111415.png>)

    - the average price of a home for each year built that have 3 bedrooms, 3 bathrooms, with two floors, and are greater than or equal to 2,000 square feet rounded to two decimal places
![Alt text](<Screenshot 2024-02-02 111427.png>)

    - the "view" rating for the average price of a home, rounded to two decimal places, where the homes are greater than or equal to $350,000
![Alt text](<Screenshot 2024-02-02 111439.png>)

    - cache the data and using the cached data, run the query that filters out the view ratings with average price greater than or equal to $350,000
![Alt text](<Screenshot 2024-02-02 111456.png>)

    - the query that filters out the view ratings with average price of greater than or eqaul to $350,000 with the parquet DataFrame
![Alt text](<Screenshot 2024-02-02 111506.png>)

    -Determine the runtime and compare it to the cached version.
By comparing the runtimes of the cached and uncached versions, we can determine that caching provides a performance improvement. The cached version is faster, it suggests that caching is effective in reducing the computational overhead.



# Dependencies
The analysis is conducted using Python programming language using Google Colab and relies on the following libraries:

findspark
pyspark
SparkFiles