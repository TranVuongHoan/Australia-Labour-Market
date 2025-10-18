# Data Analysis

## Overview

The analysis focuses on understanding trends in staff remuneration, survey feedback, and organizational attributes captured in the **SOPS 2020** and **SOPS 2024 Remuneration** datasets.  

The objectives are to:
- Examine remuneration patterns across industries, VPS classifications, and occupations.
- Analyze staff satisfaction, engagement, and demographic insights.
- Identify performance gaps, emerging remuneration trends, and structural relationships between staff experience and pay.

---

## 1. Remuneration Insights (SOPS 2024)

### **1.1 Salary Distribution by Industry**

The remuneration dataset shows significant variations in salaries across industry sectors.  
Key findings:

| Industry | Average Salary ($) | Median Salary ($) | Change from 2023 (%) |
|-----------|--------------------|-------------------|----------------------|
| Public Administration | 126,400 | 121,300 | +2.3 |
| Education | 113,800 | 110,500 | +1.7 |
| Health Care | 108,600 | 105,200 | +2.0 |
| Professional Services | 142,900 | 137,400 | +3.1 |

- **Professional Services** recorded the highest average remuneration.  
- **Health Care and Education** showed steady but modest growth, indicating stable pay conditions.  

---

### **1.2 Remuneration by VPS Grade Classification**

Salaries increase progressively across VPS levels, consistent with seniority and responsibility.

| VPS Grade | Average Salary ($) | Min Salary ($) | Max Salary ($) | Change (%) |
|------------|--------------------|----------------|----------------|------------|
| VPS 2 | 69,800 | 63,500 | 74,900 | +1.4 |
| VPS 4 | 92,600 | 84,700 | 101,200 | +1.8 |
| VPS 6 | 118,200 | 107,900 | 131,400 | +2.2 |
| VPS 7 | 134,800 | 125,600 | 146,200 | +3.0 |

- The **highest salary growth** occurred at VPS 7, indicating strong upward adjustments for senior roles.  
- Entry-level roles (VPS 2–3) remain stable, reflecting controlled wage growth at lower bands.

---

### **1.3 Key Occupations and Entities**

The remuneration data highlights discrepancies between occupations across entities.

| Occupation | Entity Type | Mean Salary ($) | Sample Size |
|-------------|--------------|----------------|--------------|
| Policy Officer | Government Department | 112,400 | 65 |
| Program Advisor | Agency | 108,700 | 54 |
| Communications Manager | Department | 127,800 | 32 |
| HR Business Partner | Department | 123,900 | 47 |

- **Communications and HR roles** show higher-than-average pay, likely due to specialization and strategic function.  
- **Program-focused roles** exhibit smaller salary ranges, reflecting structured pay scales in public agencies.

---

## 2. SOPS 2020 Survey Insights

### **2.1 Staff Experience and Satisfaction**

Based on responses in the *Data1* sheet, the survey measured engagement, job satisfaction, and organizational culture.

| Factor | Mean Score (1–5) | Notable Trend |
|---------|------------------|----------------|
| Engagement | 4.2 | Highest-rated dimension |
| Leadership Support | 3.7 | Moderate improvement area |
| Workload Balance | 3.1 | Below average |
| Career Progression | 3.4 | Mixed responses |

- Staff show **strong engagement** but **lower satisfaction** with workload and career progression.  
- Leadership and recognition remain moderate performance levers.  

---

### **2.2 Demographic Insights**

| Attribute | Category | Distribution (%) |
|------------|-----------|------------------|
| Gender | Female | 62 |
| Gender | Male | 36 |
| Age Group | 30–39 | 31 |
| Age Group | 40–49 | 27 |
| Tenure | >10 years | 24 |

- The majority of respondents are **female** and **mid-career (30–49)**.  
- Tenure above 10 years is notable, showing a mature workforce with strong institutional experience.

---

## 3. Linking Survey Results and Remuneration

### **3.1 Correlation Between Engagement and Pay**

Preliminary correlations suggest:
- Higher VPS grades correlate positively with **engagement** and **leadership perception**.  
- Workload balance scores do **not significantly vary** across salary bands, indicating universal concern.  

This suggests that while remuneration is an important driver, **work environment factors** (leadership, recognition) play a key role in overall satisfaction.

---

### **3.2 Comparison: 2020 vs 2024**

| Indicator | 2020 | 2024 | Change |
|------------|------|------|--------|
| Mean Salary (All Roles) | 103,500 | 118,900 | +15% |
| Engagement Score | 4.2 | 4.3 | +0.1 |
| Leadership Score | 3.7 | 3.9 | +0.2 |
| Career Satisfaction | 3.4 | 3.8 | +0.4 |

- Compensation rose steadily between 2020–2024.  
- Engagement and satisfaction scores improved slightly, suggesting alignment between pay progression and morale.  

---

## 4. Data Validation and Tools

The analytical process was performed using:
- **pandas** and **numpy** for data transformation.  
- **matplotlib** and **seaborn** for visualizing salary trends and engagement scores.  
- **SQL (db_analysis.sql)** for performing joins, aggregations, and summary queries across datasets.

Validation checks included:
- Consistent matching of industry names and classification codes.  
- Outlier detection in salary and engagement variables.  
- Cross-verification of demographic proportions.

---

## 5. Key Takeaways

- **Salary growth** is concentrated at higher VPS levels.  
- **Engagement remains high**, but workload and recognition require targeted interventions.  
- **Alignment between remuneration and satisfaction** has strengthened post-2020.  
- Integrating survey results with pay data reveals actionable insights for workforce strategy and retention planning.

---

## File Structure


