# User-Behavior-Analysis-Report
Analysis of the Correlation between University User Behavior Characteristics and Academic Output
# DATA2002 Student Performance and Academic Goal Association Analysis (Self-Project)

This project explores the relationships between student enrollment decisions (DATA2002 vs. DATA2902), historical academic performance (WAM), study effort (weekly study hours), and their self-set target grades for the **DATA2x02** course at the University of Sydney.

Report save in index.html

## 📋 Project Overview

The study utilizes statistical methods to analyze survey data, investigating whether academic ambition correlates with unit selection and whether past performance accurately predicts current goals and effort levels.

## 🔍 Research Questions

1.  **Unit Choice vs. Ambition**: Do students in the advanced stream (DATA2902) set higher grade targets compared to those in the standard stream (DATA2002)?
2.  **Historical Performance vs. Targets**: Is there a significant difference in historical WAM among students aiming for different grade levels (e.g., HD, D, Credit)?
3.  **Effort vs. Outcomes**: Is there a monotonic relationship between a student’s historical performance (WAM) and their current effort (weekly study hours)?

## 📊 Dataset Description

The analysis is based on student survey data, including the following key variables:
- `enrolled_unit`: The unit of study (DATA2002 or DATA2902).
- `target_grade`: The grade the student aims to achieve (ranging from High Distinction to Fail).
- `wam`: Weighted Average Mark representing past academic performance.
- `weekly_study_hours`: Number of hours spent studying per week.

## 🧪 Methodology & Results

### 1. Chi-squared Test of Independence
- **Objective**: Test the association between unit selection and target grade.
- **Findings**: DATA2902 students displayed higher academic ambitions, with **77.1%** aiming for an HD, compared to **52.12%** in DATA2002.

### 2. Analysis of Variance (ANOVA)
- **Objective**: Compare mean WAM across different target grade groups.
- **Results**: The test confirmed significant statistical differences in historical WAM between target grade groups. Generally, students with higher goals possessed higher past WAMs.

### 3. Permutation Test (Spearman Correlation)
- **Objective**: Analyze the relationship between WAM and weekly study hours.
- **Results**: 
    - **Spearman Correlation Coefficient**: 0.131 (weak positive correlation).
    - **P-value**: 0.01 (statistically significant).
    - **Conclusion**: Higher-performing students tend to dedicate slightly more time to their studies.

## 💡 Key Conclusions

- **Self-Selection Effect**: Students who opt for the more challenging advanced unit (DATA2902) typically set higher academic bars for themselves.
- **Consistency**: Past performance (WAM) is a strong reference point for the academic goals students set for future units.
- **Effort Link**: The study confirms a statistically significant positive link between prior academic performance and time investment.

## 🛠️ Tech Stack

- **Language**: R
- **Core Libraries**:
    - `tidyverse`: Data manipulation and cleaning.
    - `ggplot2`: Data visualization.
    - `infer`: Statistical inference and permutation testing.
    - `visdat`: Missing data visualization.

## 🚀 How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/KyrieChen3372/User-Behavior-Analysis-Report.git
  

2. Open the project in RStudio.

3. Install the required R packages:
    install.packages(c("tidyverse", "infer", "visdat", "ggplot2"))


4. Click the Knit button to generate the full HTML analysis report.
