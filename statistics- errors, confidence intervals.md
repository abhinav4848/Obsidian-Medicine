---
tags:
  - stats
aliases:
  - hypothesis testing
  - significance tests
---
A null hypothesis (H0) states that two treatments are equally effective (and is hence negatively phrased). A significance test uses the sample data to assess how likely the null hypothesis is to be correct.
# Errors, Power
They're thresholds you're willing to accept. 

| Reality    | H0                  | H1                   |
| ---------- | ------------------- | -------------------- |
| Reality H0 | -                   | Alpha (Type 1 error) |
| reality H1 | Beta (Type 2 error) | Power (1-Beta)       |
### Type 1 error (α)
This is also called significance level & tells the acceptable possibility of seeing a difference between 2 groups when it doesn't exist. 
aka. False positive (The null hypothesis is rejected when it is true)

i.e. the maximum acceptable probability of rejecting the null hypothesis when it's actually true. 
> You conclude the new drug works when it doesn't. 

- Probability of Type 1 error = **31%**
- That means: **31 times out of 100**, this study would wrongly say _“new drug is better”_ when in reality there is **no true difference**

*Most studies accept (α) = 5% (0.05)*

As the significance level is determined in advance the chance of making a type I error is not affected by sample size. It is however increased if the number of end-points are increased. For example if a study has 20 end-points it is likely one of these will be reached, just by chance.
### Type 2 error (β)
Null hypothesis is accepted when it's false. 
aka. false negative. 
> You conclude the new drug does **not** work when it actually **does**. 

- Probability of Type 2 error = **26%**
- So: **26 times out of 100**, the study would miss a real benefit

This corresponds to **power**:
> **Power = 1 − β**

Power means 
- correctly identifying the result regardless of whether the hypothesis is accepted or rejected. A study with high power can accurately identify an effect (or difference when one exists) or vice versa. 
- Power of a study is the probability of (correctly) rejecting the null hypothesis when it is false, i.e. the probability of detecting a statistically significant difference
- Power can be increased by increasing the sample size. 

- Standard acceptable power = **80–90%**
	- *i.e. Most studies accept (β) = 10-20%*
- If (β) = 26%, that study would be considered **underpowered**

The probability of type 1 error happening is chosen during study design itself, but type 2 error depends on sample size & alpha. 
- By increasing the sample size, you decrease beta, thus increase the power.

### Standard error
Statistics is based on the idea of taking a sample from a population. If you were to take many samples from a population and calculate a mean for each sample, these samples would be arranged into a distribution around the true population mean. The standard deviation of this distribution is called the standard error. The standard error is used in the calculation of a confidence interval. 
### Systematic error
Systematic error, also known as [[statistics- biases|bias]], involves a systematic deviation from the truth. There are many possible sources of bias within an RCT e.g. one comparing remdesivir and placebo, including selection bias, performance bias, detection bias, attrition bias, and reporting bias.

---
# p-value 
if p-value = 0.04
### What p = 0.04 mean?
> If there were actually **no difference** between the drugs (i.e. H0 was true), the chance of seeing results this extreme (or more) is **4%** 

Since:
- p = 0.04
- Conventional cutoff = 0.05
- i.e you reject the null-hypothesis if p-value comes < α
➡️ The result is **statistically significant**

So the researcher would **reject the null hypothesis** and say:
> “There is evidence the new drug is different (or better) than the old drug.”

| <br><br>       | Study accepts H0    | Study rejects H0     |
| -------------- | ------------------- | -------------------- |
| **Reality H0** |                     | Type 1 error (alpha) |
| **Reality H1** | Type 2 error (beta) | Power (1 - beta)     

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


