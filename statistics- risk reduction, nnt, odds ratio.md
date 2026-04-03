---
aliases:
  - absolute risk reduction
  - numbers needed to treat
  - relative risk
  - odd's ratio
tags:
  - stats
urls:
  - https://www.cebm.ox.ac.uk/resources/ebm-tools/number-needed-to-treat-nnt
---
NNT: how many patients would require an intervention to reduce the expected number of outcomes by one. 
### Absolute risk reduction = CER-EER or EER-CER?
ARR may be calculated by finding the absolute difference between the control event rate (CER) and the experimental event rate (EER). 

You will often find both versions of the above listed in different sources. In some ways in doesn't matter which you use as you will end up with the same answer but from a technical point of view:  
- if the outcome of the study is undesirable then ARR = CER - EER 
- if the outcome of the study is desirable then ARR* = EER - CER 
\*this may be more accurately termed absolute benefit increase, rather than absolute risk reduction

# Odd's ratio
|               | Event/outcome | No Event/outcome |
| ------------- | ------------- | ---------------- |
| Treatment (E) | a             | b                |
| Control (C)   | c             | d                |
`EER= a/a+b` & `CER=c/c+d` 

Odds of an event in treatment group: `EER/1-EER` = `a/b` 
- *odds => (probability of event/probability of no event)* 
- *`1 − EER` => what proportion did not have the event => `non-events/total` = `b/(a+b)`* 
Odds of an event in control group: `CER/1-CER` 
so, ratio= odds in treatment/odds in control = `a.d/c.b` 

# Formulae

$$
\begin{aligned}
\text{Experimental Event Rate (EER)} 
&= \frac{\text{Number who had particular outcome with intervention}}
{\text{Total number who had the intervention}} \\[6pt]
&= \frac{a}{a+b} \\[10pt]

\text{Control event rate (CER)} &= \frac{\text{Number who had a particular outcome with the control}}
{\text{Total number who had the control}}\\[6pt]
&= \frac{c}{c+d} \\[10pt]

\text{ARR} &= \text{CER} - \text{EER} \\[6pt]

\text{Number needed to treat (NNT)} &= \frac{1}{\text{Absolute Risk Reduction}} \\[6pt]

\text{RR} &= \frac{\text{EER}}{\text{CER}} \\[6pt]

\text{RRR} &= 1 - \text{RR} \\[6pt]

\text{OR} &=
\frac{\text{EER} / (1 - \text{EER})}
{\text{CER} / (1 - \text{CER})}
\end{aligned}
$$
$$
\begin{aligned}
\text{CER} &= \frac{20}{100} = 0.20 \\
\text{EER} &= \frac{10}{100} = 0.10 \\
\text{ARR} &= 0.20 - 0.10 = 0.10 \\
\text{NNT} &= \frac{1}{0.10} = 10 \\
\text{RR} &= \frac{0.1}{0.2} = 0.05 
\end{aligned}
$$
