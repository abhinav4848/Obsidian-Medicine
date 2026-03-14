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

|                                                  |                                                                                                                                                                                                             |
| ------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Pearson's product-moment correlation coefficient | is a parametric test assessing correlation. The type of significance test used depends on whether the data is parametric (something which can be measured, usually normally distributed) or non-parametric. |
| Student's unpaired t-test                        | is used for parametric data. T-tests = comparing averages                                                                                                                                                   |
| Student's paired t-test                          | is used for parametric data, and data needs to be paired.                                                                                                                                                   |

# Non-Parametric tests
Skewed or ranked data. 
Does not follow a normal distribution. 
Might be skewed, have outliers, or be based on ranks/ categories. e.g. Pain score (0-10), Likert scales, time to recovery. 

|                                                                                   |                                                                                                                                                                                                                            |
| --------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Mann–Whitney U test aka Wilcoxon rank-sum test                                    | Comparing ranked scores on unpaired data. This is for non-parametric data and compares `ordinal, interval, or ratio scales` of unpaired data. <br>	- e.g. Scale like *'Never', 'Rarely', 'Sometimes', 'Often', 'Always'*.  |
| Wilcoxon signed-rank test                                                         | Compares two sets of observations on a single sample (paired), e.g. a 'before' and 'after' test on the same population following an intervention. `Ordinal Paired` e.g *pain score before and after a new physio regimen.* |
| chi-squared test                                                                  | Used to compare proportions or percentages in `nominal unpaired` e.g. *compares the percentage of patients who improved following two different interventions*                                                             |
| Spearman rank, <br>Kendall rank correlation coefficient, aka<br>Kendall's τ (tau) | Correlation (Correlation = seeing if two numbers move together)                                                                                                                                                            |
| McNemar's test                                                                    | used to analyse nominal paired data that is non-parametric.                                                                                                                                                                |
#### These two names are the same test:
| Name (See [[statistics- basics about data#Ranking data linked\|Rank meaning]]) | Why it exists                                               |
| ------------------------------------------------------------------------------ | ----------------------------------------------------------- |
| **Mann–Whitney U test**                                                        | Name emphasises the **U statistic** used in the calculation |
| **Wilcoxon rank-sum test**                                                     | Name emphasises the **sum of ranks** used in the method     |
They both:
- Compare **two independent (unpaired) groups**
- Use **ranks instead of raw values**
- Are **non-parametric alternatives to the unpaired t-test**

Example : Compare **pain scores** between: patients on **drug A** & patients on **placebo**

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
