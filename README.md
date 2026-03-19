# Customer Segmentation Analysis

This repository contains a detailed analysis of customer data from a CSV file. The goal is to uncover key demographic and behavioral insights that can drive marketing strategies and business decisions. The analysis replicates and extends the summary metrics shown in the provided Power BI dashboard screenshots.

## Dataset Description

- **File:** `customers.csv`
- **Records:** 500 customers
- **Columns:**
  - `CustomerID`: Unique identifier
  - `Name`: Customer name
  - `Gender`: Male/Female (note: there are inconsistencies – see data cleaning)
  - `Age`: Customer age
  - `Region`: Geographic region (North, South, East, West)
  - `Occupation`: Job category (Doctor, Engineer, Teacher, Trader, Banker, Student, Retired)
  - `Income`: Annual income (in dollars)
  - `Customer_Segment`: Retail, Corporate, Private
  - `Join_Date`: Date when customer joined

## Data Cleaning Notes

- The `Gender` column contains values that do not always match the name prefix (e.g., "Mrs." with `Male`). This could be a data entry error. For the purpose of this analysis, we use the `Gender` column as provided.
- No missing values were found.
- `Join_Date` was converted to datetime format to calculate customer tenure.

## Key Insights

The analysis yields the following insights, which align with the Power BI dashboard screenshots:

### 1. Demographics
- **Gender Distribution:** 48.8% Female, 51.2% Male.
- **Average Age:** 46.3 years.
- **Average Income:** $112,450 (overall).

### 2. Regional Distribution
- **South:** 137 customers
- **East:** 133 customers
- **North:** 120 customers
- **West:** 110 customers

### 3. Occupation Breakdown
- Trader: 15.7%
- Teacher: 15.6%
- Student: 15.1%
- Doctor: 14.4%
- Banker: 14.4%
- Retired: 13.8%
- Engineer: 11.8%

### 4. Customer Segment Distribution
- Retail: 286 customers (57.2%)
- Corporate: 169 customers (33.8%)
- Private: 45 customers (9.0%)

### 5. Age Group Analysis
We defined age groups as:
- Youth: 18–30
- Young: 31–45
- Adult: 46–60
- Senior: 60+

**Average age per group:**
- Senior: 67 years
- Adult: 49 years
- Young: 32 years
- Youth: 21 years

**Customer count per age group:**
- Senior: 169
- Adult: 148
- Young: 112
- Youth: 71

### 6. Gender‑Based Subsets
- **Female customers (244):** Average age 47.7, average income $108.2K. Most are in Retail segment (150).
- **Male customers (256):** Average age 44.8, average income $114.1K. Most are in Corporate segment (86).

### 7. Customer Growth Timeline
- Number of new customers has steadily increased from 2016 (11) to 2024 (29), with a dip in 2023.

## Visualizations


- Gender distribution (pie/bar chart)
- Age histogram by gender
- Income distribution by customer segment
- Occupation frequency (horizontal bar chart)
- Region counts (bar chart)
- Customer growth over time (line chart)
- Age group averages (bar chart)
- Segment distribution (stacked bar by gender)

