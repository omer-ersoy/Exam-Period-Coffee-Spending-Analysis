# Exam Period Coffee Spending Analysis

## Project Description

This project investigates the frequency of coffee transactions during midterm and final exam periods. By analyzing personal spending data, we aim to determine whether coffee transaction frequency increases during these stressful academic periods.

## Hypothesis

### Null Hypothesis (H0):

There is no significant difference in coffee transaction frequency between exam periods and normal periods.

### Alternative Hypothesis (H1):

Exam periods have a significant impact on coffee transaction frequency.

## Data Sources

### Spending Data:

- Personal bank statement filtered for coffee shop purchases.
- Data fields include:
  - Transaction date.
  - Merchant name.

### Exam Periods:

- Derived from the university's academic calendar or personal study schedule.
- Defined as the exam dates plus 1-2 days before for preparation.

## Methodology

### 1. Data Preparation

- **Filter Relevant Transactions:**

  - Extract only coffee-related transactions.

- **Define Exam Periods:**

  - Include the following periods:
    - **First Final:** January 8-20, 2023
    - **First Midterm:** April 11-24, 2023
    - **Second Final:** May 30 - June 11, 2023
    - **Second Midterm:** November 6-18, 2023
    - **Third Final:** January 5-19, 2024
    - **Third Midterm:** March 22 - April 3, 2024
    - **Fourth Final:** May 29 - June 9, 2024
    - **Fourth Midterm:** November 1-16, 2024
    - **Fifth Midterm:** November 29 - December 14, 2024
    - **Fifth Final:** January 1-12, 2025

### 2. Data Analysis

- **Categorize Transactions:**

  - Label each transaction as "Exam Period" or "Normal Period" based on its date.

- **Statistical Analysis:**

  - Perform a chi-squared test to compare transaction frequencies during exam and normal periods.
  - Use the p-value to determine the statistical significance of the observed differences.

### 3. Visualization

- Create visualizations to highlight trends:
  - Bar plots showing transaction counts during exam vs. normal periods.
  - Time-series plots illustrating transaction frequency fluctuations over time.

## Results

### Statistical Findings:

- Total transactions during exam periods: 91.
- Total transactions during normal periods: 161.
- **Chi-squared test results:**
  - Chi-squared statistic: 18.30.
  - P-value: 0.000019.
  - Conclusion: There is a statistically significant difference in coffee transaction frequency between exam and normal periods.

### Visualization:

- Bar plots reveal frequency differences during exam periods compared to normal periods.

## Conclusion

This analysis provides insights into whether coffee transaction frequency increases during exam periods. The results reject the null hypothesis (H0) and support the alternative hypothesis (H1), indicating a significant impact of exam periods on coffee transaction frequency. Future work could involve:

- Expanding the dataset to include more semesters.
- Investigating transaction frequencies across different merchants.

## Tools and Libraries Used

- **Data Processing:** Python (pandas, numpy)
- **Statistical Analysis:** SciPy
- **Visualization:** Matplotlib

## Limitations

- The analysis is limited to personal data, which may not generalize to others.

## Future Directions

- Automate merchant categorization using machine learning.
- Expand the dataset to include other caffeine-related purchases.
- Explore correlations between transaction frequency and academic performance.

