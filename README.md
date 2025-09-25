# 📊 Healthcare Analytics: Chronic Disease Prevalence in Canada and Ontario

## Project Overview
This project provides a comprehensive exploratory data analysis (EDA) of chronic disease in Canada using the **Canadian Community Health Survey (CCHS) 2019-2020 dataset**.

The analysis is presented in two parts:

- **National-level report**: Examines the overall burden of ten chronic conditions, explores variations across key demographics (age, gender, income, province), and contrasts the patterns of mental versus physical health issues.  
- **Provincial deep-dive**: Uses Ontario as a case study to compare its disease prevalence against the national average and, more importantly, to identify the key drivers of health inequity within the province.

The goal is to translate complex health data into clear, actionable insights for healthcare planners, community organizations, and decision-makers.

---

## ❓ Key Research Questions
This analysis was guided by the following core questions:

1. What is the overall **national burden** of the most common chronic conditions in Canada?  
2. How do prevalence patterns differ for **mental vs. physical health conditions** across different age groups and genders?  
3. How does chronic disease prevalence vary by **province**, and which regions are most affected?  
4. Is Ontario's chronic condition burden significantly different from the **national average**?  
5. Within Ontario, what are the most significant drivers of health disparities, specifically looking at **age and income**?  

---

## 💡 Key Findings

### National-Level Insights
- **Age is the dominant factor in chronic disease.** The burden is overwhelmingly concentrated in older populations, with **83.7% of seniors (65+)** reporting at least one chronic condition, compared to just **19% of adolescents**.  
- **Mental health conditions peak in young adulthood.** Unlike physical ailments, the prevalence of mental health disorders is highest among young adults (**17.4% for ages 18-34**) and declines in older age groups.  
- **Women report significantly higher rates of mental illness.** Women are about **1.6 times more likely** to report a mood or anxiety disorder than men (**17.3% vs. 10.7%**).  
- **Significant regional variation exists.** The Atlantic provinces, particularly **Newfoundland & Labrador (57.6%)** and **Nova Scotia (56.7%)**, show the highest prevalence of chronic conditions in the country.  

### Ontario-Specific Insights
- **Ontario is not an outlier.** For all ten conditions studied, Ontario's overall prevalence closely mirrors the national average, with differences being less than one percentage point.  
- **Internal disparities are the real story.**  
  - **Age Gradient:** The prevalence of high blood pressure skyrockets from **0.1% among adolescents** to **52.4% among seniors**.  
  - **Income Gradient:** For musculoskeletal conditions, prevalence in the lowest-income groups (**~32%**) is nearly **double** that of the highest-income group (**17%**).  

**Conclusion:** While inter-provincial comparisons are interesting, the most critical health equity challenges lie in addressing the vast disparities driven by **age and income** within a province's own borders.  

---

## ⚙️ Data and Methodology

- **Data Source:** Canadian Community Health Survey (CCHS) 2019-2020.  
- **Population:** Canadians aged 12 and over.  
- **Analytical Approach:** The analysis uses survey weights to produce representative estimates. 95% confidence intervals are calculated using 1,000 bootstrap replicates. The primary measures of association are **Cramér's V**, **absolute differences**, and **relative risks**, with a de-emphasis on p-values to focus on practical significance.  

---

## 🛠️ Tools and Libraries

- **Python**: The core programming language used for the analysis.  
- **Pandas & NumPy**: For data manipulation and cleaning.  
- **Matplotlib & Seaborn**: For data visualization.  
- **Jupyter Notebook**: As the interactive development environment.  

---

## 🗂️ Repository Structure

```
Healthcare-Analytics-Project/
│
├── notebooks/
│ ├── 01_CCHS_ChronicConditions_Stratification.ipynb
│ ├── 02_CCHS_National_Inferential_Stats.ipynb
│ └── 03_CCHS_Practical_Significance.ipynb
│
├── reports/
│ ├── Canada_ChronicConditions_Report_WithNotes_2019-2020.pdf
│ ├── Canada_ChronicConditions_LiteratureReview_2025.pdf
│ ├── Ontario_ChronicConditions_Report_2019-2020.pdf
│ └── Ontario_ChronicConditions_LiteratureReview_2025.pdf
│
└── README.md
```
---

## 🚀 How to Run

1. Clone this repository to your local machine.  
2. Install the necessary packages from the requirements.txt file:  

```bash
pip install -r requirements.txt
```

3. Launch Jupyter Notebook and open the analysis file:  

```bash
jupyter notebook
```

---

## 👤 Author

**Arun Acharya**
