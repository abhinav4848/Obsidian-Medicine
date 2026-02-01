---
tags:
  - stats
urls:
  - https://chatgpt.com/share/6934f4bf-00b0-8012-86e9-bac790ddff7d
---
# Parametric tests
Normally distributed (the classic bell curve). 
Usually measured on a continuous scale (height, BP, HbA1c).
Because it's well-behaved mathematically, we can use more powerful statistical tests

|                                                  |                                                                                                                                                                                                             |
| ------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Pearson's product-moment correlation coefficient | is a parametric test assessing correlation. The type of significance test used depends on whether the data is parametric (something which can be measured, usually normally distributed) or non-parametric. |
| Student's unpaired t-test                        | is used for parametric data. T-tests = comparing averages                                                                                                                                                   |
| Student's paired t-test                          | is used for parametric data, and data needs to be paired.                                                                                                                                                   |

- **Paired data** refers to data obtained from a single group of patients, such as before and after an intervention. 
- **Unpaired data** comes from two different groups of patients, such as those given the vaccine and those given the placebo in a study. 

# Non-Parametric tests
Does not follow a normal distribution. 
Might be skewed, have outliers, or be based on ranks/ categories. e.g. Pain score (0-10), Likert scales, time to recovery. 

|                                                                                   |                                                                                                                                                                                                      |
| --------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Mann–Whitney U test                                                               | comparing ranked scores. This is for non-parametric data and compares ordinal, interval, or ratio scales of unpaired data. <br>	- e.g. Scale like 'Never', 'Rarely', 'Sometimes', 'Often', 'Always'. |
| Wilcoxon signed-rank test                                                         | compares two sets of observations on a single sample, e.g. a 'before' and 'after' test on the same population following an intervention.                                                             |
| chi-squared test                                                                  | used to compare proportions or percentages e.g. compares the percentage of patients who improved following two different interventions                                                               |
| Spearman rank, <br>Kendall rank correlation coefficient, aka<br>Kendall's τ (tau) | correlation (Correlation = seeing if two numbers move together)                                                                                                                                      |

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
# Paired vs Unpaired
### Parametric
**Paired = same people measured twice**  
(e.g. weight before vs after diet)

**Unpaired = different groups of people**  
(e.g. Group A on drug vs Group B on placebo)

### Non-parametric
Mann-Whitney U = comparing 2 unpaired non-parametric groups  
Wilcoxon = comparing 2 paired non-parametric groups