# Amazon_Vine_Analysis

# Overview of the analysis
Since the intial work on the SellBy project was so successful, a new larger project has been assigned: analyzing Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.

In this project, the team has access to approximately 50 datasets. Each one contains reviews of a specific product, from clothing apparel to wireless products.  The dataset for wireless products was selected for analysis by the team and PySpark is used to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Next, Pandas is used to determine if there is any bias toward favorable reviews from Vine members in the dataset. A summary of the analysis is generated for submission to the SellBy stakeholders.

# Resources

- Data Sources:  Amazon review dataset:   https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Wireless_v1_00.tsv.gz
- Software: Google Colab with PySpark, pgAdmin, Python, Jupyter notebook 

# Results
## Deliverable 1
PySpark is used to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Images of the process are captured below: 

![Alt Text](https://github.com/syoder821/Amazon_Vine_Analysis/blob/main/Resources/load_amazon_data.png) 

![Alt Text](https://github.com/syoder821/Amazon_Vine_Analysis/blob/main/Resources/tables1_2_creation.png) 

![Alt Text](https://github.com/syoder821/Amazon_Vine_Analysis/blob/main/Resources/tables3_4_creation.png)

![Alt Text](ADD AWS RDS INstance)

## Deliveriable 2 
Pandas is used to determine if there is any bias toward favorable reviews from Vine members in the Wireless product dataset.

Retrieve data with > 20 total votes and helpful votes > 50%
![Alt Text](https://github.com/syoder821/Amazon_Vine_Analysis/blob/main/Resources/clean_data_frame.png) 


Retrieve Vine and non-Vine data
![Alt Text](https://github.com/syoder821/Amazon_Vine_Analysis/blob/main/Resources/Vine_paid_unpaid.png) 


Total the Vine and non-Vine data
![Alt Text](https://github.com/syoder821/Amazon_Vine_Analysis/blob/main/Resources/vine_totals.png) 

- How many Vine reviews and non-Vine reviews were there? There are 613 Vine reviews and 64968 non-Vine reviews.  
- How many Vine reviews were 5 stars?  222 Vine reviews recieved a Five star rating.   
- How many non-Vine reviews were 5 stars? 30543 non-Vine reviews recieved a Five star rating. 
- What percentage of Vine reviews were 5 stars? 36.21% of Vine reviews recieved Five stars.  
- What percentage of non-Vine reviews were 5 stars? 47.01% of non-Vine reviews recieved Five stars.  

# Summary
The results from the anaysis do not show any positivity bias for Five tar reviews in the Vine program.  The percentage of Five star reviews in the Vine program was 36.21% while the percentage of non_Vine reviews that recieved Five stars was ~ 11% higher at 47.01%.  Additional product categories could be examined in a similiar fashion to determine if this trend holds true.  Also, the results could be analyized further to look at the average review ratings and standard deviation to determine if Vine members give on average higher ratings vs. non-Vine memebers.  

