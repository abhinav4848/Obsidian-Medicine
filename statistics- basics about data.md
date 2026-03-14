---
tags:
  - stats
---
# Paired vs Unpaired

| Type              | Definition                                                                           | Example                           |
| ----------------- | ------------------------------------------------------------------------------------ | --------------------------------- |
| **Paired data**   | Data obtained from the same individuals measured twice or from matched pairs | Weight before vs after a diet |
| **Unpaired data** | Data obtained from two independent groups of individuals                         | Drug group vs placebo group   |
### Parametric Tests
Normally distributed numerical data. 
There is meaningful distances between numbers
Can be paired or unpaired. 

| Data type    | Test                          | Example                                          |
| ------------ | ----------------------------- | ------------------------------------------------ |
| **Unpaired** | Unpaired (independent) t-test | Mean BP in drug group vs placebo group           |
| **Paired**   | Paired t-test                 | Weight before vs after diet in the same patients |
### Non-parametric
Skewed or ranked data. 

| Data type    | Test                                             | Purpose                                                                               |
| ------------ | ------------------------------------------------ | ------------------------------------------------------------------------------------- |
| **Unpaired** | Mann–Whitney U test *aka* Wilcoxon rank-sum test | Compare two independent groups (unpaired) with non-parametric (skewed or ranked) data |
| **Paired**   | Wilcoxon signed-rank test                        | Compare paired measurements in the same individuals                                   |

---
# Ranking data
#### What is a rank, Why use it, when to use it? 
What: 
- Literally just ranking the data, like Rank 1, Rank 2... 
When: 
- Ranking can be done to any data, including parametric (normally distributed) data.
- But in statistics, ranking is mainly used in non-parametric tests.
Why: 
- Ranking replaces raw numbers with their **ordered position**.
- This removes information about **exact distances between values**.
#### Why it's not used in Parametric data?
Parametric tests like: **t-tests**, **ANOVA**, **Pearson correlation** use the **actual numerical values**, because they assume:
- normally distributed data
- meaningful distances between numbers

Example: BP 120 vs 140 → difference **20 mmHg** matters.
Ranking would throw away that information.
## Rank-Sum
Rank all observations across two groups.
## Signed-Rank
Rank the differences within pairs.

---
# Nominal Data vs Ordinal Data
### Nominal data
**Categories with NO natural order** (Nominal = _name only_)
e.g. Blood group, eye colour, diagnosis type.
### Ordinal data
Categories with order
e.g. Mild, moderate, severe

### Paired Nominal data
e.g. Smoking status before and after an intervention
Data is nominal (smoker/non-smoker), Observation is paired (before and after on the same person)

---
# Correlation Coefficient
A **single number** that tells you:
- **Direction** (positive or negative)
- **Strength** (how tightly related)
### Range
`-1 to +1`

| Value | Meaning                       |
| ----- | ----------------------------- |
| +1    | Perfect positive relationship |
| 0     | No relationship               |
| -1    | Perfect negative relationship |
### Examples
- Height vs weight → positive correlation
- Exercise vs resting heart rate → negative correlation