# Online-Retail-Customer-Segmentation
Customer segmentation is the process of separating customers into groups on the basis of their shared behavior or other attributes. The groups should be homogeneous within themselves and should also be heterogeneous to each other. The overall aim of this process is to identify high-value customer base i.e. customers that have the highest growth potential or are the most profitable.

In this project, our task is to identify major customer segments on a transnational dataset which contains all the transactions occurring between 01/12/2010 and 09/12/2011 for a UK-based and registered non-store online retail. The company mainly sells unique all-occasion gifts. Many customers of the company are wholesalers. So we need to divide customers into n number of segments to find out which group we need to focus on most to help for business growth.

To solve the above problem we run an experiment on the UK-based and registered non-store online retail dataset with InvoiceNo, Stockcode, Description, Quantity, InvvoiceDate, UnitPrice, CustomerID and Country as the variables, in which as the first step, we have started with Exploratory Data Ananysis followed by the data cleaning. In data cleaning we remove the duplicate rows. Remove the redundant values which are negatives and zeros from the UnitePrice and quantity Vriables. After that we remove the Null value from CustomerID column. 

Further,  we check the country-wise distribution of the customers and checked which are the top five items have been sold in UK because most of the customers are from Uk.

After that we start with RFM anylysis which is Recency, frequency, Monetary analysis help us to segregate the customers based on the score given  to the each customer in these segments. Recency score tells us how recently a customer has made a purchase, Frequency tells us how often a customer makes a purchase and Monetary Value tells us how much money a customer spends on purchases.

After that we scaled the data using standarscaler and the apply the KMeans clusturig model. To find the good K value we uses the Elbow method and to calculate the goodness of the clustring we use the Silhouette score. Here our experimets has ended and the conclusion we got is as follows:

The best no. of clustures we found using Ellbow methos is 5 and basis on that we segmented the cutomers in 5 groups (Group no. 0 to 4)

Group 0 has high Recency but Low Frequency and Low Monetary means they come recently but they are not frequent or they do not spend more.

Group 4 has high Monetary and high Frequency customers spend the most and they are also frequent
