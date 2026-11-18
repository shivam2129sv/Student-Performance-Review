# 🎓 Student Performance Analysis

An exploratory data analysis project focused on understanding students' academic performance and identifying the factors that influence their scores in Mathematics, Reading, and Writing.

The project analyzes student demographics, parental education, lunch types, and test preparation to uncover meaningful patterns and identify students who may need additional academic support.

## 📌 Project Overview

This project uses a dataset of **1,000 students** to investigate the relationship between academic performance and various socioeconomic and educational factors.

The analysis explores how different backgrounds and preparation levels relate to students' examination results, with the goal of generating actionable insights for educators and school administrators.

## 🎯 Project Objectives

- Analyze student performance across three academic subjects.
- Explore the relationship between parental education and student scores.
- Understand the impact of test preparation on academic performance.
- Compare performance across gender and ethnicity groups.
- Investigate the relationship between lunch type and academic outcomes.
- Identify students who may be academically at risk.
- Present findings through charts and a detailed report.

## 📂 Repository Structure

```text
Student-Performance-Review/
│
├── charts/
│
├── dataset/
│
├── Analysis_Summary.md
│
├── Principal_Report.docx
│
├── Principal_Report.pdf
│
├── LICENSE
│
└── README.md
```

## 📊 Dataset Overview

The dataset contains **1,000 records and 8 original columns**.

| Feature | Description |
|---|---|
| Gender | Student gender |
| Race/Ethnicity | Student ethnicity group |
| Parental Level of Education | Highest education level of parents |
| Lunch | Standard or free/reduced lunch |
| Test Preparation Course | Whether the student completed test preparation |
| Math Score | Mathematics examination score |
| Reading Score | Reading examination score |
| Writing Score | Writing examination score |

### Additional Features

Two additional features were created during analysis:

- **Total Score:** Sum of Mathematics, Reading, and Writing scores.
- **Average Score:** Average score across all three subjects.

## 🛠️ Analysis Performed

### 1. Data Exploration
- Examined dataset dimensions and column types.
- Checked for missing values and duplicate records.
- Explored categorical and numerical variables.
- Created additional performance metrics.

### 2. Academic Performance Analysis
- Compared average scores across subjects.
- Examined total score distributions.
- Identified differences in subject-wise performance.
- Studied correlations between academic subjects.

### 3. Factor Analysis
Investigated how different factors relate to student performance:

- Gender
- Parental education
- Race/Ethnicity
- Lunch type
- Test preparation course

### 4. Statistical Analysis
- Correlation analysis
- ANOVA testing
- Chi-square testing
- At-risk student analysis

## 🔍 Key Findings

Some important findings from the analysis:

**1. Overall Academic Performance**

| Subject | Average Score |
|---|---:|
| Mathematics | 66.1 |
| Reading | 69.2 |
| Writing | 68.1 |

- Overall average total score: 203.3 out of 300.
- Reading has the highest average score.
- Mathematics has the lowest average score.

**2. Impact of Test Preparation**

Students who completed test preparation performed better across all three subjects.

| Subject | Score Advantage |
|---|---:|
| Mathematics | +5.6 |
| Reading | +7.4 |
| Writing | +9.9 |

**3. Parental Education**

Students with parents holding higher educational qualifications generally achieved higher average scores.

- Master's degree: 73.6 average.
- High school: 63.1 average.

**4. Subject Correlations**

Strong positive relationships were observed between academic subjects:

- Reading & Writing: 0.955
- Mathematics & Reading: 0.818
- Mathematics & Writing: 0.803

**5. At-Risk
