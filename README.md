# Big Data

## Overview of Analysis

### *Deliverable One*: To connect to an Amazon Web Services (AWS) Instance before extracting, transforming and loading an Amazon Vine dataset into pgAdmin, creating four distinctly useful dataframes in the process. 

### *Deliverable Two*: To utilize the ``Vine_Table`` dataframe created in Deliverable One, filtering for ``helpful`` reviews and whether said reviews were part of the paid Amazon Vine program to determine whether paid reviews showcased bias compared to their unpaid counterparts. 

## Deliverable One: Creating Dataframes

## Deliverable Two: Filtering for Amazon Vine Data

### Paid Amazon Vine Participants

From our ``Vine_Table`` we used Google Collab to create a dataframe to house our AWS dataset, filtering for those who were part of the Amazon Vine program. The code used to create that dataframe, and the calculations based around said dataframe are listed below. 

![](https://github.com/chrisknox97/amazon_vine/blob/main/PNGs/paid_code.png)
![](https://github.com/chrisknox97/amazon_vine/blob/main/PNGs/paid_df.png)
![](https://github.com/chrisknox97/amazon_vine/blob/main/PNGs/paid_calculation.png)

### Unpaid Participants

We also used Google Collab to create a dataframe to filtering for those who were not part of the Amazon Vine program. The code used to create that dataframe, and the calculations based around said dataframe are listed below. 

![](https://github.com/chrisknox97/amazon_vine/blob/main/PNGs/unpaid_code.png)
![](https://github.com/chrisknox97/amazon_vine/blob/main/PNGs/unpaid_df.png)
![](https://github.com/chrisknox97/amazon_vine/blob/main/PNGs/unpaid_calculation.png)

## Results

The Results of our analysis showed a disparity between reviews affiliated and unaffiliated with the Amazon Vine Program. For this dataset, most reviews were unaffiliated with Amazon Vine. However, those affiliated with the program had a higher propensity to award a product a 5-Star Review compared to the overall 5-Star review percentage. 

### Vine Review Totals

* There were 94 reviews in the Amazon Vine Program. 
* There were 40,471 reviews unaffiliated with the Amazon Vine Program.

### 5-Star Reviews

* There were 48 5-Star reviews in the Amazon Vine Program. 
* There were 15,663 5-Star reviews unaffiliated with the Amazon Vine Program. 

### Percentage of 5-Star Reviews

* The percentage of 5-Star reviews in the Amazon Vine Program was approximately 51 percent. 
* The percentage of 5-Star reviews unaffiliated with the Amazon Vine Program was approximately 39 percent. 
* The overall percentage of 5-Star reviews deemed 'helpful' was approximately 39 percent. 

## Summary

### Positivity Bias

The results initially suggest that there is positivity bias in the paid Amazon Vine program with approximately 51 percent of participants awarding a 5-star review compared to only 39 percent of those unaffiliated (a 12 percent difference). Additionally, the 39 percent of 5-star reviews from those unaffiliated with the Amazon Vine program aligns with our overall 5-star review percentage of 39 percent. 

### Sample Size

However, the issue of these results remains sample size as only 94 reviews analyzed (as part of our ``helpful`` reviews dataset) were part of the Amazon Vine program compared to 40,471 reviews that remained unaffiliated. That difference of nearly 40,000 reviews cannot be ignored and may have contributed to the 12-percent difference in the respondent's 5-Star review percentages. 

### Verified Purchases

Another issue arises when it comes to whether a review is associated with a verified purchase. When we displayed the first 20 rows of our two datasets (Amazon Vine participants, non-Amazon Vine participants), we found that while some non-Amazon Vine participants had verified purchases, none of the initial twenty reviews for Amazon Vine had a verified purchase. Without a verified purchase, customers may be led to question the validity of its associated review. 

### Further Analysis

Similarly, additional analysis can be conducted to uncover whether our own analysis remains indicative of the Amazon Vine service, or rather an aberration. Further analysis include:

* Analysis of Additional Amazon Vine Datasets
* Comparative Analysis Examining Percentage of Positive (3-Star Rating and Above) and Extremely Positive (4-Star Rating and Above) Reviews in Amazon Vine Program and those Unaffiliated. 
* Comparative Analysis Examining Percentage of Verified Purchases for Amazon Vine and Non-Amazon Vine Participants 
* Comparative Analysis Examining Percentage of Positive Reviews with Percentage of Verified Purchases

Whenever a program exists where reviews may be paid for, customer inclination remains to dismiss them as dishonest, and undermines the product's integrity. This analysis has only furthered questions surrounding this program, yet without additional analysis, no definitive conclusion can yet be made.
