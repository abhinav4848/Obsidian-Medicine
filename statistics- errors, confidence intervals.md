---
tags:
  - stats
---
# Errors, Power
### Type 1 error (α)
false positives. 
> You conclude the new drug works when it doesn't. 

- Probability of Type 1 error = **31%**
- That means: **31 times out of 100**, this study would wrongly say _“new drug is better”_ when in reality there is **no true difference**

*Most studies accept (α) = 5% (0.05)*
### Type 2 error (β)
false negative. 
> You conclude the new drug does **not** work when it actually **does**. 

- Probability of Type 2 error = **26%**
- So: **26 times out of 100**, the study would miss a real benefit

This corresponds to **power**:
> **Power = 1 − β**

- Standard acceptable power = **80–90%**
- This study is **underpowered**

---
# p-value 
if p-value = 0.04
### What does this mean?
> If there were actually **no difference** between the drugs, the chance of seeing results this extreme (or more) is **4%**

Since:
- p = 0.04
- Conventional cutoff = 0.05
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
- For [[statistics- risk reduction|relative risk / odds ratio]] → does not cross **1**

➡️ That agrees with the p-value being < 0.05