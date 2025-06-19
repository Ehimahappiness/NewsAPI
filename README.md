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
✔ Top sources contribute `60%` of content (long-tail distribution)  

🚀 Business Value
Enables data-driven decisions for:

Optimal publication scheduling
Headline length targeting
Source partnership strategies
Engagement prediction models

# Setup & Usage

# 1. Install requirements
pip install -r requirements.txt

# 2. Configure API key
echo "NEWS_API_KEY= 4c5acc6d462e409b9ebd8c1f62d3176d" > .env

# 3. Run analysis
python news_engagement_analysis.py

## Code Features
```python
🔍 Key Features:
- Automated NewsAPI data pipeline (real-time & historical)
- Publication time optimization (morning vs. evening A/B test)
- Headline length analysis for engagement maximization with np.random.normal()
- Statistical validation with SciPy (p-value calculation)
- Interactive visualizations (Seaborn/Matplotlib)
- Outlier detection and data cleaning workflows

📈 Sample Output
<img width="615" alt="Screenshot 2025-06-18 at 01 43 35" src="https://github.com/user-attachments/assets/f17b34d8-ad35-4b3a-9289-0ca6ad4d6c49" />

<img width="600" alt="Screenshot 2025-06-18 at 02 11 01" src="https://github.com/user-attachments/assets/7627ee66-b8b4-4684-8bdf-6be8a3e0c72f" />

<img width="758" alt="Screenshot 2025-06-18 at 10 49 18" src="https://github.com/user-attachments/assets/421383d6-6c64-4159-ae8a-839623c8fe68" />

<img width="1101" alt="Screenshot 2025-06-19 at 09 44 24" src="https://github.com/user-attachments/assets/4d44ece5-63b9-484e-9ea4-a333bfbf14d7" />

