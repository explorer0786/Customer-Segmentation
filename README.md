# Customer Segmentation

This project focuses on segmenting customers into distinct groups based on their behavior and characteristics, using two powerful clustering techniques. Customer segmentation helps businesses better understand their customers, personalize marketing strategies, and enhance customer experience.

## Problem Statement

XYZ.com is an e-commerce company based in Argentina. They have past order details which includes customer personal details like customer name, address, etc and order details like order quantity, sales, product code, etc. The company wants to understand if there is any pattern among these customers and use it for making more profit. They want to analyse the sales data, wrt to customers and identify high yield groups of customers.

Objective: We will use clustering techniques to identify the segment of customers. We will see if these groups are similar or different. We will analyse these groups and brainstorm about how this info can be utilised to make an informed business decision.

## 📊 Techniques Used

- **K-Means Clustering**
- **Hierarchical Clustering**

Both methods were applied and compared to identify meaningful patterns in customer data.

## 🛠️ Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Scipy

## 📈 Project Workflow

1. **Import Libraries**  
   - Imported necessary libraries for data manipulation, visualization, and modeling.

2. **Setting Options**  
   - Set environment options for better data display and visualization.

3. **Read Data**  
   - Loaded the dataset into the environment for analysis.

4. **Data Analysis and Preparation**  
   - **4.1 Data Types and Summary Statistics:** Understood the data structure and basic statistics.  
   - **4.2 Missing Values:** Checked for and handled missing values.  
   - **4.3 Data Cleansing and Univariate Analysis:** Cleaned the data and analyzed individual features.  
   - **4.4 Bivariate and Multivariate Analysis:** Explored relationships between different variables.  
   - **4.5 Data Preparation:** Scaled and prepared the data for clustering algorithms.

5. **K-Means Clustering**  
   - Applied K-Means clustering and determined the optimal number of clusters using the Elbow Method.  
   - Visualized and interpreted the resulting clusters.

6. **Hierarchical Clustering**  
   - Applied Hierarchical Clustering techniques.  
   - Generated dendrograms to find optimal cluster divisions and compared results with K-Means.

7. **Conclusion and Interpretation**  
   - Summarized findings, interpreted the customer segments, and discussed potential business strategies based on the clustering results.

## 📋 Conclusion and Interpretation

From K-means clustering, we are getting 6 clusters. Here, the cluster 0 and cluster 1 are much bigger than other 4 clusters. From the dendrogram, there seems to be two kinds of data. We can find 4 groups from the dendrogram if we remove the highly variable data which is merging towards the end of the agglomerative clustering model.

Cluster profiling based on K-means clustering. These results may vary based on the random state.

CLUSTER 0 (highest) - customers in this group buy items in high quantity. The sales amount is also on the higher side. The mean price of each item is close to 99. They are the highest buyers of products with high MSRP.

CLUSTER 1 (lowest) - This group represents customers who buy items in varying quantities ~30, they tend to low price items ~68. Their sales are ~ 2061, they buy products with lowest MSRP.

CLUSTER 2, 3, 4, 5 have quite similar properties. We need to analyze them deeper to understand their pattern of purchase.

   git clone https://github.com/your-username/customer-segmentation.git
