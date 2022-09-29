# Amazon Vine Analysis

## Overview of analysis
In this analysis, PySpark in a colab notebook was used to perfom an extract, transform and load on a data set of Amazon reviews for outdoor products. Using
AWS to create an RDS database and then connecting to a local postgres pg admin, the new dataframes were loaded into postgres database tables. Additional analysis
was performed using PySpark to determine if there was favorable bias toward paid vine reviews for the products in the dataset. To achieve this the data was
filtered to reviews that had more than 20 votes. Then the data was split into vine reviews and non vine reviews. The percentage of 5 star reviews was then 
calculated from these to sets.
## Results
- There were 107 paid Vine reviews
- There were 39,869 non_Vine Reviews
- There were 56 five star reviews for Vine reviews
- There were 21,005 five star reviews for non-Vine reviews
- The percentage of five star reviews for Vine was 52.33%
- The percentage of five star reviews for non-Vine was 52.68%
## Summary
There was not a favorable bias for paid vine reviews. Vine reviews had slightly smaller percentage, but practically the same, of five star reviews than
non-vine reviews. Additional analysis to consider when looking at the vine reviews would be, to find the percentage of four and five star reviews for
both vine and non vine reviews to compare.
