#  Simulating an A/B test from a NewsAPI
NewsAPI is a REST API that delivers real-time and historical news headlines from global sources in JSON format.
# News Article Engagement Analysis

📊 **A/B Testing & Performance Insights** using NewsAPI data  

## Project Overview
This analysis examines how **publication timing** (morning vs. evening) and **headline attributes** affect article engagement. Key features:

- **A/B Testing**: Statistical comparison of engagement metrics (`scipy.stats.ttest_ind`)
- **Time Analysis**: Optimal posting hours identification  
- **Content Insights**: Headline length distributions and source contributions  
- **Automated Cleaning**: Handles missing data and outliers  

## Key Findings
✔ **Morning posts** (6AM-12PM) drive `150.31` higher engagement (*p < 0.05*)  
✔ **8–12 word headlines** dominate high-performing articles  
✔ Top sources contribute `20%` of content (long-tail distribution)  

## Code Features
```python
# Highlights:
1. Automated data cleaning (datetime conversion, NA handling)
2. Engagement simulation with np.random.normal()
3. Dynamic visualization (Seaborn/Matplotlib)
4. Statistical testing with confidence intervals
