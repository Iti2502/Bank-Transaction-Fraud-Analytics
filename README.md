# Bank-Transaction-Fraud-Analytics
This project aims to analyse 200K transactions data to uncover fraud trends across time, account types, transaction categories, and many more categories. 

Following is a short overview of the work that has been done:

* Created new features like time between transactions, transaction hour (as sine/cosine), and holiday indicators to understand user behavior.
∗ Used statistical tests (Chi-squared, ANOVA, etc) to check if frauds were linked to account type, balance range, or special days.
∗ Built a clean, reusable data cleaning and preprocessing pipeline to handle cleaning, creating mappings, and other transformations.
∗ Identified fraud spikes around national events and disproved common assumptions (e.g., business accounts having higher fraud due to larger balances) using statistical tests like ANOVA and Chi-Square.


Statistical Tests for Deeper Insights:

- Shapiro-Wilk Test: Rejected normality for all account types — data is not normally distributed.
- Levene’s & ANOVA Tests: No significant variance or mean differences across account types.
- Kruskal-Wallis Test: Confirmed no significant difference in balance distributions by account type.
- T-test & Mann-Whitney: Festivals don’t significantly affect fraud rates.
- Chi-Square Test: Fraud is evenly spread across all hours — not limited to odd or business hours.

Key Insights:

* Fraud is not time-bound — it can occur at any hour with equal probability.
* Business accounts showed slightly higher fraud rates, but statistical tests revealed no strong link to account balance.
* While Finance and Travel categories had higher fraud rates, seasonal spikes during festivals weren’t statistically significant.
