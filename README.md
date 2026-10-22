<!-- Animated header -->

<h1 align="center">
  🚀 Exploring Trends: Terrorism report dashboard and YouTube streamer analysis
</h1>

## Terrorism report dashboard: A dynamic data visualisation of terrorism trends around the world

This terrorism report is a visually engaging analytical report designed to explore terrorist attacks around the world between 1970 and 2017. It highlights the types, frequency, and geographical distribution of these attacks, providing insights into global terrorism trends over time. The report can be used by researchers, policymakers, security analysts, and the general public to identify patterns, understand regional differences, and gain a better understanding of the evolution of terrorism worldwide.

### Tech and Data
- 📊 Power BI Desktop: For data visualisation and report creation.
- 📂 Power Query: For data transformation and cleaning
  
- 📁 Data Source: The Global Terrorism Database (GTD) on Kaggle: https://www.kaggle.com/datasets/START-UMD/gtd

### Key Findings
![Dashboard snapshot](https://github.com/OreoDebi/InternCareer/blob/main/Snapshot%20of%20terrorism%20report.png)

- A climb in terrorism attacks, peaking in the year 2014 with 16694 attacks (Line Chart).
- Most attacked group: The private citizens and property
- Most attacked regions (Horizontal bar chart): Middle East & North Africa and South Asia
- Most attacked country: Iraq
- Most successful attack types (Pie chart): Bombing/Explosion and Armed Assault
- Most successful attack weapons (Pie chart): Explosives and firearms.

**Report implications:** These findings highlight the importance of counterterrorism efforts that protect civilians, address regional instability, and promote international collaboration against terrorist attacks.

##
## YouTube Streamers: Exploratory data analysis

A Jupyter notebook that explores the Top 1000 YouTubers dataset to uncover patterns in categories, audiences, and engagement, and builds a simple streamer recommender.

### Tech and Data
- ![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white) Python and ![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter) Jupyter
- ![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas) Pandas: For data transformation and cleaning.
- ![Seaborn](https://img.shields.io/badge/Seaborn-4EAEAA?logo=python&logoColor=fff) Seaborn and ![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge) Mathplotlib: For data visualisation.
  
- 📁 Data Source: Top 1000 Youtubers statistics can be found on Kaggle: [https://www.kaggle.com/datasets/START-UMD/gtd](https://www.kaggle.com/datasets/computingvictor/top1000youtubers)

| Column | Description |
|---|---|
| Rank | Rank by subscribers |
| Username | Channel name |
| Categories | Content categories (Spanish labels, some missing) |
| Suscribers | Subscriber count (spelling as in source) |
| Country | Channel country |
| Visits | Visit count |
| Likes | Like count |
| Comments | Comment count |
| Links | Channel URL |

### Contents

1. 🕵️ **Data exploration**: loads data (1000 rows, 9 columns), checks structure, missing values (306 in `Categories`), duplicates, and summary statistics.
2. 📈 **Outlier check**: boxplots of subscribers, visits, likes, and comments. Outliers are expected and are therefore retained.
3. 📊 **Trend, audience and metrics analysis**:
   - Streamer counts per category (top: *Música y baile*, 160 streamers).
   - Category-by-country subscriber heatmap (strongest in the United States and India).
   - Average metrics and a correlation matrix (visits and likes are strongly correlated, ~0.95).
   - Rank vs. metrics scatterplots (rank follows subscribers, not engagement).
   - A list of channels above average on all four metrics.
4. 🔓 **Recommendations**: item-item collaborative filtering using correlations between streamers' performance metrics, demonstrated with `MrBeast2`.

### Potential additions
🤔 The recommender created is very simple. Including categories would potentially improve the recommendation to reflect content.
