---
tags:
  - stats
---
*see [[statistics- significance tests]]* 
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
# Ranking data %%linked%%
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
[chatgpt](https://chatgpt.com/share/697feb75-5aec-8012-9b56-8446cce9d893)
Rank all observations across two unpaired groups.
**Process**
1. Combine values from both groups.
2. Rank all values from smallest to largest.
3. Sum the ranks for each group.
4. Compare the rank sums to see if one group tends to have higher values.
**Idea:**
> Tests whether **one independent group tends to have larger values than the other**.
## Signed-Rank
Rank the differences within pairs.
**Process**
1. Calculate the **difference** between paired measurements (before & after intervention)
2. Rank the **absolute differences** (ignore signs initially).
3. Add the **sign (+/−)** back to each rank.
4. Sum positive and negative ranks to see if changes occur consistently in one direction.
**Idea:**
> Tests whether **paired measurements consistently increase or decrease**.

---
# Nominal Data vs Ordinal Data %%linked%%

| Feature        | Meaning                                                                                              |
| -------------- | ---------------------------------------------------------------------------------------------------- |
| Quantitative   | Can be discrete or continuous                                                                        |
| Categorical    | aka Qualitative data. Can be nominal or ordinal                                                      |
| Nominal        | Categories with no order                                                                             |
| Ordinal        | Categorical data. Just has an order.                                                                 |
| Paired         | Same subject measured twice or matched pairs                                                         |
| Interval scale | Quantitative. Values are ordered, differences are meaningful, but ratios don't exist as no true zero |
| ratio scale    | Quantitative. Values have order, equal intervals, true zero exists                                   |
### Nominal data
Categorical data with NO natural order (Nominal = _name only_) & no ranking. 
- e.g. Blood group, eye colour, diagnosis type.
**Key idea**: Categories are different but not ranked.

Special case of nominal data is binary data: yes/no, alive/dead. 

### Ordinal data
Categorical data with a natural order or ranking. 
- Data is **ordered**, but the **distance between values isn’t consistent or known**.
- You can say _greater/less_, but not _how much greater_.
e.g. 
- Mild → Moderate → Severe
- Pain score categories
- Satisfaction levels (poor / fair / good)
- Underweight < Normal < Overweight < Obese
	- Raw BMI (e.g. 23.4 kg/m²) would be continuous. But you've converted it into categories, so no longer continuous

**Key idea**: Categories are ranked, but the distance between them is not necessarily equal. If we mark mild/mod/severe as 1,2,3, then the jump from 1 → 2 is not guaranteed to equal 2 → 3.

**Note**: Ordinal data is not "non-normal". The idea of normality simply doesn’t apply to it. Ordinal data are categories with order, not true numbers. Because ordinal data are not true continuous numbers, we usually analyse them with non-parametric tests, such as: Mann–Whitney U test, Wilcoxon signed-rank test, Spearman's rank correlation coefficient.
These tests work with ranks rather than numerical distances.
### Paired Nominal data
Nominal categorical data where observations are paired within the same subject or matched unit.
Example: Smoking status **before and after** an intervention.

|Patient|Before|After|
|---|---|---|
|A|Smoker|Non-smoker|
|B|Smoker|Smoker|
- **Data type:** Nominal (smoker / non-smoker)
- **Observation type:** Paired (same person measured twice)
### Interval scale
- Values are ordered and **differences are meaningful and equal**.
- But there’s **no true zero**, so ratios don’t make sense.
**Examples**: Temperature in °C or °F ; IQ scores
**Why no true zero?** : 0°C doesn’t mean “no temperature” — it’s arbitrary.

**Key point:**  
✔ Order + equal intervals  
❌ Cannot say “twice as much”
### Ratio scale (full mathematical meaning)
- Has order + equal intervals + a true zero.
- You can do all maths, including ratios.

**Examples:** Weight, Height, Age, Income, Temperature in Kelvin
**Why true zero matters:** 
0 kg = absence of weight → makes ratios meaningful  
(80 kg is twice 40 kg) 

**Key point:**  
✔ Order + equal intervals + true zero 
✔ Ratios meaningful

---
# t-Test vs U-test
A t-test compares means for normally distributed continuous data. It is a measure of similarity between two means. 
The Mann–Whitney U test compares ranks when data are non-normal or ordinal. 
- t-test: compares averages using actual values. 
- U-test: compares relative positions using ranks (U = Unpaired) 

| Situation                                | Parametric Test               | Non-Parametric Equivalent                  | Notes                                                       |
| ---------------------------------------- | ----------------------------- | ------------------------------------------ | ----------------------------------------------------------- |
| Two independent groups                   | Unpaired (independent) t-test | Mann–Whitney U test aka. Wilcoxon rank-sum | Compares group averages vs ranks; data should be continuous |
| Same individuals measured twice (paired) | Paired t-test                 | Wilcoxon signed-rank test                  | Compares before–after or matched pairs; uses differences    |
- Unpaired → independent groups → t-test / U-test
- Paired → same subjects → paired t-test / signed-rank

### T-test for independent samples
- Also called **unpaired t-test**
- **Key point:** The two groups are **independent** – nobody in one group is “paired” with anyone in the other.

---
# Correlation Coefficient
Correlation coefficient, denoted by 'r', is a statistical measure that calculates the strength of the relationship between the relative movements of two variables.

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