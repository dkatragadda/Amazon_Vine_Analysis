# Amazon_Vine_Analysis

## Project Overview

This project involved the usage of big data technologies to access large amounts of data on Amazon's S3 service and perform ETL activities using Pyspark and Amazon's RDS instance of a PostgreSQL database. This project analyzed product reviews for Grocery on the Amazon US website. Our goal was to go through the reviews and transform the data and break up the dataset into 4 different dataframes and load the PostgreSQL tables on RDS with the dataframes. Subsequently, we analyzed the dataset pertaining to the reviews to determine if there was any positivity bias for 5-star reviews in the paid or Vine review program. 

## Resources
* [Amazon Review Datasets](https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt "Amazon Review Datasets"), [Grocery Review Datasets](https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Grocery_v1_00.tsv.gz "Grocery Review Datasets")
* Tools Used: Google Colab Notebooks, PostgreSQL 12.5, Amazon RDS, pgAdmin 4

## Results

### Total number of Reviews
* Vine/Paid Reviews

![Paid_Reviews](https://github.com/dkatragadda/Amazon_Vine_Analysis/blob/main/Resources/Total_Vine_Reviews.png)

There were a total of 61 paid or vine reviews in the dataset for grocery.

* Unpaid Reviews

![Unpaid_Reviews](https://github.com/dkatragadda/Amazon_Vine_Analysis/blob/main/Resources/Total_Unpaid_Reviews.png)

There were a total of 28,287 unpaid reviews in the dataset for grocery.

### Total number of 5-Star Reviews
* Vine/Paid 5-Star Reviews

![Paid 5-Star_Reviews](https://github.com/dkatragadda/Amazon_Vine_Analysis/blob/main/Resources/Total_5_star_paid.png)

There were a total of 20 paid or vine 5-star reviews in the dataset for grocery.

* Unpaid 5-Star Reviews

![Unpaid 5-Star_Reviews](https://github.com/dkatragadda/Amazon_Vine_Analysis/blob/main/Resources/Total_5_star_unpaid.png)

There were a total of 15,689 unpaid reviews in the dataset for grocery.

### Percent of 5-Star Reviews
* % of vine/paid 5-star reviews

![% of Paid 5-Star_Reviews](https://github.com/dkatragadda/Amazon_Vine_Analysis/blob/main/Resources/Percent_5_star_paid.png)

32.8% of the paid/vine reviews were 5-star reviews. 

* % of unpaid 5-star reviews

![% of Unpaid 5-Star_Reviews](https://github.com/dkatragadda/Amazon_Vine_Analysis/blob/main/Resources/Percent_5_star_unpaid.png)

55.5% of the unpaid reviews were 5-star reviews. 


## Summary 

Based on the analysis conducted, there is no positivity bias towards 5-star reviews in the paid/vine review program. This is based on the fact that only 32.8% of the paid reviews were 5-star reviews whereas 55.5% or a higher proportion of the unpaid reviews were 5-star reviews indicating that paid reviews may not yield certainty of receiving 5-star reviews.  

Further analysis can be conducted on the dataset to look at the statistical distribution of the ratings for the paid and unpaid reviews by reviewing the mean, median, mode etc. This will help in making a more advised decision on the dataset. 

