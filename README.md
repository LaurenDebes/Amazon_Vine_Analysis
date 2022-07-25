# Amazon Vine Analysis
Module 16 Challenge
## Overview of Analysis
We have been asked to analyze Amazon reviews and compare those written by the paid Amazon Vine program to regular customer reviews. We analyzed the "jewelry" dataset with PySpark to perform ETL into pgAdmin. We are looking to see if there are any biases in reviews from the vine members.

## Results
We first filtered our data to show only products with 20 or more votes for the review and with 50% or more of the views being rated as helpful. This allowed us to look at higher quality reviews.
  - <b>Number of reviews:</b> There were 21 vine reviews and 7689 reviews that did not use vine. 
  - <b>Number of 5 star reviews:</b> There were 11 vine reviews with 5 stars and 4444 regular reviews with 5 stars.
  - <b>Percentage of 5 star reviews:</b> 53% of the reviews were 5 star from vine users, while 57% of the reviews were 5 star without vine.
![vinereviews.png](https://raw.githubusercontent.com/LaurenDebes/Amazon_Vine_Analysis/main/vinereviews.png) ![regularreviews.png](https://raw.githubusercontent.com/LaurenDebes/Amazon_Vine_Analysis/main/regularreviews.png) 

## Summary
There does not appear to be any positivity bias for reviews in the Vine program. There were actually 4% less 5 star reviews from users of the vine program. An additional analysis that could be done would be to look at the individual customer_ids and see if there are users that always rate things 5 star and to filter them out if so. You could also filter for verified versus unverified purchase to see if that changes the number of 5 star reviews.

