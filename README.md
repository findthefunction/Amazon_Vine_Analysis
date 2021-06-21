# Amazon Vine Analysis

![vine_table](https://user-images.githubusercontent.com/31022640/122704099-d2501600-d207-11eb-9d9d-c30b0854e37e.png)

## Overview of the analysis: 

The purpose of this analysis is to utilize the review data provided and determine if there are any pattern in the data that could suggest bias.  The analysis will be performed by comparing two seperate groups of reviewers, a paid group and a non paid group.  

## Results: 

After performing ETL on the Amazon data set by using an Amazon RDS instance and pgAdmin the data was converted to a Pandas DataFrame for further analysis.  The data was filtered to promote quality data by eliminating the reviews with a lower percentage of "helpful" upvotes.

![to_pandas](https://user-images.githubusercontent.com/31022640/122664775-3ddaaa80-d158-11eb-8b80-ef41e01b9c69.png)

- How many Vine reviews and non-Vine reviews were there?

  - There were 1080 paid vine review and 49673 unpaid vine review in our modified dataset that include only 5 star ratings

![image](https://user-images.githubusercontent.com/31022640/122665196-b478a780-d15a-11eb-91ec-637d4151dc28.png)

![image](https://user-images.githubusercontent.com/31022640/122665245-f9044300-d15a-11eb-82ba-152c85a38ca3.png)

  - How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
    -  454 Vine reviews and 23043 non-Vine reviews
  - What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?
    -  1.9% paid and 98% unpaid reviews
![image](https://user-images.githubusercontent.com/31022640/122704429-910c3600-d208-11eb-8f11-fa52aacd046a.png)


## Summary: 

The positivity bias that was potentially uncovered through our data analysis identifies that the unpaid vine reviewers had significantly higher instances of 5 star review for products. In contrast, the paid vine reviewers had a very low 5 star percentages, suggesting that they took the task more seriously and approached the reviews more critically.  
