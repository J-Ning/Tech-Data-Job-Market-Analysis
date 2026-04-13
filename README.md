# Tech & Data Job Market Analysis: Skills, Salaries, Remote Work, and Seniority Trends

## Overview

This project analyzes over 1.3 million LinkedIn tech and data job postings to understand which technical skills are most in demand and how they relate to salary, remote work, and seniority. The goal is to bridge the gap between the skills students learn and the skills employers actually seek.

Using Python, Pandas, NumPy, Matplotlib, and Seaborn, I cleaned and merged multiple large datasets, explored trends in the tech labor market, and prepared the data for future machine learning analysis.

---

## Research Questions

* Which technical skills are most demanded in tech and data jobs?
* How do salaries vary by experience level?
* Are remote jobs associated with different salaries or skills?
* What is the difference between senior and non-senior roles?
* Can technical skills help predict job outcomes such as salary or remote work?

---

## Datasets

### 1. LinkedIn Jobs and Skills 2024

Source: [https://www.kaggle.com/datasets/asaniczka/1-3m-linkedin-jobs-and-skills-2024](https://www.kaggle.com/datasets/asaniczka/1-3m-linkedin-jobs-and-skills-2024)

Contains:

* 1,348,454 LinkedIn job postings
* Job titles, company, location, experience level, and work type
* A separate skills dataset with associated job skills

### 2. Data Science Salaries 2024

Source: [https://www.kaggle.com/datasets/saurabhbadole/latest-data-science-job-salaries-2024](https://www.kaggle.com/datasets/saurabhbadole/latest-data-science-job-salaries-2024)

Contains:

* Salary in USD
* Experience level
* Remote work ratio
* Job title and company information

---

## Methods

1. Cleaned the LinkedIn postings dataset by removing unused columns.
2. Filtered the dataset to keep only tech and data-related roles such as:

   * Data Analyst
   * Data Scientist
   * Software Engineer
   * Data Engineer
   * Machine Learning Engineer
   * Backend Engineer
3. Merged the postings dataset with the skills dataset using the `job_link` column.
4. Parsed and normalized skill names to combine similar skills and remove duplicates.
5. Created exploratory visualizations for:

   * Salary distributions
   * Remote work trends
   * Senior vs non-senior roles
   * Most common job titles
   * Most common technical skills
6. Built binary features for the top 30 most common skills to prepare for future machine learning models.

---

## Key Findings

* Over half of all tech and data job postings were senior-level roles.
* The most common non-senior job titles were:

  1. Business Analyst
  2. Software Engineer
  3. Data Engineer
  4. Data Analyst
  5. Data Scientist
* Python and SQL appeared among the most common technical skills across job postings.
* Remote and hybrid jobs were common in technical fields, especially for higher-level roles.
* Salary generally increased with experience level.

---

## Example Visualizations

The project includes:

* Distribution of salaries
* Salary by experience level
* Remote work ratio distribution
* Salary vs remote work ratio
* Senior vs non-senior job postings
* Top 20 non-senior job titles
* Top 30 technical skills before and after cleaning

Example image files:

```text
plots/salary_distribution.png
plots/salary_by_experience.png
plots/remote_work_distribution.png
plots/senior_vs_nonsenior.png
plots/top20_nonsenior_titles.png
plots/skills_before_after_normalization.png
```

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Jupyter Notebook

---

## Repository Structure

```text
├── data/
│   ├── raw/
│   └── processed/
├── notebooks/
│   └── analysis.ipynb
├── plots/
├── README.md
└── requirements.txt
```

---

## Future Improvements

* Train machine learning models to predict salary or remote work from skills.
* Compare demand for skills across different cities or countries.
* Analyze trends over time to see which skills are becoming more important.
* Create an interactive dashboard using Streamlit or Tableau.

---

## Author

Jenny Fu
Mathematics–Computer Science, UC San Diego
Nishka Vaghela
Computer Science and Bioinformatics, UC San Diego
Renee Li 
Mathematics–Computer Science, UC San Diego
Niharika Sapre
Cognitive Science, UC San Diego
Eric Badilla
Mathematics–Computer Science, UC San Diego
