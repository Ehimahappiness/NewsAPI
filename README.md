# News Article Engagement Analysis

NewsAPI is a REST API that delivers real-time and historical news headlines from global sources in JSON format.

📊 **A/B Testing & Performance Insights** using NewsAPI data

## Step 1: Import Libraries

```python
import requests
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
from scipy import stats
from datetime import datetime
import json
import warnings
warnings.filterwarnings('ignore')
```

## Step 2: Data Cleaning and Feature Engineering

* Convert `publishedAt` to datetime
* Extract hour
* Assign groups (Morning, Evening, Other)
* Calculate headline length (word count) and content length

## Step 3: Analysis and Visualization

* Engagement by group (boxplot, barplot with CI)
* Headline length distribution
* Publication hour distribution
* Source frequency

## Step 4: A/B Test (t-test)

## Step 5: Outlier Removal and Sensitivity Analysis

---

## Project Overview

This analysis examines how **publication timing** (morning vs. evening) and **headline attributes** affect article engagement. Key features:

* **A/B Testing**: Statistical comparison of engagement metrics (`scipy.stats.ttest_ind`)
* **Time Analysis**: Optimal posting hours identification
* **Content Insights**: Headline length distributions and source contributions
* **Automated Cleaning**: Handles missing data and outliers

## Key Findings

* **Morning posts** (6AM-12PM) drive `150.31` higher engagement (*p < 0.05*)
* **8–12 word headlines** dominate high-performing articles
* **Top sources contribute** `60%` of content (long-tail distribution)

## 🚀 Business Impact

Enables data-driven decisions for:

* Optimal publication scheduling
* Headline length targeting
* Source partnership strategies
* Engagement prediction models

## 🔍 Key Features

* Automated NewsAPI data pipeline (real-time & historical)
* Publication time optimization (morning vs. evening A/B test)
* Headline length analysis for engagement maximization with `np.random.normal()`
* Statistical validation with SciPy (p-value calculation)
* Interactive visualizations (Seaborn/Matplotlib)
* Outlier detection and data cleaning workflows

---

## Setup & Usage

### 1. Install requirements

```python
pip install -r requirements.txt
```

### 2. Configure API key

```python
echo "NEWS_API_KEY=4c5acc6d462e409b9ebd8c1f62d3176d" > .env
```

### 3. Run analysis

```python
NewsAPI_Engagement.ipynb
```

## 📈 Visual Output
```markdown
Engagement Overview
Headline Length Distribution
Source Frequency Chart
Time of Day Impact
```

<img width="615" alt="Screenshot 2025-06-18 at 01 43 35" src="https://github.com/user-attachments/assets/dc68bfc8-40bd-4386-b48b-92bad1e079f5" />

<img width="600" alt="Screenshot 2025-06-18 at 02 11 01" src="https://github.com/user-attachments/assets/962b11e0-5e47-484b-b7cf-837d1b911ae5" />

<img width="758" alt="Screenshot 2025-06-18 at 10 49 18" src="https://github.com/user-attachments/assets/acc02c84-9b98-4193-8071-a7c210dd6dfa" />

<img width="1101" alt="Screenshot 2025-06-19 at 09 44 24" src="https://github.com/user-attachments/assets/e4ea5df2-e463-4526-933e-c4602d288ac8" />
