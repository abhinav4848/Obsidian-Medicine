---
tags:
  - stats
urls:
  - https://chatgpt.com/share/697feb75-5aec-8012-9b56-8446cce9d893
---
*See also [[statistics- basics about data]]* 
# Parametric tests
Normally distributed (the classic bell curve). 
Usually measured on a continuous scale (height, BP, HbA1c).
Because it's well-behaved mathematically, we can use more powerful statistical tests

|                                                  |                                                                                                                                                                                                                                                  |
| ------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Pearson's product-moment correlation coefficient | is a parametric test assessing correlation. The type of significance test used depends on whether the data is parametric (something which can be measured, usually normally distributed) or non-parametric. e.g relation between height & weight |
| Student's unpaired t-test                        | is used for parametric data. T-tests = comparing averages                                                                                                                                                                                        |
| Student's paired t-test                          | is used for parametric data, and data needs to be paired.                                                                                                                                                                                        |
| ANOVA                                            | Used to demonstrate statistically significant differences between the means of several groups. It is similar to a student's t-test apart from that ANOVA allows the comparison of more than just two means.                                      |
To use Student's _t_-test we must be able to assume that the dependent variable in each group is normally distributed. If the data are near-normal or a suitable transformation is applied to the data to make them normal, Student's _t_-test can sometimes be used
# Non-Parametric tests
Skewed or ranked data. 
Does not follow a normal distribution. 
Might be skewed, have outliers, or be based on ranks/ categories. e.g. Pain score (0-10), Likert scales, time to recovery. 

|                                                                                   |                                                                                                                                                                                                                                                                                                                                                                                      |
| --------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Mann–Whitney U test aka Wilcoxon rank-sum test                                    | Comparing ranked scores on unpaired data. This is for non-parametric data and compares `ordinal, interval, or ratio scales` of unpaired data. <br>	- e.g. Scale like *'Never', 'Rarely', 'Sometimes', 'Often', 'Always'*.<br>Same as student unpaired t test<br><br>#mnemonic U test: Unpaired data                                                                                  |
| Wilcoxon signed-rank test aka Wilcoxon matched pair                               | Compares two sets of observations on a single sample (paired), e.g. a 'before' and 'after' test on the same population following an intervention. `Ordinal Paired` e.g *pain score before and after a new physio regimen.*<br>Same as student paired t test                                                                                                                          |
| chi-squared test                                                                  | Used to compare proportions or percentages in [[statistics- basics about data#Nominal Data vs Ordinal Data linked\|nominal]] unpaired categorical data (e.g. pass/fail) to see if there's an association between 2 variables. e.g. *compare the percentage of patients who improved following two different interventions*, male vs female exam participants & their pass/fail ratio |
| Spearman rank, <br>Kendall rank correlation coefficient, aka<br>Kendall's τ (tau) | Correlation (Correlation = seeing if two numbers move together). Same as Pearson's but for non-parametric                                                                                                                                                                                                                                                                            |
| McNemar's test                                                                    | used to analyse nominal paired data that is non-parametric. Classically this test can be used to compare the sensitivity and specificity of 2 diagnostic tests on a matched sample.                                                                                                                                                                                                  |
#### These two names are the same test:
| Name (See [[statistics- basics about data#Ranking data linked\|Rank meaning]]) | Why it exists                                                                                                                           |
| ------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------- |
| Mann–Whitney U test                                                            | Name emphasises the U statistic used in the calculation. <br>U is a test statistic calculated from:<br>- The sum of ranks in each group |
| Wilcoxon rank-sum test                                                         | **Name emphasises the sum of ranks used in the method**.                                                                                |
They both:
- Compare two independent (unpaired) groups
- Use ranks instead of raw values
- Are non-parametric alternatives to the unpaired t-test

**Example**: Compare **pain scores** between: patients on **drug A** & patients on **placebo**

---
# Correlation (relationship between two variables)
Correlation means seeing whether two variables move together (as one increases, does the other increase or decrease?).

| Purpose                                                               | Parametric test                                  | Non-parametric test              |
| --------------------------------------------------------------------- | ------------------------------------------------ | -------------------------------- |
| Strength & direction of relationship between two continuous variables | Pearson's product-moment correlation coefficient | Spearman's rank or Kendall’s tau |
### Pearson's correlation
- **Parametric**
- Assumes data is normally distributed and linear
- Gives a value **r** (from –1 to +1)  
    🔹 +1 = perfect positive relationship  
    🔹 –1 = perfect negative relationship  
    🔹 0 = no correlation
### Spearman / Kendall
- **Non-parametric**
- Use when data isn’t normally distributed or is ranked/ordinal
- Spearman and Kendall also give a value between –1 and +1 but based on RANKS, not raw numbers
---
# ANOVA
Analysis of Variance
It's a statistical method used to determine whether there are any statistically significant differences between the means of three or more independent groups. e.g. you are comparing the weight gain of individuals across three different diets with varying sugar content. It is similar to a student's t-test apart from that ANOVA allows the comparison of more than just two means. 

ANOVA assumes that the variable is normally distributed. The nonparametric equivalents to this method are the Kruskal-Wallis analysis of ranks, the Median test, Friedman's two-way analysis of variance, and Cochran Q test

It works by comparing the variance of the means. It distinguishes between within group variance (the variance of the sample mean) and between group variance (the variance between the separate sample means). The null hypothesis assumes that the variance of all the means are the same and that within group variance is the same as between group variance. The test is based on the ratio of these two variances (known as the F statistic).