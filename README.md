Geo-Temporal Insights from Twitter Data
This project analyzes ~14 million geotagged tweets from Helwig et al. (2015) to explore spatial and temporal patterns of Twitter activity across the U.S. The workflow includes large-scale data cleaning, aggregation, and visualization to quantify tweet intensity by longitude, latitude, and time.

A Random-Forest regression model was implemented to estimate tweet counts per spatial-temporal cell, revealing strong geographic clustering (major urban corridors) and stable day-to-day dynamics. While limited to a seven-day sample window and lacking textual context for trending topics, the model serves as a baseline estimator for spatiotemporal tweet intensity and demonstrates practical challenges of short-horizon social-signal prediction.

Key features:
• Processing of > 14 M records with pandas and scikit-learn
• Geo-temporal aggregation into 1° grids and daily counts
• Visualization of spatial intensity and error distribution
• RMSE ≈ 20 % relative to mean counts, R² ≈ 0.99 on out-of-sample day
• Discussion of limitations (e.g., event-driven surges, data scope).

Helwig, N., Gao, Y., Wang, S., & Ma, P. (2015). Twitter Geospatial Data [Dataset]. UCI Machine Learning Repository. https://doi.org/10.24432/C5RS5J.
