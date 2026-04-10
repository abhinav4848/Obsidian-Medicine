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

# Odds ratio vs Risk ratio

| Odds Ratio                                                                                                           | Risk Ratio aka Relative Risk                                                                                      |
| -------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------- |
| Case-control studies                                                                                                 | Cohort / RCTs                                                                                                     |
| Compares odds (not probability) of an outcome in exposed individuals to odds of an outcome in unexposed individuals. | Compares the risk of an outcome in exposed individuals to the risk of that same outcome in unexposed individuals. |
| - You **start with disease status** (cases vs controls)<br>- Then look _backward_ at exposure                        | - You **start with exposure**<br>- Then follow *forward* to see who gets disease                                  |
| - Smokers: 20 disease / 80 no disease → odds = 0.25<br>- Non-smokers: 10 / 90 → odds = 0.111                         | - 20 out of 100 smokers get disease → risk = 0.2<br>- 10 out of 100 non-smokers → risk = 0.1                      |
| OR= 0.25/0.111 = 2.25<br>Odds suggest a **2.25× increase**                                                           | RR > 1 → higher risk with exposure<br>RR < 1 → protective effect                                                  |
### Odds ratio

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
# Population attributable risk
The **population attributable risk** can be described as the reduction in incidence that would be observed if the population were entirely unexposed. For instance how would the incidence of lung cancer change if everyone stopped smoking? It can be calculated by multiplying the attributable risk by the prevalence of exposure in the population. 

By quantifying how much disease could be prevented by eliminating exposure, Population Attributable Risk provides an estimate for the potential impact on public health if effective control measures were implemented against specific risks. 
# Attributable proportion 
The **attributable proportion** is the proportion of the disease that would be eliminated in a population if its disease rate were reduced to that of the unexposed group.

# Attributable Risk (AR)
Sometimes called Risk Difference, measures how much of the disease incidence can be attributed directly to exposure. It's calculated exactly as described - by subtracting the disease rate among non-exposed from that among exposed.