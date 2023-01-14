# Online-Retail-Customer-Segmentation
 Identify major customer segments.
 # **Project Summary -**
 #### In this project, our task was to identify major customer segments on a transnational data set that contained one-year historical transactions for a UK-based online retail store. This would help the company segregate its customers based on transaction data and help them in marketing decisions and strategy.
#### Effective decisions are  mandatory   for any   company   to   generate   good revenue. In these days competition is huge   and   all  companies   are   moving forward   with   their   own   different strategies.   We   should   use   data   and take a proper decision. Every person is different   from   one   another   and   we don’t know what he/she buys or what their  likes  are.   But,  with the   help  of machine   learning  technique   one  can sort out the data and can find the target group by applying   several   algorithms to the dataset. Without this, It will be very difficult and no better techniques are   available   to   find   the   group   of people   with   similar   character   and interests in a large dataset.Customer segmentation can help businesses focus on each customer group in a different way, in order to maximise benefits for customers as well as the business.
#### After basic exploration and cleaning the data we found relationships between features in EDA and then jumped into the RFM analysis part.I implemented various unsupervised machine learning algorithm such as KMeans Clustering,  Hierarchical Clustering(Agglomerative Clustering). Here to find the Optimal number of clusters we used Elbow method and Silhouette Score and Silhouette Plot to visualize the clusters with different number of clusters. For Agglomerative Clustering we used Dendogram to find the optimal number of clusters.
#### First imported the libraries and dataset which was in excel file and This dataset contains 541909 rows and 8 columns, then checked for duplication of data and null values.
#### There were more than 120000 null values present in CustomerID Column it main column as other column was filled with zero and drop all values.
#### Various plots are visualized to see Outliers and Applied Inter Quartile Range method.
#### RFM analysis can segment customers into homogenous group quickly with set of minimum variables. Scoring system can be defined and ranged differently. We get a better result for clustering steps by applying scoring rather than using the raw calculated RFM values. Therefore, segmenting should be done by RFM scoring and further analysis on the spending behavior should be done on the raw values for the targeted cluster to expose more insight and characteristics. RFM analysis solely depends on purchasing behavior and histories, analysis can be further improved by exploring weighted composite scoring or including customer demographic information and product information. A good analysis can increase effectiveness and efficiency of marketing plans, hence increase profitability at minimum cost.
#### Data was used different units so its scaled using Standard Scaler and normalise data.To find Number Clusters we applied Elbow Method and silhouette score the Selected Cluster Size with Visualized Graph.K-Means Clustering was applied,Dendrogram Linkage and Hierarchical Agglomerative Clustering Models are applied.
#### We started with a simple binning and quantile based simple segmentation model first then moved to more complex models because simple implementation helps having a first glance at the data and know where/how to exploit it better.
#### Then we moved to k-means clustering and visualized the results with different number of clusters. As we know there is no assurance that k-means will lead to the global best solution. We moved forward and tried Hierarchical Clustering

### Variables Description 
#### **InvoiceNo:** Invoice number. Nominal, a 6-digit integral number uniquely assigned to each transaction. If this code starts with letter 'c', it indicates a cancellation.

#### **StockCode:** Product (item) code. Nominal, a 5-digit integral number uniquely assigned to each distinct product.

#### **Description:** Product (item) name. Nominal.

#### **Quantity**: The quantities of each product (item) per transaction. Numeric.

#### **InvoiceDate**: Invice Date and time. Numeric, the day and time when each transaction was generated.

#### **UnitPrice:** Unit price. Numeric, Product price per unit in sterling.

#### **CustomerID:** Customer number. Nominal, a 5-digit integral number uniquely assigned to each customer.

####**Country:** Country name. Nominal, the name of the country where each customer resides.

# **Conclusion**
#### Following are the conclusion made during EDA:

#### 1. Top Five Countries: Uniter Kingdom, Germany, France, Ireland and Spain.

#### 2. Month which give maximum business: November, October, December, September and May.

#### 3. Maximum purchasing on different days: Thursday > Wednesday > Tuesday > Monday > Saturday > Friday.

#### 4. Most of the customers usually purchase products in between 10:00 A.M to 3:00 P.M.

#### 5. The company should make sure that the website server is up and running during that hrs, and also invest on cx support during that hrs.

#### 6. WHITE HANGING HEART T-LIGHT HOLDER > REGENCY CAKESTAND 3 TIER> JUMBO BAG RED RETROSPOT were ordered with top 3 highest frequency.
#### The company is suggested to keep the inventory always stocked with these products.

#### 7. GLASS AND BEADS BRACELET IVORY , CROCHET LILAC/RED BEAR KEYRING , PINK BAROQUE FLOCK CANDLE HOLDER were ordered in the lo9west number.

#### 8. A number of cx also cancelled the order. The company should ideally look into it.

#### 9. Given Data for Customer Segmentation most of them are irrelevant like StockCode, Description.etc and there is no relation.

#### 10. After Applying Elbow and Silhouette score are more at cluster size =3 or 2

#### 11. Same results applied with Dendrogram results of Kmeans Clusters Centers in plots appears better than Hierarchical Agglomerative Clustering

#### **Cluster_0 CustomerID's take more time gap between Each Order they Placed (Rarely).**

#### **Cluster_1 CustomerID's Makes always a Bulk Purchases which leads high Spending's (Retailers).**

#### **Cluster_2 CustomerID's Has Highest Orders Placed (Small Shops with less inventory).**

#### 12. To conclude, we saw how we can segment our customer depending on our business requirements. You can perform RFM for your entire customer base, or just a subset. For example, you may first segment customers based on a geographical area or other demographics, and then by RFM for historical, transaction-based behaviour segments. RFM analysis can help in answering many questions with respect to their customers and this can help companies to make marketing strategies for their customers, retaining their slipping customers and providing recommendations to their customer based on their interest. We used the K-means algorithm to segment our customer in various clusters having similar similarity. I think K-means did a pretty good job here.

#### **How is your project useful to stakeholders.**

##### The project help the company to improve their business by undestanding the income , highest selling product , based on the country where the customer residing . so considering these factors company can sell more product depenting on their needs , and region where most of the wholesailers residing etc .


