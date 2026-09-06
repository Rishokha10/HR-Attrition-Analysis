# HR-Attrition-Analysis

Data analysis project exploring employee attrition using Python, SQL, and Power BI — includes data cleaning, EDA, and key retention insights from the IBM HR Analytics dataset.

## 📊 Overview

This project analyzes why employees leave a company, using the IBM HR Analytics Employee Attrition dataset. The goal was to identify the strongest drivers of attrition and turn them into clear, business-relevant recommendations.

**Dataset:** [IBM HR Analytics Employee Attrition & Performance](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset) (Kaggle) — 1,470 employee records, 35 features.

## 🛠️ Tools Used

- **Python** (Pandas, NumPy, Matplotlib, Seaborn) — data cleaning and exploratory data analysis
- **SQL** — querying and aggregation practice on the dataset
- **Power BI** — interactive dashboard for stakeholder-facing reporting

## 🔍 Key Findings

| Finding | Detail |
|---|---|
| Overall attrition rate | **16.12%** (237 of 1,470 employees) |
| Highest attrition department | **Sales — 20.6%** |
| Lowest attrition department | Research & Development — 13.8% |
| Overtime impact | Employees working overtime attrit at **30.5%**, vs. **10.4%** for those who don't |
| Tenure risk | 0–2 year employees attrit at **28.9%**, vs. **8.1%** for 10+ year employees |
| Income gap | Employees who left earned **$4,787/month** on average, vs. **$6,833/month** for those who stayed |
| Highest-risk combined group | **Sales employees working overtime — 37.5%** attrition |

**Top recommendation:** HR should prioritize retention efforts on early-tenure employees and overtime workers, particularly within the Sales department, since these factors compound to create the highest attrition risk in the organization.

## 📁 Project Structure

```
HR-Attrition-Analysis/
├── data/
│   ├── WA_Fn-UseC_-HR-Employee-Attrition.csv   # Raw dataset (from Kaggle)
│   └── HR_Attrition_Cleaned.csv                # Cleaned dataset (used for analysis & Power BI)
├── HR_ATTRITION_ANALYSIS_.ipynb                 # Full Python notebook: cleaning + EDA
├── 1_univariate_bivariate.png                   # EDA chart: department, overtime, income, age, satisfaction, tenure
├── 2_correlation_heatmap.png                    # Correlation of all numeric features with attrition
├── 3_multivariate_dept_overtime.png             # Department × Overtime combined attrition rates
├── 4_multivariate_joblevel_gender.png           # Job Level × Gender combined attrition rates
├── 5_engineered_satisfaction.png                # Combined satisfaction score vs attrition
└── README.md
```

## 🚀 How to Run

1. Clone this repository or download the `.ipynb` file
2. Open it in [Google Colab](https://colab.research.google.com/) or Jupyter Notebook
3. Upload `WA_Fn-UseC_-HR-Employee-Attrition.csv` when prompted (or update the file path if running locally)
4. Run all cells (`Runtime → Run all` in Colab)

## 📈 Analysis Approach

Each analysis in the notebook follows a **Business Question → Analysis → Insight → Recommendation** structure, rather than generating charts without context. For example:

> **Question:** Does working overtime increase the likelihood of leaving?
> **Insight:** Employees who work overtime leave at 30.5%, nearly 3x the rate of those who don't.
> **Recommendation:** Review workload distribution for employees who consistently work overtime.

## 📌 Next Steps

- SQL queries exploring the same dataset (joins, aggregation, filtering)
- Interactive Power BI dashboard with KPIs and DAX measures for stakeholder reporting

## 👤 About

This project was built as part of a data analyst portfolio, demonstrating skills in data cleaning, exploratory data analysis, SQL, and business insight generation using Python and Power BI.
