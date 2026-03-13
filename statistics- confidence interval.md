---
tags:
  - stats
aliases:
  - standard error of the mean
---
# Confidence interval and standard error of the mean
> Given a sample mean, how close is it likely to be to the true population mean?

The **confidence interval (CI)** gives a _range of plausible values_ for the true population mean.

The likelihood of the true effect lying within the confidence interval is determined by the confidence level. For example a confidence interval at the 95% confidence level means that the confidence interval should contain the true effect of intervention 95% of the time.  

---
## How is the confidence interval calculated?
The standard error of the mean (SEM) is a measure of the spread expected for the mean of the observations - i.e. how 'accurate' the calculated sample mean is from the true population mean  
##### Key point
- SEM = SD / square root (n)
	- SD = standard deviation
	- n = sample size

| Increase           | Effect on SEM |
| ------------------ | ------------- |
| Larger SD          | SEM increases |
| Larger sample size | SEM decreases |
So bigger samples → more precise estimate of the true mean.

---
## A 95% confidence interval
- lower limit = mean - (1.96 * SEM)
- upper limit = mean + (1.96 * SEM)
#### Why the number 1.96 appears
If sample means follow a **normal distribution**, then:

|Range|% of values|
|---|---|
|±1 SD|68%|
|±1.96 SD|95%|
|±2.58 SD|99%|
Because **sample means vary by the SEM**, we use:
Mean±1.96×SEM

That gives the range containing **95% of possible sample means**, which translates to a **95% confidence interval for the population mean**.

---
## We sometimes use Student’s t instead
The above formula is a slight simplification: 
- if a small sample size is used (e.g. n < 100) then it is important to use a 'Student's T critical value' look-up table to replace 1.96 with a different value
- When sample sizes are small, the estimate of SD is less reliable. So we adjust using the Student's t-distribution, which has fatter tails. This means the multiplier is slightly larger than 1.96.
- if a different confidence level is required, e.g. 90% then 1.96 is replaced by a different value. For 90% this would 1.645

Results such as mean value are often presented along with a confidence interval. For example, in a study the mean height in a sample taken from a population is 183cm. You know that the standard error (SE) (the standard deviation of the mean) is 2cm. This gives a 95% confidence interval of 179-187cm (+/- 2 SE).