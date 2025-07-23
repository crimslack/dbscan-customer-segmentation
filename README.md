# Customer Segmentation using DBSCAN

This project applies the DBSCAN clustering algorithm to segment customers based on their behavior using the [Customer Personality Analysis Dataset](https://www.kaggle.com/datasets/imakash3011/customer-personality-analysis).

## 📁 Dataset

- `marketing_campaign.csv` (tab-separated file)
- Contains customer demographics, product purchases, and behavior.

## 🎯 Objective

To identify distinct customer segments based on:
- Income  
- Wine spending  
- Meat product spending  
- Number of web purchases  
- Recency of last purchase

## 🧠 Methodology

1. **Data Cleaning**  
   Removed rows with missing income values.

2. **Feature Selection**  
   Selected 5 numerical features for clustering.

3. **Scaling**  
   Standardized the features using `StandardScaler`.

4. **KNN Distance Plot**  
   Used to determine optimal `eps` value for DBSCAN.

5. **DBSCAN Clustering**  
   Applied with `eps=1.4`, `min_samples=5`.

6. **PCA Visualization**  
   Reduced dimensions to 2D for cluster visualization.

7. **Evaluation Metrics**  
   - Silhouette Score  
   - Davies-Bouldin Index  
   - Calinski-Harabasz Score  
   (Metrics only calculated when more than 1 cluster is formed.)

## 📈 Outputs

- `outputs/pca_plot.png`  
- `outputs/knn_distance_plot.png`

## 🧪 Requirements

```bash
pip install -r requirements.txt

🛠️ Technologies Used
Python 3

pandas, numpy, matplotlib, scikit-learn
