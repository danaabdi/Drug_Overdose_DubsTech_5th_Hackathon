
# 💊 Drug Overdose in the USA — DubsTech 5th Datathon

## 👥 Team: Hire Me Now
- **Dana Abdirakhym** — ML Lead ([LinkedIn](https://www.linkedin.com/in/danabdirakhym/))  

## 🧠 Project Overview

In this project, we analyzed overdose death trends across demographics in the United States to identify high-risk groups and evaluate policy effectiveness using machine learning and visualization tools.

This project was submitted to the **5th DubsTech Datathon** and focused on both exploratory data analysis and predictive modeling.

---

## 📊 Agenda

1. Background Knowledge  
2. Data Cleaning  
3. Data Visualization  
4. Machine Learning Model

---

## 🔍 Background

- Drug overdoses are a significant public health issue.
- Synthetic opioids (e.g., Fentanyl, Carfentanil) are particularly lethal — Carfentanil is **100x stronger than Fentanyl** and **5000x more lethal than Heroin**.
- In 2017, China regulated Carfentanil, which had a visible impact on U.S. overdose trends.

**Sources:**  
[DEA Report](https://www.dea.gov/press-releases/2016/09/22/dea-issues-carfentanil-warning-police-and-public)  
[NIH Analysis](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC8019064/)

---

## 🧹 Data Cleaning Process

We cleaned and standardized fields such as:

- `Sex`, `Age`, `Race`, `Hispanic Origin`
- Re-mapped nested demographic values to simplified columns
- Created new numerical encodings for modeling: `AGE_NUM`, `YEAR_NUM`, `STUB_LABEL_NUM`, etc.
- Removed nulls and non-applicable demographic splits
- Ensured consistency for age-adjusted and crude rate formats

---

## 📈 Data Visualization

### Trends in Drug Overdose Death Rates:
- Deaths **fell for age groups 15–54** after 2017, but **continued to rise for 55–74**.
- Rates **declined across both sexes** after China's Carfentanil regulation in 2017.
- Deaths **continued rising across all races**, especially with synthetic opioids.

---

## 🤖 Machine Learning Model

We built a **Random Forest Regressor** to predict the estimated overdose death rate (`ESTIMATE`) using demographic and drug type features.

### 🔢 Model Performance

| Metric       | Training Set | Validation Set |
|--------------|--------------|----------------|
| **RMSE**     | 0.3903       | 0.3903         |
| **R² Score** | 0.9963       | 0.9963         |

> ✅ The model explained **99.6% of the variance** with **very low error** — indicating strong predictive accuracy.

### 🔍 Top 8 Features (by importance):

1. `PANEL_NUM`  
2. `AGE_NUM`  
3. `YEAR_NUM`  
4. `STUB_LABEL_NUM`  
5. `Sex_Male`  
6. `STUB_NAME_NUM`  
7. `Race_Hispanic_or_Latino`  
8. `UNIT_NUM`



---

## 🧠 Key Insights

- **Age** and **drug type** were the strongest predictors of overdose risk.
- **Race and gender** were less influential but still relevant.
- Public health regulation (e.g., Carfentanil ban) had measurable impacts across demographics.

---

## 📦 Files in this Repository

- cleaned_overdose_death_rates_updated.xlsx, final_overdose.xlsx, etc. — Cleaned datasets

- test_df_with_predictions.xlsx — Prediction results

- Drug_Overdose_Tableau.pdf — Tableau dashboard screenshots

- Pre_Process.pdf — Data preprocessing in R

- README.md — Project overview

- TEAM HIRE ME NOW HEALTH Drug Overdose Presentation — Final presentation

---

## Acknowledgments

Special thanks to DubsTech for organizing the datathon, and to all data providers for making this project possible.

---

> **Have questions or feedback?**  
> Reach out on [LinkedIn](https://www.linkedin.com/in/danabdirakhym/) or open an issue in this repo!
