# Customer and Purchase Analysis for a Retail Store

Analysis of the segmentation and purchase dataset of a retail store

## Tools and Technologies

![microsoftexcel Badge](https://img.shields.io/badge/-excel-217346?style=for-the-badge&labelColor=black&logo=microsoftexcel&logoColor=217346) ![python Badge](https://img.shields.io/badge/-python-3776AB?style=for-the-badge&labelColor=black&logo=python&logoColor=3776AB) ![jupyter Badge](https://img.shields.io/badge/-jupyter-F37626?style=for-the-badge&labelColor=black&logo=jupyter&logoColor=F37626)


## Process and Report

### Customer Segmentation

- See jupyter notebook file for [customer segmentation](https://github.com/uedwinc/Retail-Store-Customer-Analytics-in-Python/blob/main/Customer%20Analytics%20-%20Segmentation/Customer%20Analytics%20-%20Segmentation.ipynb)

- We employed correlation heatmap to see the correlation between different variables of the dataset

- Then, we used K-Means and Hierarchical clustering to obtain four (4) clusters for the customer base:
    - Fewer opportunities group
    - Standard group
    - Career-focused group
    - Well-off group

- Lastly, we used Principal Component Analysis (PCA) to understand the variance in the data

### Customer Purchase Descriptive Analysis

- See jupyter notebook file for [customer purchase descriptive analysis](https://github.com/uedwinc/Retail-Store-Customer-Analytics-in-Python/blob/main/Purchase%20Analytics%20-%20Descriptive%20and%20Predictive/Purchase%20Analytics%20-%20Descriptive.ipynb)

- We determined the proportions of the different cluster segments in the purchse data based on the number of purchases

|Segment|Proportions|
|---|---|
|Standard|20.6|
|Career-Focused|22.0|
|Fewer-Opportunities|37.8|
|Well-Off|19.6|

- We also obtained the average number of store visits by segments and the average number of purchases by segment

![store visits](https://github.com/uedwinc/Retail-Store-Customer-Analytics-in-Python/blob/main/images/store%20visits.png)  ![purchases](https://github.com/uedwinc/Retail-Store-Customer-Analytics-in-Python/blob/main/images/purchases.png)

- Finally, we obtained the brand preference of the different segments and their contributions to the brand revenue

![brand choice](https://github.com/uedwinc/Retail-Store-Customer-Analytics-in-Python/blob/main/images/brand%20choice.png)

|Segment|Total Revenue|
|---|---|
|Standard|14590.01|
|Career-Focused|24952.16|
|Fewer-Opportunities|20790.10|
|Well-Off|22424.31|

### Customer Purchase Predictive Analysis

- See jupyter notebook file for [customer purchase predictive analysis](https://github.com/uedwinc/Retail-Store-Customer-Analytics-in-Python/blob/main/Purchase%20Analytics%20-%20Descriptive%20and%20Predictive/Purchase%20Analytics%20-%20Predictive.ipynb)

- We created a purchase probability model for our customers based on price

    - We obtained a negative coefficient signaling that with an increase in price, the purchase probability decreases.

- Next, we compute the purchase probability and price elasticity for the different segments:

    > For the Career-Focused, we observe that the Career-focused segment are the least elastic when compared to the rest. So, their purchase probability elasticity is not as affected by price.

    > Fewer-Opportunities segment are the most affected by price

    > The standard segment is least homogenous, which we discovered during our descriptive analysis. It may be that the customers in this segment have different shopping habbits, which is why their customers start with being more elastic than average but then shift to being more inelastic than the average customer

- We also calculated the purchase probability with promotion feature as well as the brand choice for the different segments

    - It appears that promotion reflects negatively on the purchase quantity of the average client, which is unexpected.
    

- We also observe differences and similiraties between the segments and examine their preference, when it comes to brand choice.

    > The two segments, which seem to be of most interest for the marketing team of brand 5, are the Career-focused and the Well-off. They are also the segments which purchase this brand most often. 

    > The Career-focused segment is the most inelastic and they are the most loyal segment. Based on our model, they do not seem to be that affected by price, therefore brand 5 could increase its price, without fear of significant loss of customers from this segment. 

    > The Well-off segment on the other hand, seems to be more elastic. They also purchase the competitor brand 4 most often. In order to target this segment, our analysis signals that price needs to be decreased. However, keep in mind that other factors aside from price might be influencing the purchase behaivour of this segment.
