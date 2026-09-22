# Hospital-operations-service-financial-analytics
End-to-end healthcare analytics project analyzing hospital operations, patient satisfaction, waiting-time bottlenecks, revenue patterns, financial burden, and chronic-care trends using Python and data visualization.
Integrated Hospital Performance & Patient Insights

## End-to-End Healthcare Data Analytics Project

An end-to-end healthcare analytics project focused on understanding **patient behavior, hospital operations, patient experience, and financial performance** using integrated Patients, Visits, and Billing data.

The project uses Python-based data analysis and visualization to convert raw hospital records into actionable business insights for operational and management decision-making.

---

## Project Overview

Hospitals generate large volumes of data across patient registration, visits, departments, services, waiting times, satisfaction, billing, and payment activity.

This project integrates these data sources to answer key business questions such as:

- What does the hospital's patient population look like?
- Which departments handle the highest patient workload?
- Where are waiting-time bottlenecks occurring?
- How does waiting time relate to patient satisfaction?
- Which patient age groups generate the most visits?
- Which services and visit types contribute most to revenue?
- How do insurance and payment patterns affect patient financial burden?
- Where can data help improve operational efficiency and patient service?

---

## Business Objectives

### 1. Patient Insights
Understand patient demographics, age groups, chronic conditions, and visit patterns.

### 2. Operational Performance
Analyze department workload, patient flow, waiting times, visit types, and length of stay.

### 3. Patient Experience
Evaluate satisfaction levels and identify relationships between waiting time and patient satisfaction.

### 4. Financial Visibility
Analyze billing amounts, insurance coverage, patient payments, outstanding balances, and revenue patterns.

---

## Dataset

The project works with three related datasets:

| Dataset | Description |
|---|---|
| `patients.csv` | Patient demographics, city, insurance status, chronic conditions, BMI, and registration information |
| `visits.csv` | Visit date, department, diagnosis, visit type, waiting time, length of stay, and satisfaction |
| `billing.csv` | Bill amount, insurance coverage, patient payment, payment method, and payment status |

Initial dataset sizes:

- **Patients:** 4,010 records
- **Visits:** 12,015 records
- **Billing:** 12,015 records

After data preparation and deduplication, the final analytical dataset contains approximately **12,000 visits across 3,803 unique patients**.

---

## Analysis Workflow

The project follows a structured data analytics approach:

**Business Question → Data Preparation → Analysis → Visualization → Observation → Insight → Recommendation**

The objective is not only to create charts, but to understand what the results mean from a hospital management perspective.

---

## Key Analysis Areas

### Patient Demographics

The project examines:

- Age-group distribution
- Gender distribution
- City-wise patient distribution
- Chronic-condition patterns
- Patient visit frequency
- Returning vs. new patient behavior

### Department & Service Analysis

Department performance is analyzed using:

- Visit volume
- Visit type
- Department workload
- Waiting time
- Satisfaction
- Revenue contribution

The analysis shows that **General Medicine has the highest visit volume**, followed by Orthopedics and Cardiology.

---

## Waiting Time Analysis

Waiting time is one of the major operational focus areas of the project.

The analysis compares waiting times across departments and visit types to identify concentrated bottlenecks.

One important finding is that **Cardiology OPD has an average waiting time of around 60+ minutes**, making it one of the major waiting-time problem areas.

The department/service analysis also shows that waiting problems are not evenly distributed across the hospital and are concentrated in particular department–visit-type combinations.

### Business Insight

The results suggest that improving specific high-delay workflows may be more effective than applying the same operational solution across every department.

---

## Waiting Time vs Patient Satisfaction

The relationship between waiting time and patient satisfaction was examined using correlation and wait-band analysis.

### Key Finding

**Waiting time and satisfaction show a negative correlation of approximately -0.59.**

The analysis also shows satisfaction declining as waiting time increases:

| Waiting Time | Average Satisfaction |
|---|---:|
| Shortest wait band | 4.76 |
| Longest wait band | 4.03 |

### Insight

Longer waiting times are associated with lower patient satisfaction, and the pattern is visible across departments.

### Recommendation

Waiting time should be monitored as an important patient-experience KPI, with department-level tracking and attention to visits exceeding longer waiting thresholds.

---

## Revenue & Service Analysis

The project analyzes revenue by visit type to understand the relationship between hospital activity and financial contribution.

### Key Findings

