# Amazon_Vine_Analysis

# Overview of the analysis
Since your work with Jennifer on the SellBy project was so successful, you’ve been tasked with another, larger project: analyzing Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.

In this project, you’ll have access to approximately 50 datasets. Each one contains reviews of a specific product, from clothing apparel to wireless products. You’ll need to pick one of these datasets and use PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Next, Pandas is used to determine if there is any bias toward favorable reviews from Vine members in your dataset. A summary of the analysis for Jennifer to submit to the SellBy stakeholders is provided.

# Resources

- Data Sources:  Amazon review dataset:   https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Wireless_v1_00.tsv.gz
- Software: pgAdmin, Python, Jupyter notebook 

# Results

![Alt Text](https://github.com/syoder821/Amazon_Vine_Analysis/blob/main/Resources/load_amazon_data.png) 

Retrieve data with > 20 total votes and helpful votes > 50%

![Alt Text](https://github.com/syoder821/Amazon_Vine_Analysis/blob/main/Resources/clean_data_frame.png) 


![Alt Text](https://github.com/syoder821/Amazon_Vine_Analysis/blob/main/Resources/tables1_2_creation.png) 

![Alt Text](https://github.com/syoder821/Amazon_Vine_Analysis/blob/main/Resources/tables3_4_creation.png)

Results: Using bulleted lists and images of DataFrames as support, address the following questions:

How many Vine reviews and non-Vine reviews were there?
How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?

![Alt Text](https://github.com/syoder821/Amazon_Vine_Analysis/blob/main/Resources/Vine_paid_unpaid.png) 

![Alt Text](https://github.com/syoder821/Amazon_Vine_Analysis/blob/main/Resources/vine_totals.png) 

# Summary
Summary: In your summary, state if there is any positivity bias for reviews in the Vine program. Use the results of your analysis to support your statement. Then, provide one additional analysis that you could do with the dataset to support your statement.

