# Customer Segmentation Using K-Means Clustering

## 📌 Project Overview

This project focuses on customer segmentation using **unsupervised machine learning**. The **Mall Customers Dataset** was analyzed to identify meaningful customer groups based on demographic and purchasing-related characteristics.

The **K-Means clustering algorithm** was used to segment customers according to:

* Age
* Annual Income
* Spending Score

The resulting customer segments were analyzed to identify their characteristics and potential business applications.

---

## 🎯 Objectives

* Analyze customer demographic and purchasing data.
* Perform data preprocessing and feature scaling.
* Explore customer behavior through data visualization.
* Apply K-Means clustering.
* Determine a suitable number of clusters using the Elbow Method and Silhouette Score.
* Visualize customer segments.
* Interpret the characteristics of each segment.
* Identify potential business applications of customer segmentation.

---

## 📊 Dataset

**Dataset:** Mall Customers Dataset

The dataset contains **200 customer records** and 5 columns:

| Feature                | Description                           |
| ---------------------- | ------------------------------------- |
| CustomerID             | Unique customer identifier            |
| Genre                  | Customer gender                       |
| Age                    | Customer age                          |
| Annual Income (k$)     | Annual income in thousands of dollars |
| Spending Score (1-100) | Customer spending score               |

---

## 🛠️ Technologies Used

* Python
* Jupyter Notebook
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn

### Machine Learning Techniques

* StandardScaler
* K-Means Clustering
* Elbow Method
* Silhouette Score
* Principal Component Analysis (PCA)

---

## 🔧 Data Preprocessing

The following preprocessing steps were performed:

1. Checked dataset structure and data types.
2. Checked for missing values.
3. Checked for duplicate records.
4. Removed `CustomerID` from clustering features because it is an identifier and does not represent customer behavior.
5. Selected Age, Annual Income, and Spending Score as clustering features.
6. Standardized the numerical features using `StandardScaler`.

No missing values or duplicate records were found in the dataset.

The `Genre` feature was retained for demographic analysis but was not used as a primary clustering feature.

---

## 🔍 Exploratory Data Analysis

EDA was performed to understand customer demographics and purchasing behavior.

The analysis included:

* Customer distribution by Genre
* Age distribution
* Annual income distribution
* Spending score distribution
* Annual income vs spending score
* Correlation heatmap

---

## 🤖 Clustering

### K-Means Clustering

K-Means was selected because the selected features are numerical and customer similarity can be represented using distance after feature standardization.

Different values of K from **2 to 10** were evaluated.

### Elbow Method

The Elbow Method was used to examine changes in clustering inertia as the number of clusters increased.

### Silhouette Analysis

The Silhouette Score was calculated for K values from 2 to 10.

**Selected K = 6**

**Best Silhouette Score ≈ 0.4284**

Based on the highest Silhouette Score among the tested values, six clusters were selected for the final model.

---

## 📈 Final Customer Segments

| Cluster | Customers | Avg. Age | Avg. Income (k$) | Avg. Spending Score |
| ------- | --------: | -------: | ---------------: | ------------------: |
| 0       |        45 |    56.33 |            54.27 |               49.07 |
| 1       |        39 |    26.79 |            57.10 |               48.13 |
| 2       |        33 |    41.94 |            88.94 |               16.97 |
| 3       |        39 |    32.69 |            86.54 |               82.13 |
| 4       |        23 |    25.00 |            25.26 |               77.61 |
| 5       |        21 |    45.52 |            26.29 |               19.38 |

---

## 💡 Segment Insights

### Cluster 0

Older customers with moderate income and moderate spending behavior.

**Potential application:** Loyalty programs and retention-focused campaigns.

### Cluster 1

Younger customers with moderate income and moderate spending.

**Potential application:** Engagement campaigns and personalized promotions.

### Cluster 2

Higher-income customers with relatively low spending scores.

**Potential application:** Personalized incentives and campaigns aimed at increasing engagement.

### Cluster 3

Higher-income customers with high spending scores.

**Potential application:** Premium products, loyalty rewards, and personalized recommendations.

### Cluster 4

Younger customers with lower income but high spending scores.

**Potential application:** Affordable promotions, discounts, and engagement campaigns.

### Cluster 5

Older customers with lower income and low spending scores.

**Potential application:** Value-based offers and suitable retention strategies.

---

## 📊 Visualizations

The project includes:

* EDA visualizations
* Elbow Method plot
* Silhouette Score plot
* Cluster distribution
* Income vs Spending Score cluster visualization
* PCA visualization
* Cluster profile heatmap

---

## 🧠 Key Findings

The clustering analysis identified six customer segments with different combinations of age, annual income, and spending behavior.

The results demonstrate that customers with similar demographic and spending characteristics can be grouped together, providing a structured way to understand customer diversity.

These segments can potentially support targeted marketing, customer engagement, personalized recommendations, and retention strategies.

---

## ⚠️ Limitations

* The dataset contains only 200 customers.
* Behavioral information is limited.
* Detailed purchase history and product preferences are not available.
* K-Means can be sensitive to feature scaling and outliers.
* Business recommendations would require real-world testing to evaluate their effectiveness.

---

## 🚀 Future Improvements

Future versions of this project could include:

* Larger customer datasets
* Transaction history
* Purchase frequency
* Product preferences
* Customer lifetime value
* Comparison with DBSCAN and Hierarchical Clustering
* Interactive Streamlit dashboard
* Recommendation system based on customer segments

---

## 👩‍💻 Project Author

**Aiman Babar**

BS Bioinformatics Student
Interested in Data Science, Machine Learning, Bioinformatics and Computational Research.

---

## 📌 Project Type

**EncoderX Remote Internship – Batch 02**
**Week 03 – Data Science Task: Customer Segmentation**
