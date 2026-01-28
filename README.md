# Geo-Temporal Insights from Twitter Data

This project analyzes approximately **14 million geotagged tweets** from Helwig et al. (2015) to examine spatial and temporal patterns of Twitter activity across the United States. The workflow includes large-scale data cleaning, aggregation, and visualization to quantify tweet intensity across longitude, latitude, and daily time windows.

A **Random Forest regression model** is used to estimate tweet counts per spatial–temporal grid cell, revealing strong geographic clustering (major urban corridors) and relatively stable day-to-day dynamics. Although limited to a seven-day sample and lacking textual context for topic-level analysis, the model serves as a baseline estimator for spatiotemporal tweet intensity and illustrates the challenges of short-horizon social signal prediction.

---

## Key Features

- Processing of **14M+ records** using `pandas` and `scikit-learn`
- Geo-temporal aggregation into **1° latitude–longitude grid cells**
- Daily tweet count modeling and spatial intensity visualization
- Out-of-sample performance: **RMSE ≈ 20% of mean counts**, **R² ≈ 0.99**
- Discussion of modeling limitations (event-driven surges, limited time window, lack of textual context)

---

## Data Source

Helwig, N., Gao, Y., Wang, S., & Ma, P. (2015).  
**Twitter Geospatial Data.** UCI Machine Learning Repository.  
https://doi.org/10.24432/C5RS5J
