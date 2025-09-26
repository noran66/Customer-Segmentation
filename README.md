# 🛒 Customer Segmentation – Elevvo Internship

For the second internship task, I worked on **customer segmentation** using clustering techniques.  
The goal was to group mall customers into segments based on their **Age, Annual Income, and Spending Score**.  

---

## ✅ Steps
- Data preprocessing:  
  - Dropped `CustomerID` (not useful).  
  - Encoded categorical column `Gender`.  
  - Selected features (`Age`, `Annual Income`, `Spending Score`).  
  - Applied feature scaling with `StandardScaler`.  
- Used the **Elbow Method** to determine the optimal number of clusters.  
- Applied **KMeans Clustering** with k=5 (chosen from elbow method).  
- Visualized customer groups using scatter plots.  
- Calculated **average spending & income per cluster**.  
- **Bonus**: Applied **DBSCAN** for density-based clustering and outlier detection.  

---

## 📊 Results
### KMeans (k=5) Cluster Averages
| Cluster | Avg Income (k$) | Avg Spending | Insights |
|---------|-----------------|--------------|----------|
| 0 | 47.6 | 41.7 | Moderate income & moderate spending |
| 1 | 86.1 | 81.5 | **High income & high spenders** 💎 |
| 2 | 26.1 | 74.8 | Low income & high spenders |
| 3 | 54.3 | 40.9 | Moderate income & low spenders |
| 4 | 89.8 | 18.5 | High income & low spenders |

---

## 🔎 Insights
- **Cluster 1** are the most profitable customers (high income + high spenders).  
- **Cluster 4** are wealthy but spend little → great potential for targeted campaigns.  
- **Cluster 2** are engaged spenders but have lower income → might be sensitive to promotions.  
- **Clusters 0 & 3** represent average or budget-conscious customers.  
- DBSCAN highlighted some outliers, showing its usefulness for noisy datasets.  

---

## ✅ Conclusion
Clustering allows businesses to better understand their customers and design **personalized marketing strategies**.  
KMeans worked well for segmenting groups, while DBSCAN provided additional insight into outliers.  

---

📂 **Full code + analysis is available on GitHub:**  
👉 [Customer Segmentation Repo](https://github.com/noran66/Customer-Segmentation.git)
