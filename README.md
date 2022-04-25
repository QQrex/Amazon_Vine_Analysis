# Amazon_Vine_Analysis

## Purpose

We are tasked to analysis Amazon reviews from wireless products written by Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products.

## Overview
For us to complete our analysis we must extract our data from Amazon wireless S3 dataset and then transform our wireless dataset so it could be read into our AWS RDS database with tables in pgAdmin. Once in pgAdmin, we can export our vine review table as a csv file and use Pandas to analysis our data for:

- Total reviews and total helpful reviews.
- Total vine subscriber and non-vine subscribers.
- Total 5-star reviews, vine subscribed and non-vine subscriberd.
- Percentage of 5-star vine subscribed and non-vine subscribed reviews.

## Results

![total]()
- With our dataset container over 9 million reviews, we decided to narrow down our dataset by filtering for reviews with helpful votes percentage greater than 50%. In our helpful reviews, we found 613 vine subscriber reviews and 64968 non vine subscriber reviews.

![five]()
- From there we narrowed down our search for only 5-star reviews and found a total of 222 vine subscriber reviews and 30543 non vine subscriber reviews.

![percent]()
- Finally, we calculated 36.22 % of vine subscribers gave 5 star reviews and 47.01% of non-vine subscribers gave 5 star reviews.

## Summary

In summary, when looking at only helpful reviews from our Amazon dataset, we see 36.22% of vine subscribers and 47.01% of non-vine subscribers giving 5-star reviews. This is only about a 10% difference, so we can say for 5-star reviews there is no bias from vine subscribers. However, we can only say that about 5-star reviews. We can expand on our analysis by filtering our data for verified or not verified purchase as well. In addition, we can also
