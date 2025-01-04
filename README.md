# Clustering Analysis on the Bank Marketing Dataset

## Project Overview
This project performs clustering analysis on the Bank Marketing Dataset by applying and comparing two clustering algorithms:
- **K-Means Clustering** 
- **Hierarchical Clustering** (Single Linkage and Average Linkage)

The primary goal is to segment the data and identify potential patterns within the dataset by clustering customers based on their characteristics. This unsupervised learning task excludes the target variable since clustering does not rely on labeled data.

---

## Dataset Information
- **Dataset**: Bank Marketing Dataset
- **Size**: 45,211 rows and 17 columns
- **Features**: Contains a mix of categorical and numerical attributes representing customer information and banking activities.
- **Target Variable**: The target variable `y` (indicating subscription to term deposits) is excluded for clustering.

---

## Key Steps in Analysis
1. **Data Preprocessing**:
   - **Encoding Categorical Variables**: One-Hot Encoding is used to transform categorical features into numerical form.
   - **Scaling Numerical Data**: StandardScaler is applied to normalize numerical features to ensure consistent scaling for clustering.
   - **Combining Processed Data**: Encoded categorical data and scaled numerical data are merged to form a final dataset with 42 features.

2. **K-Means Clustering**:
   - **Elbow Method**: The optimal number of clusters is determined using the Elbow Method. 
   - **Clustering**: K-Means is applied with the chosen value of `K=3`.

3. **Hierarchical Clustering**:
   - **Agglomerative Clustering**: Hierarchical clustering is performed using both Single Linkage and Average Linkage.
   - **Dendrogram Visualization**: Dendrograms visualize cluster formation and help in understanding cluster hierarchy.

4. **Performance Evaluation**:
   - **Silhouette Score**: The clustering quality is evaluated by comparing the Silhouette Scores for K-Means and Hierarchical Clustering methods.

---

## Results and Visualizations
- **Elbow Method**: K = 3 was chosen as the optimal cluster number for K-Means Clustering.
- **Silhouette Scores**:
   - K-Means: `0.1047`
   - Hierarchical (Single Linkage): `0.779`
   - Hierarchical (Average Linkage): `0.766`
- **Visualizations**:
   - Scatter plots visualize the distribution of clusters using two key variables (`balance` and `age`).

---

## Tools and Libraries Used
- **Python** 
- **Pandas** – Data manipulation and analysis
- **Scikit-Learn** – Clustering algorithms, preprocessing, and evaluation
- **Matplotlib/Seaborn** – Visualization of clustering results
- **Scipy** – Hierarchical clustering and dendrogram plotting

---

## How to Run the Code
1. Clone the repository:
   ```bash
   git clone https://github.com/username/repositoryname.git
