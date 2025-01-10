# Exam Period Coffee Spending Analysis

## Project Description
Visualizations and Code
All visualizations and code used in this project are available for review and exploration on my GitHub page and personal website. Visit [https://omer-ersoy.github.io/](https://omer-ersoy.github.io/) for access.

This project investigates the frequency of coffee transactions during midterm and final exam periods. By analyzing personal spending data, we aim to determine whether coffee transaction frequency increases during these stressful academic periods.

## Hypothesis

### Null Hypothesis (H0):

There is no significant difference in coffee transaction frequency between exam periods and normal periods.

### Alternative Hypothesis (HA):

Exam periods have a significant impact on coffee transaction frequency.

## Data Sources

### Spending Data:

- Personal bank statement filtered for coffee shop purchases.
- Data fields include:
  - Transaction date.
  - Merchant name.

### Exam Periods:

- Derived from the university's [academic calendar](https://www.sabanciuniv.edu/en/academic-calendar?b=2024&c=16&d=tr) or personal study schedule.
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

- Visualizations were used to highlight frequency differences in coffee transactions during exam periods compared to normal periods:

  - **Bar Plot:** Provides a clear comparison of total transactions during exam and normal periods.

  - **Scatter Plot:** Displays individual transaction occurrences over time, showing distribution patterns.

  - **Line Plot:** Illustrates trends in transaction frequency, emphasizing changes across time.

## Findings

### Statistical Findings:

- Total coffee transactions during exam periods: 52.
- Total coffee transactions during normal periods: 182.
- **Chi-squared test results:**
  - Chi-squared statistic: 2.32.
  - P-value: 0.12.

### Additional Data Analysis:

- Seasonal coffee consumption was analyzed to investigate potential patterns:
  - Monthly transaction counts ranged from 1 (July) to 42 (December).
  - Spearman correlation analysis showed a significant inverse relationship between monthly average temperature and coffee consumption frequency:
    - **Spearman Correlation:** -0.65
    - **P-value:** 0.02 (statistically significant)

## Conclusion

This analysis provides insights into whether coffee transaction frequency increases during exam periods. However, the results failed to reject the null hypothesis (H0) and did not provide sufficient evidence to support the alternative hypothesis (H1). This indicates that exam periods do not have a statistically significant impact on coffee transaction frequency.

## Tools and Libraries Used

- **Data Processing:** Python (pandas, numpy, read_excel)
- **Statistical Analysis:** SciPy (chi2_contingency, spearmanr)
- **Visualization:** Matplotlib (scatter, plot, bar)

## Additional Data

- This analysis also provides insight into the distribution of coffee transactions across different brands, showing that Starbucks has the highest transaction count, followed by other brands such as Fasshane, Coffy, and EspressoLab.
- The significant inverse relationship between monthly average temperature and coffee consumption frequency highlights an interesting seasonal pattern worth exploring further.

## Limitations

- The analysis is based solely on personal data, meaning:
  - It reflects patterns and trends observed in a specific individual's behavior.
  - Findings may not be applicable or generalizable to a broader population.
  - Different individuals or groups may have varying habits, preferences, and external factors influencing their behavior, which are not captured in this dataset.
- Limited to specific coffee vendors.
- The bank transaction file was not shared publicly due to privacy concerns.

## Future Directions

- Expand the dataset to include other caffeine-related purchases.
- Explore correlations between transaction frequency and academic performance.
- Investigate broader seasonal and temperature-related consumption patterns.

