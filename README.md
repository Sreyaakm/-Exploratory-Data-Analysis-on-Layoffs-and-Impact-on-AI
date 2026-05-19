![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
![Google Colab](https://img.shields.io/badge/Google_Colab-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge&logo=matplotlib&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-4C72B0?style=for-the-badge&logo=python&logoColor=white)
![Plotly](https://img.shields.io/badge/Plotly-3F4F75?style=for-the-badge&logo=plotly&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge)

# Layoffs & Impact of AI — Exploratory Data Analysis

An end-to-end EDA project examining global workforce layoffs from 2020–2023 and the parallel rise of Artificial Intelligence — exploring how AI adoption, market growth, and job displacement are interconnected.

---

## Project Overview

This notebook investigates three interconnected questions:

1. **Where and when did layoffs hit hardest?** — across countries, industries, and company stages
2. **Which tech companies drove the most layoffs in 2022?** — sector-specific deep dive
3. **How has AI grown as layoffs surged?** — market value, software revenue, and organizational adoption trends

The analysis connects the dots between a workforce in disruption and the technology driving that disruption.

---

## Datasets

| Dataset | Description | Source |
|---|---|---|
| `W_layoffs.csv` | Global layoffs across industries (2020–2023) | Kaggle / public layoff trackers |
| `Tech_Layoffs_of_2022.csv` | Tech-sector-specific layoff data for 2022 | Kaggle |
| `AI50 2024.csv` | Forbes Top 50 AI Companies — funding, HQ, founding year | Forbes AI 50 (2024) |
| `The Rise Of Artificial Intelligence2.csv` | Year-over-year AI market metrics (revenue, market value, org adoption) | Statista / industry reports |

---

## Tools & Libraries

- **Data manipulation** — `pandas`, `numpy`
- **Static visualization** — `matplotlib`, `seaborn`
- **Interactive visualization** — `plotly.express`
- **Machine learning** — `scikit-learn` (Linear Regression, Random Forest, preprocessing utilities)
- **Environment** — Google Colab + Google Drive

---

## Notebook Structure

### Part 1 — Global Layoffs EDA (`W_layoffs.csv`)

**Data Cleaning**
- Missing value imputation (mean for numerical, mode for categorical columns)
- Date parsing and feature engineering (`year`, `month`, `day`)

**Visualizations**
- Top 5 and Bottom 5 countries by total layoffs (bar charts)
- Correlation heatmap of numeric features
- Industry breakdown — top 8 industries by layoff count (pie chart)
- Layoffs by company funding stage (count plot with mean line)
- Distribution of total layoffs (histogram + KDE)
- Filtered distribution for companies with >200 layoffs
- Average layoffs per year (line plot)
- Interactive scatter — layoffs by year and company (Plotly)
- Interactive bar — total layoffs by country (Plotly)
- Violin plot comparing 2021 vs. 2022 layoff distributions

---

### Part 2 — Tech Sector Layoffs 2022 (`Tech_Layoffs_of_2022.csv`)

**Analysis**
- Top 5 and Bottom 5 tech companies by layoffs
- Top 10 companies across combined dataset
- Month with the highest layoff count
- Founding year of the most affected companies
- Scatter plot of layoffs over time by company (interactive, Plotly)

---

### Part 3 — AI Industry EDA

**Top 50 AI Companies — Forbes 2024** (`AI50 2024.csv`)
- Companies by founding year
- Funding cleaned and normalized (non-numeric characters stripped)
- Top 10 companies by funding (bar chart)
- Top 10 headquarters cities by total funding (bar chart)
- Funding by headquarters — static and interactive scatter (Plotly)

**AI Market Growth** (`The Rise Of Artificial Intelligence2.csv`)
- Organizations planning to implement AI over time (line plot)
- AI software revenue vs. global AI market value trends (dual line plot)
- AI software revenue vs. estimated revenue increase from AI (scatter)

---

## Key Findings

- **Layoff peak**: The highest single-month layoffs occurred in **July 2022**, with a sharp acceleration visible from late 2021.
- **Geography**: The **United States** leads all countries in total layoffs, directly correlated with its position as the world's largest AI adopter.
- **Industries**: Technology, retail, and consumer sectors account for the majority of layoff events.
- **AI market**: AI software revenue grew consistently from 2018 through 2024, signaling deepening institutional reliance on automation.
- **Adoption surge**: The share of organizations planning to implement AI is projected to rise from ~40% to **58% by 2025**.
- **Top AI funding**: The leading Forbes AI 50 companies collectively secured over **$23 billion** in funding, predominantly headquartered in San Francisco and New York.
- **Skills gap**: While AI creates opportunities in data science and AI engineering, the barrier to entry is rising, leaving routine and repetitive-role workers most exposed.

---

## Conclusion

AI adoption and workforce displacement are two sides of the same coin. The data confirms a direct correlation between high AI adoption and elevated layoff counts — but also reveals a market creating entirely new categories of work. The central challenge is the **pace of reskilling** relative to the pace of automation. Proactive investment in workforce transition programs, education, and policy is essential to ensure equitable outcomes in an AI-driven economy.

---

## How to Run

1. Open the notebook in **Google Colab**
2. Mount your Google Drive:
   ```python
   from google.colab import drive
   drive.mount('/content/drive')
   ```
3. Place all four CSV datasets under `MyDrive/Colab Notebooks/`
4. Run cells top to bottom — no additional setup required

---

## Author

**Kuladeep Roy**  
M.S. Data Science & Analytics — Grand Valley State University  
[GitHub](https://github.com/kdeepr)
