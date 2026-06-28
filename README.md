# 🎯 Recruitment Channel Effectiveness Analytics

> Statistical analysis of recruitment sourcing channels using ANOVA, regression, and correlation to identify cost-efficient, high-quality hiring pathways.

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Statsmodels](https://img.shields.io/badge/Statsmodels-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-3776AB?style=for-the-badge&logo=python&logoColor=white)

---

## 📌 Overview

This project evaluates the effectiveness of multiple recruitment sourcing channels using a multi-metric analytical framework covering:

- **Cost-per-hire** — financial efficiency across channels
- **Yield ratio** — applicant-to-hire conversion at each funnel stage
- **Performance score** — post-hire quality of candidates by channel
- **Satisfaction score** — hiring manager and candidate experience ratings

Statistical techniques (ANOVA, regression, correlation) are applied to identify which channels deliver the best outcomes across all four dimensions simultaneously.

---

## 🏆 Key Results

| Analysis | Finding |
|----------|---------|
| ANOVA | Statistically significant differences in yield ratio across channels |
| Regression | Cost-per-hire and performance score are the strongest predictors of channel ROI |
| Correlation | High satisfaction scores correlate positively with lower time-to-fill |
| Top channel | Employee referrals scored highest on performance + satisfaction; lowest cost-per-hire |
| Weakest channel | Generic job boards: high volume, lowest yield ratio and performance scores |

---

## 🔍 Methodology

```
1. Data Preparation (SQL + Python)
   └── Cleaned recruitment records; standardised channel categories and metric definitions

2. Descriptive Analysis
   ├── Cost-per-hire distribution by channel (boxplots, summary statistics)
   ├── Funnel analysis: application → interview → offer → acceptance rates
   └── Performance and satisfaction score distributions

3. Statistical Testing
   ├── One-way ANOVA: test for significant differences across channel groups
   ├── Post-hoc Tukey HSD: identify which channel pairs differ significantly
   └── Pearson correlation matrix: relationships between all four metrics

4. Regression Modelling
   ├── OLS regression: predict hire quality (performance score) from channel + cost variables
   └── Feature importance: which channel attributes most predict downstream performance

5. Recommendations
   └── Channel ranking dashboard + ROI-adjusted sourcing strategy
```

---

## 📁 Repository Structure

```
recruitment-channel-analytics/
│
├── README.md
├── requirements.txt
│
├── scripts/
│   ├── 01_data_cleaning.py          # Data standardisation and feature engineering
│   ├── 02_descriptive_analysis.py   # EDA: distributions, funnel analysis, summaries
│   ├── 03_anova_testing.py          # One-way ANOVA + Tukey HSD post-hoc tests
│   ├── 04_regression.py             # OLS regression for performance prediction
│   └── sql_queries.sql              # SQL queries for data extraction
│
├── data/
│   └── README.md                    # Data description and schema
│
└── outputs/
    └── README.md                    # Charts and visualisation exports
```

---

## 🚀 Getting Started

### Prerequisites
```bash
pip install -r requirements.txt
```

### Run the Analysis
```bash
# Step 1: Clean data
python scripts/01_data_cleaning.py

# Step 2: Descriptive analysis
python scripts/02_descriptive_analysis.py

# Step 3: ANOVA and statistical tests
python scripts/03_anova_testing.py

# Step 4: Regression model
python scripts/04_regression.py
```

---

## 📊 Key Visualisations

- **Channel comparison matrix** — heatmap of all 4 metrics by sourcing channel
- **Funnel visualisation** — applicant-to-hire yield ratio per channel
- **ANOVA results plot** — group means with confidence intervals
- **Regression coefficients chart** — predictor importance for hire quality

---

## 💡 Business Implications

| Recommendation | Rationale |
|---------------|-----------|
| Increase employee referral budget | Highest performance + satisfaction, lowest cost |
| Reduce spend on generic job boards | High volume but lowest yield and post-hire quality |
| Invest in LinkedIn sourcing | Strong performance scores; moderate cost-per-hire |
| Measure satisfaction systematically | Significant predictor of time-to-fill and retention |

---

## 👩‍💻 About

Developed as **Portfolio Project 2** — part of an end-to-end analytics portfolio built during BS Analytics & Sustainability Studies at TISS Mumbai.

📫 [rupalrani2303@gmail.com](mailto:rupalrani2303@gmail.com) · [LinkedIn](https://www.linkedin.com/in/rupal-rani-a23b36257) · [GitHub](https://github.com/rupalrani)
