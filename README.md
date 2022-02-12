# Amazon_Vine_Analysis

![Screenshot 2022-02-12 151808](https://user-images.githubusercontent.com/88118587/153726998-df61bf14-4ed7-4ec7-936a-9e9b6aa40807.jpg)

## Overview

The Amazon Vine program enables manufacturers and publishers to receive reviews for their products. Companies such as SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review. With google Colab and Pyspark, we have performed the ETL process to extract the dataset, transform the data and connect to an AWS RDS instance, then load the transformed data into pgAdmin. Finally, we have continued to use Google Colab and Pyspark to determine if there is bias toward favorable reviews from vine members in our dataset.

## Resources
Data Source: 
* [Amazon Review datasets](https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt)

* [Video Games Review dataset](https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Video_Games_v1_00.tsv.gz)
## Software: 
* Google ColabNotebook
* AWS Simple Storage Service (S3)
* Pyspark to handle Dataset and ETL
*PostgreSQL
* pgAdmin 4 

## Results

![totalrating1](https://user-images.githubusercontent.com/88118587/153728816-f8cf1441-80fc-49c9-9226-54726450912b.jpg)


> 1. How many Vine reviews and non-Vine reviews were there?
> 
>> A : **46,125**
>2. How many Vine reviews were 5 stars? 
>
>>A: **480**
>3. How many non-Vine reviews were 5 stars?
>
>>A: **45645**
>4. What percentage of Vine reviews were 5 stars? 
>
>>A: **35.29%**
>5. What percentage of non-Vine reviews were 5 stars?
>
>>A: **44.53%**

## Summary
The results suggest that the members of the vine program are not biased, as they show a low rate of 35.30%, and that non-vintage members had a higher percentage with 44.53%. If we could also find out how recent the vine members were in these reviews, we could try to find out whether there is psychological pressure to give the products a higher or lower rate. We could adopt a more statistical approach, such as the mean, the median mode.  

