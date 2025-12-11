# 📘 Introduction
* This project focuses on segmenting mall customers into different groups based on their Annual Income and Spending Score. Customer segmentation helps businesses understand various customer behaviors, enabling them   to create personalized marketing strategies that improve customer satisfaction and increase overall sales.

# 🎯 Objective 
* To identify meaningful customer groups using unsupervised machine learning.
* To analyze purchasing behavior based on income and spending score.
* To help businesses target the right customers with the right offers.
* To visualize clusters for easy interpretation and decision-making.

# 📊 Dataset Description
* The dataset contains 200 customer records with the following features:
* CustomerID – Unique ID (removed in preprocessing)
* Genre – Male / Female
* Age
* Annual Income (k$)
* Spending Score (1–100)
* The dataset is clean with no missing values

# ⭐ Key Insights from EDA
* Most customers fall in the middle-age range (20–50 years), showing a young-to-middle-aged customer base.
* Annual Income is mostly concentrated between 40k and 80k, indicating a strong middle-income segment.
* Spending Score shows a wide variation, meaning customers have very different purchasing behaviors.
* No strong correlation exists between Age, Income, and Spending Score, making them suitable for clustering.
* Scatterplots of Income vs Spending Score reveal natural cluster patterns, helpful for K-Means segmentation.

#  🛠 Libraries Used
* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn (StandardScaler, KMeans)

# 🤖 Model Used
* K-Means Clustering Algorithm
* Number of clusters (k) = 5
* Initialization = k-means++
* Trained on scaled data for accurate distance calculation.

# 📈 Results / Evaluation
* Silhouette Score = 0.55
* Indicates good clustering quality
* Clusters are clearly separated and meaningful
* Customer Segments Identified
* Cluster 0: Average income, average spending
* Cluster 1: High income, high spending (Premium customers)
* Cluster 2: Low income, high spending (Enthusiastic shoppers)
* Cluster 3: Low income, low spending (Budget customers)
* Cluster 4: High income, low spending (Careful spenders)

# 🔄 Project Workflow / Steps
* 1. Load the dataset
* 2. Perform EDA (Histograms, KDE, Scatterplots, Pairplots, Heatmap)
* 3. Preprocessing
   * Remove CustomerID
   * Encode Genre
   * Select features (Income, Spending Score)
   * Scale features using StandardScaler
* 4. Use Elbow Method to find optimal number of clusters
 * 5. Build K-Means model with k = 5
* 6. Assign clusters to each customer
* 7. Visualize clusters using scatter plots
 * 8. Evaluate model using Silhouette Score
 * 9.  Interpret clusters and derive business insights
  
  # ▶️ How to Run the Project
 * Install dependencies:
 * pip install pandas numpy matplotlib seaborn scikit-learn
 * Download the dataset and place it in your project folder.
 * Run the Python script or Jupyter Notebook:

   # 🏁 Conclusion

 * The customer segmentation model clearly identifies different customer groups and their purchasing patterns. These insights help businesses build personalized marketing strategies, enhance customer satisfaction, and boost revenue. By understanding each segment’s behavior, companies can make smarter decisions and deliver targeted offers effectively.
