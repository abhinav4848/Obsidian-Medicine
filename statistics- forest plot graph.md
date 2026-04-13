---
tags:
  - stats
aliases:
  - Forest Plot
urls:
  - "[Forest plot - Wikipedia](https://en.wikipedia.org/wiki/Forest_plot)"
cssclasses:
  - red-border
  - invert-image
---
*See [[statistics- graphical representations|Graphical representations of statistical data]]* 
![forest plot|404](https://upload.wikimedia.org/wikipedia/commons/f/f0/Generic_forest_plot.png)

Summary measure (centre line of diamond) and associated confidence intervals (lateral tips of diamond), and **solid** vertical line of no effect ([[statistics- risk reduction, nnt, odds ratio|OR]]=1).

- Bigger the square- Bigger the weight (meaningfulness) of the study & bigger the sample size. 
	- The further away a box is from 1, the larger effect size it has. 
- Horizontal lines are confidence intervals. Also seen as the difference between the numbers in the bracket. 
	- Narrow horizontal line means study has narrow CI & is more precise. It doesn't say about significance. 
	- if the horizontal lines cross 1.0, then it's not statistically significant. Odd's ratio is a ratio, so if the ratio is <1.0, then it's not significant. 
- If the diamond (pooled OR) is not crossing 1.0 -> overall effect is statistically significant 
- Statistical insignificant does not mean clinical insignificant. 
### Overall Effect (Diamond)
- At the bottom of the forest plot, a **diamond** represents the **pooled effect estimate** from all studies.
    - Width of the diamond = 95% CI for the overall effect.
    - If the diamond **does not touch the centre line**, the pooled effect is statistically significant.
### Examples

| Study | OR  | 95% CI  | Interpretation                          |
| ----- | --- | ------- | --------------------------------------- |
| A     | 3.0 | 0.9–10  | ❌ Not significant (CI crosses 1)        |
| B     | 1.8 | 1.5–2.1 | ✅ Significant (tight CI, no crossing 1) |

| Study | OR  | 95% CI  | Interpretation                        |
| ----- | --- | ------- | ------------------------------------- |
| A     | 2.5 | 2.4–2.6 | ✅ Very precise → **more significant** |
| B     | 3.5 | 1.2–6.0 | ✅ Significant but wide → less precise |


