# Air Quality Index Analysis (2015-2025)

**Student Name:** Qamar Abbas Shahzad  
**Registration Number:** 2280163  

## Dataset
Global Urban Air Quality Index Dataset (2015-2025)  
- After cleaning: 3,660 rows, 13 columns.

## Problem Statement
This project analyzes global air quality data to understand AQI trends, identify important pollutants, classify AQI categories using KNN and Naive Bayes, and discover pollution patterns using K-Means and PCA.

## Tools & Libraries Used
Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, Google Colab

## How to Run
1. Clone this repository or open in Google Colab.
2. Ensure `global_air_quality_dataset.csv` is in the same directory.
3. Run `IDS_ASSIGNMENT_3.ipynb` sequentially.

## Summary of Main Findings
- **Data:** 3,660 records, no missing values, no duplicates.
- **AQI distribution:** Very Unhealthy (1,360), Moderate (673), Unhealthy (666), Unhealthy for Sensitive Groups (664), Good (297).
- **Top polluted countries:** India, Japan, Brazil (avg AQI = 168 each).
- **Highest AQI:** 300 (São Paulo, Brazil). **Lowest AQI:** 30 (Los Angeles, USA).
- **KNN best accuracy:** 25.0% (k=7).
- **Naive Bayes accuracy:** 38.7% (but only predicted majority class).
- **K-Means clusters:** 3 clusters with increasing PM2.5 (120 → 135).
- **PCA explained variance:** 23.6% (PC1=12.0%, PC2=11.6%).

## Report
[IDS 3 Qamar.docx](IDS 3 Qamar.docx)

## GitHub Repository
[https://github.com/qamarmanawari/AQI-Data-Science-Project](https://github.com/qamarmanawari/AQI-Data-Science-Project)