- **Inpatient visits:** approximately 14% of visit volume but contribute around **62% of revenue**
- **OPD visits:** approximately 67% of visit volume but contribute around **25% of revenue**
- **Emergency visits:** approximately 19% of visit volume

Average bill values in the analysis:

| Visit Type | Average Bill |
|---|---:|
| Inpatient | ₹28,640.87 |
| Emergency | ₹4,723.14 |
| OPD | ₹2,397.32 |

The correlation between **length of stay and bill amount is approximately 0.86**, indicating a strong positive relationship in this dataset.

### Business Insight

Hospital volume and hospital revenue are distributed differently across service types. Inpatient activity contributes a much larger share of revenue relative to its visit volume.

---

## Patient Financial Burden

Insurance and payment behavior were analyzed to understand how financial responsibility is distributed across patients.

### Key Findings

- Approximately **32% of visits** are classified as Self Pay.
- **3,886 visits** fall under the Self Pay category.
- Self Pay patients bear approximately **99.9% of the billed amount out of pocket** in the analysis.
- Government Scheme patients have a substantially higher coverage contribution than Self Pay patients.

### Business Insight

The results highlight a significant financial-burden segment and indicate an opportunity to improve awareness and enrollment in available coverage schemes.

---

## Chronic Condition Analysis

The project examines how chronic conditions vary across age groups.

The analysis shows a strong age-related pattern:

- Around **69% of visits for patients under 18** have no recorded chronic condition.
- Only around **29% of visits for patients aged 60+** have no recorded chronic condition.
- Conditions such as **Hypertension, Diabetes, and Cardiac conditions** become more prominent with increasing age.
- The final analysis identifies chronic-condition involvement in approximately **65% of visits among patients aged 46+**.

### Business Insight

The increasing chronic-condition burden among older patient groups highlights the importance of age-focused chronic-care planning and preventive screening.

---

## Patient Experience Strengths

The analysis also identifies several positive patterns:

- Approximately **98.6% of patients rate their visit 4 or 5 out of 5**
- Pediatrics and Gynecology show strong satisfaction levels
- Satisfaction remains relatively consistent across analyzed cities
- Approximately **94.9% of visits are from returning patients**

These results indicate strong overall satisfaction and a high proportion of repeat hospital utilization.

---

## Key Insights Summary

| Business Area | Key Finding |
|---|---|
| Patient Volume | General Medicine handles the highest number of visits |
| Waiting Time | Cardiology has major waiting-time pressure, particularly OPD |
| Patient Satisfaction | Longer waiting time is associated with lower satisfaction |
| Revenue | Inpatient services generate a disproportionate share of revenue |
| Length of Stay | Strong positive relationship with bill amount |
| Financial Burden | Self Pay represents a significant out-of-pocket segment |
| Chronic Care | Chronic-condition burden increases substantially with age |
| Patient Retention | Returning patients represent the majority of visits |

---

## Recommendations

Based on the analysis, the project identifies the following management actions:

### 1. Address the Cardiology OPD Bottleneck
Investigate scheduling, patient flow, staffing, and visit-volume patterns contributing to longer waits.

### 2. Make Waiting Time a Key Patient Experience KPI
Track waiting time regularly by department and visit type and monitor the growth of high-delay visits.

### 3. Manage OPD and Inpatient Operations Separately
Since visit volume and revenue contribution differ significantly, operational and financial planning should account for these differences.

### 4. Reduce Financial Burden for Self Pay Patients
Explore Government Scheme enrollment support and payment options for patients facing higher out-of-pocket expenses.

### 5. Strengthen Chronic-Care Programs for Older Patients
Focus screening, follow-up, and chronic-care capacity around older patient groups where chronic conditions are more prevalent.

---

## Technology Stack

- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Seaborn**
- **Jupyter Notebook**

---

## Visualizations Used

The project uses multiple visualization techniques to communicate hospital performance, including:

- Department visit-volume charts
- Age-group analysis
- Department waiting-time boxplots
- Department × visit-type waiting-time heatmaps
- Waiting-time distribution charts
- Waiting-time vs satisfaction analysis
- Revenue comparisons by visit type
- Chronic-condition distribution by age group
- Financial analysis charts
- Correlation heatmaps

---

## Project Structure

```text
hospital-operations-service-financial-analytics/
│
├── patients.csv
├── visits.csv
├── billing.csv
├── final codefile.ipynb
└── README.md
