# Statistics for Data Science with Python (IBM-Coursera)

Basic principles of statistical methods and procedures used for data analysis


## Hypothesis Testing

Use the norm.cdf() function in the scipy.stats library to find the standardized (z-score) value. In cases where we are looking for the area to the right of the curve, we will remove the results above from 1. Remember to import scipy.stats

Levene's test for equal variance: Levene's test is a test used to check for equality of variance among groups. We use the scipy.stats.levene() from the scipy.stats library.

T-test for two independent samples: This test compares the means of two independent groups to determine whether there is a significant difference in means for both groups. We use the scipy.stats.ttest_ind() from the scipy.stats library.

One-way ANOVA: It compares the mean between two or more independent groups to determine whether there is a statistical significance between them. We use the scipy.stats.f_oneway() from the scipy.stats library or you can use the anova_lm() from the statsmodels library.

Chi-square (𝜒2) test for association: Chi-square test for association tests the association between two categorical variables. To do this we must first create a crosstab of the counts in each group. We do this by using the crosstab() function in the pandas library. Then the scipy.stats.chi2_contingency() on the contingency table - it returns the 𝜒2 value, p-value, degree of freedom and expected values.

Pearson Correlation: Tests the correlation between two continuous variables. we use the scipy.stats.pearsonr() to get the correlation coefficient

To run the tests using Regression analysis, you will need the OLS() from the statsmodels library. When running these tests using regression analysis, you have fit() the model, make predictions using predict() and print out the model summary using model.summary()
