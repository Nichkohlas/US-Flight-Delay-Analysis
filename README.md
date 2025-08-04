# US Flight Delay Analysis

As part of my **Programming for Data Science** coursework, this project analyzes US domestic flight data from the Havard Dataverse to answer key questions around flight delays and diversions.

This project was conducted in both **Python** and **R**, validating findings across both languages.

---

## Project Overview

The dataset contains flight arrival and departure details for all commercial flights on major carriers within the USA from **Oct 1987 to Apr 2008**, containing nearly **120 million records** (~1.6GB Compressed, ~12GB Uncompressed). 
To maximize analysis efficiency, I established a connection to an **SQLite Database** and used data from **10 consecutive years (1997-2006)** resulting in nearly **60 million** records for this analysis.

This project addresses 3 key questions:
1. **What are the best times and days to minimize flight delays each year?**  
2. **Do older aircraft experience more delays over time?**  
3. **Can we build a logistic regression model to predict the probability of flight diversions?**

---

## Key Features

- **Exploratory Analysis:** Trends by day-of-week, time-of-day, and seasonality for delay minimization.
- **Aircraft Age Analysis:** Investigated whether older aircraft are correlated with increased delays.
- **Predictive Modeling:** Built a **logistic regression model** to predict flight diversion probability.
- **Cross-Language Validation:** Implemented in **both Python and R** for reproducibility.

---

## Results

### 1. What are the best times and days to minimize flight delays?
- Boxplots of Average Delays:
  -  **Friday** (Day 5) consistently had the **highest Average Delays** across all seven days.
- Heatmaps of Average Delays cross the 10 years reveal a consistent pattern:
  - **Highest Delays:** Late-night/ Early-morning flights (00:00 - 04:00) experienced the longest delays.
  - **Lowest Delays:** Mid-morning to Early afternoon (08:00 - 14:00) experienced the shortest delays.

- These patterns remained consistent across all years, making mid-morning, mid-week flights the most reliable for minimizing delays.

![Heatmap analysis of time of day]()  

*Heatmap of Average Delays by Time of Week (Python and R implementation)* 

![Boxplot analysis of day of week]()  

*Boxplot of Average Delays across Day of Week (Python and R implementation)*

