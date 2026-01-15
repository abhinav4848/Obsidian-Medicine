---
tags:
  - stats
aliases:
  - hypothesis testing
  - significance tests
---
# Errors, Power
The probability of errors happening is chosen during study design itself. They're thresholds you're willing to accept. 

| Reality                  | H1                  | H0                   |
| ------------------------ | ------------------- | -------------------- |
| Study rejects H0         | Power (1-Beta)      | Alpha (Type 1 error) |
| Study does not reject H0 | Beta (Type 2 error) | -                    |
### Type 1 error (α)
This is also called significance level & tells the acceptable possibility of seeing a difference between 2 groups when it doesn't exist.
aka. False positive. 

i.e. the maximum acceptable probability of rejecting the null hypothesis when it's actually true. 
> You conclude the new drug works when it doesn't. 

- Probability of Type 1 error = **31%**
- That means: **31 times out of 100**, this study would wrongly say _“new drug is better”_ when in reality there is **no true difference**

*Most studies accept (α) = 5% (0.05)*

 As the significance level is determined in advance the chance of making a type I error is not affected by sample size. It is however increased if the number of end-points are increased. For example if a study has 20 end-points it is likely one of these will be reached, just by chance.
### Type 2 error (β)
Null hypothesis is acc
false negative. 
> You conclude the new drug does **not** work when it actually **does**. 

- Probability of Type 2 error = **26%**
- So: **26 times out of 100**, the study would miss a real benefit

This corresponds to **power**:
> **Power = 1 − β**

Power means correctly identifying the result regardless of whether the hypothesis is accepted or rejected. A study with high power can accurately identify an effect (or difference when one exists) or vice versa.

- Standard acceptable power = **80–90%**
	- *Most studies accept (β) = 10-20%*
- As (β) = 26%, This study is **underpowered**

---
# p-value 
if p-value = 0.04
### What does this mean?
> If there were actually **no difference** between the drugs, the chance of seeing results this extreme (or more) is **4%**

Since:
- p = 0.04
- Conventional cutoff = 0.05
- i.e you reject the null-hypothesis if p-value comes < α
➡️ The result is **statistically significant**

So the researcher would **reject the null hypothesis** and say:
> “There is evidence the new drug is different (or better) than the old drug.”

---
## Confidence interval
CI = 95%
### This means:
> If we repeated this trial **100 times**, about **95 of those confidence intervals** would contain the **true treatment effect**

⚠️ Important:
- A **95% CI does NOT mean** “there is a 95% chance the true value lies inside this CI” 
- The true value is fixed — the interval varies

If the **95% CI does not cross the null value**:
- For difference in means → does not cross **0**
- For [[statistics- risk reduction, nnt, odds ratio|relative risk / odds ratio]] → does not cross **1 (one)**

➡️ That agrees with the p-value being < 0.05

---


