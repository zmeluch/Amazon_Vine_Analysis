# Amazon Vine Analysis

## Overview of analysis
In this analysis, PySpark in a colab notebook was used to perfom an extract, transform and load on a data set of Amazon reviews for outdoor products. Using
AWS to create an RDS database and then connecting to a local postgres pg admin, the new dataframes were loaded into postgres database tables. Additional analysis
was performed using PySpark to determine if there was favorable bias toward paid vine reviews for the products in the dataset. To achieve this the data was
filtered to reviews that had more than 20 votes. Then the data was split into vine reviews and non vine reviews. The percentage of 5 star reviews was then 
calculated from these to sets.
## Results
- There were 107 paid Vine reviews
![Vine_Total](https://user-images.githubusercontent.com/103155045/192915053-21368ced-1a17-4d27-acd6-749145064a68.png)
- There were 39,869 non_Vine Reviews
![Non_Vine_Total](https://user-images.githubusercontent.com/103155045/192915071-e77c28c5-2920-47f9-9c77-a1671aef93e0.png)
- There were 56 five star reviews for Vine reviews
![5_star_Vine](https://user-images.githubusercontent.com/103155045/192915088-ea833acc-d83d-44c9-a970-6ec6770b124c.png)
- There were 21,005 five star reviews for non-Vine reviews
![5_star_Non_VIne](https://user-images.githubusercontent.com/103155045/192915104-9bddbe42-9022-4357-aa6e-8d3b76533b88.png)
- The percentage of five star reviews for Vine was 52.33%
![Vine_5_star_percentage](https://user-images.githubusercontent.com/103155045/192915127-4f129f0a-0e03-4092-995d-8feb64dcc542.png)
- The percentage of five star reviews for non-Vine was 52.68%
![Non_Vine_5_star_percentage](https://user-images.githubusercontent.com/103155045/192915153-2072d6dd-ed6b-4def-8929-d190df4fa777.png)
## Summary
There was not a favorable bias for paid vine reviews. Vine reviews had slightly smaller percentage, but practically the same, of five star reviews than
non-vine reviews. Additional analysis to consider when looking at the vine reviews would be, to find the percentage of four and five star reviews for
both vine and non vine reviews to compare.
