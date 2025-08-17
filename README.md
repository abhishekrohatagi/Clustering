#  Customer Segmentation Project

##  Project Introduction
This project focuses on segmenting wholesale customers based on their **annual spending across multiple product categories** using **unsupervised machine learning techniques**.  
The objective is to identify distinct customer groups to help businesses:

- Design **targeted marketing strategies**
- Optimize **resource allocation**
- Better serve the **needs of different customer types**

---

##  Dataset Summary

The dataset contains annual spending (in Euros) of wholesale clients across six product categories:

| Feature            |
|--------------------|
| Fresh             |
| Milk              |
| Grocery           |
| Frozen            |
| Detergents_Paper  |
| Delicassen        |

>  All values were **normalized** before clustering.

---

##  Clustering Techniques Used

### 1. **K-Means Clustering**
- Optimal number of clusters determined using **silhouette scores**
- Final model used **3 clusters**
- Identified low, medium, and high spenders with different product preferences

### 2. **Hierarchical Clustering**
- Employed **dendrograms and heatmaps** for pattern validation
- **Z-score normalization** highlighted relative spending behavior

### 3. **DBSCAN**
- Tuned `eps` and `min_samples` to detect dense clusters and outliers
- Less effective here but useful for **outlier detection**

### 4. **Visualization**
- **Heatmaps**, **dendrograms**, and **clustermaps** gave intuitive representations of customer similarity
- Helped understand **feature importance** across clusters

### 5. **New Customer Prediction**
- Built a complete **prediction pipeline** to:
  - Scale new customer data
  - Assign segments using the trained **KMeans** model

---

##  Business Insights

| Cluster | Characteristics | Business Strategy |
|--------|------------------|-------------------|
| 0      | Low overall spenders | Upselling & promotions |
| 1      | High on *Fresh* and *Frozen* | Likely food-service businesses (e.g., restaurants) |
| 2      | High on *Milk*, *Grocery*, *Detergents_Paper* | Likely retailers or resellers |

**Conclusion:**  
Customer segmentation provides actionable insights to:
-  Improve marketing precision  
-  Enhance customer retention  
-  Personalize product recommendations

---

## Tech Stack & Libraries
- Python, NumPy, Pandas, Scikit-learn
- Seaborn, Matplotlib, Scipy

---

