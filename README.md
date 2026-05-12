# Air Quality Index Analysis (2015-2025)

**Student Name:** Qamar Abbas Shahzad  
**Registration Number:** 2280163  

## Dataset
Global Urban Air Quality Index Dataset (2015-2025)  
- Source: Publicly available air quality dataset  
- Contains daily air quality measurements for multiple cities worldwide.  
- After cleaning: 3,660 rows, 13 columns.

## Problem Statement
This project analyzes global air quality data from 2015 to 2025. The purpose is to understand AQI trends across cities and countries, identify important pollutants, classify AQI categories using basic supervised learning algorithms (KNN and Naive Bayes), and discover pollution patterns using unsupervised learning techniques (K-Means clustering and PCA).

## Tools & Libraries Used
- Python 3.x
- Pandas – data manipulation
- NumPy – numerical operations
- Matplotlib & Seaborn – data visualization
- Scikit-learn – machine learning (KNN, Naive Bayes, K-Means, PCA, preprocessing)
- Google Colab – Jupyter notebook environment

## How to Run the Notebook
1. Clone this repository to your local machine or open in Google Colab.
2. Ensure the file `global_air_quality_dataset.csv` is in the same directory as the notebook.
3. Open `IDS_ASSIGNMENT_3.ipynb` in Jupyter Notebook / JupyterLab / Google Colab.
4. Run all cells sequentially (from top to bottom).
5. The notebook will load the data, perform cleaning, create visualizations, train models, and show outputs.

## Summary of Main Findings
- **Data overview:** 3,660 records, no missing values or duplicates. Date converted and year/month extracted.
- **AQI distribution:** "Very Unhealthy" is the most frequent category (1,360 records), "Good" least (297 records).
- **Top polluted countries:** India, Japan, Brazil (average AQI = 168 each); highest single AQI = 300 (São Paulo, Brazil); lowest = 30 (Los Angeles, USA).
- **Supervised learning:** KNN best accuracy = 25.0% (k=7); Naive Bayes accuracy = 38.7% but predicted only the majority class. KNN is preferred for multi‑class prediction despite lower accuracy.
- **Unsupervised learning:** K-Means (k=3) produced three clusters with similar AQI (~164) but increasing PM2.5 (120 → 135), representing low, medium, and high particulate pollution.
- **PCA:** Explained only 23.6% of variance (PC1=12.0%, PC2=11.6%), indicating that two dimensions are insufficient to capture data complexity.

## Screenshots of Important Charts

![AQI Category Distribution](images/aqi_distribution.png)  
*Most records fall into "Very Unhealthy" category.*

![Top 10 Countries by Average AQI](images/top_countries.png)  
*India, Japan, Brazil share the highest average AQI (168).*

![AQI Trend by Year (2015-2025)](images/aqi_trend.png)  
*Flat trend – the dataset only contains 2024 data.*

![PM2.5 vs AQI Scatter Plot](images/pm25_vs_aqi.png)  
*Positive relationship between PM2.5 concentration and AQI.*

![Correlation Heatmap](images/correlation_heatmap.png)  
*Unusually weak correlations – possible data anomaly.*

![PCA – Colored by K-Means Clusters](images/pca_clusters.png)  
*Cluster 0 (low pollution) shows some separation.*

![PCA – Colored by True AQI Category](images/pca_true_category.png)  
*Poor linear separation confirms high‑dimensional complexity.*

## Report File Location
The full written report is available in this repository:  
[`IDS 3 Qamar.docx`](IDS 3 Qamar.docx)

## GitHub Repository
[https://github.com/qamarmanawari/AQI-Data-Science-Project](https://github.com/qamarmanawari/AQI-Data-Science-Project)
