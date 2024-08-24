## Marketing Strategy Analysis According to Customer Behavior

- How consumers decide when purchasing products or services, the personal, social and psychological parameters they are affected by, and their after-sales expectations from companies determine the behavior of consumers.

- Businesses try to increase their market shares, brand values ​​and profitability by using marketing strategies by dividing consumers into various groups and applying similar strategies to customers whose behaviors are similar.

### Goals

- It is desired to examine the returns to the campaigns through customer behavior analysis and to determine the return effects on the campaign.
-By analyzing customer behavior, it is desired to create a model to predict whether the customer will accept the offer in the last campaign.
- It is desired to analyze the customer base according to those who share similar characteristics and to obtain campaigns with better returns on the created clusters.

## Task

- Load Data
- Data Cleaning 
- Feature Engineering
- Data Visualization
- Create Model
 - Simple Logistic Regression 
   - Using Metrics: Accuracy, Confusion Matrix, Recall, Precision, F1 Score
 - Full Logistic Regression
   - Using Metrics: Accuracy, Confusion Matrix, Recall, Precision, F1 Score
- Clustering
 - Scale Data
 - KMeans
   - Silhouette score
- Analysis
 - visualization evaluation
 - Insights

 ## Dataset Summary Information

- [AcceptedCmp1], [AcceptedCmp2], [AcceptedCmp3], [AcceptedCmp4],[AcceptedCmp5],[AcceptedCmp6]: 1 if campaign offers are accepted, 0 if not.
- [Complain] If the customer has made a complaint within the last 2 years 1
- [Marital_Status]: Marital status of the customer.
- [Dt_Customer] Müşterinin şirkete kayıt tarihi
- [Income] Customer's income.
- [MntFishProducts] Amount spent on fish products.
- [MntGoldProds] Amount spent on gold products.
- [MntSweetProducts]  Amount spent on sweet products.
- [MntFruits]  Amount spent on fruits products.
- [MntMeatProducts]  Amount spent on meat products.
- [MntFishProducts]  Amount spent on fish products.
- [NumDealsPurchases] Number of purchases made with deals or discounts.
- [NumWebPurchases] Number of purchases made through the web.
- [NumCatalogPurchases] Number of purchases made from catalogs.
- [NumStorePurchases] Number of purchases made from store.
- [Recency] Number of days since the last purchase.
- [Z_CostContact] Cost of contacting the customer.
- [Z_Revenue] Revenue generated from the customer.
- [Education] SMA: Three years high school, s1: bachelor, s2: master, s3: doctorate, d3: vocational school



## Conclusion

Logistic Regressions:
- In general, if customers responded to the first five campaigns, they also respond positively to the last campaign. However, there are customers who responded negatively to the previous campaign and responded positively to the latest campaign.
- When full logistic regression was performed by including other customer behaviors, a better predictive value was obtained than simple logistic regression. This shows that customer behavior (time since the last purchase, income level, age, shopping environment, etc.) has a more important impact on the participation rates in the campaign.

Clustering:
- n_clusters=3

Customers were seperated into three clusters. Insights into these clusters were gained.

Cluster 3 Insights:
- The focus should be on this cluster. Because almost every type of product has high sales.
- Those with high income are in this cluster.
- Focus should be on catalog and store sales. Because the most spending is here.
- Online purchasing is high but website visits are low.

Cluster 2 Insights:
- This customer should not have any room points.
- Purchases are low. They visit the website but do not buy the product.

Cluster 1 Insights:
- A cluster with a high concentration of customers who have more children at home compared to other clusters.
- Too many products are purchased. The website is highly visited.
- The second focus should be this cluster. They are customers with average income. They are more likely to purchase medium or low cost products.

- n_clusters=4
Customers were seperated into four clusters. Insights into these clusters were gained.
  
Cluster 0 Insights:
- Low-income, old customer group with low shopping potential. Not a suitable target.

Cluster 1 Insights:
- High potential customer group. Campaign acceptance rates, income levels and total 
expenditures are also better. A very suitable target.

Cluster 2 Insights:
- Low income, low spending, slightly newer customers. The majority of married 
customers.

Cluster 3 Insights: 
- Customer group with high income levels and spending above average
