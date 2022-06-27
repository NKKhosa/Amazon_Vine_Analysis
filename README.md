# Amazon Vine Analysis

## Overview of the analysis

An analysis was conducted on Amazon reviews to determine if companies participating in the Vine program recieve more 5-star reviews. Out of 50 available datasets of different product categories, one was chosen for the analysis to be conducted on (Jewelry). ETL was conducted using PySpark, and the transformed data was then loaded onto a PostgresSql database hosted on AWS. 

## Results

- Vine reviews 
	- There were 21 total Vine reviews.
	- There were 11 5-star Vine reviews.
	- 52.4% of Vine reviews were 5-star.
	
- Non-Vine reviews
	- There were 7689 total non-Vine reviews.
	- There were 4444 5-star non-Vine reviews.
	- 57.8% of non-Vine reviews were 5-star. 


## Summary

Based on the analysis, there is not a positivity bias for reviews in th Vine program. In fact, the percentage of 5-star reviews was lower for reviews in the Vine program than non-Vine reviews. A statistical test should be done to determine if the difference between the Vine reviews (52.4%) and the non-Vine reviews (57.8%) is significantly different.

The above analysis, however, was conducted strictly on 5-star reviews. This is a very strict threshold for 'positive' reviews. Further analysis could be conducted on 4-star reviews, separately as well as in addition to 5-star reviews (i.e. filtelring the dataframe for 4-star reviews and then filtering it for 4+5-star reviews and analyze both). 

An analysis could also be conducted on the negative reviews to see if the Vine program has fewer poor reviews.
