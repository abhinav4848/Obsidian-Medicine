---
tags:
  - stats
revision counter: 1
revision notes: Sensitivity vs specificity
---
Patients and doctors need to know if a disease or condition is present or absent. Tests can be used to help us decide. Tests generally guide us by indicating how likely it is that the patient has the condition.  
  
In order to interpret test results we need to have a working knowledge of the statistics used to describe them.  

Contingency tables (also known as 2 * 2 tables, see below) are used to illustrate and calculate test statistics such as sensitivity. It would be unusual for a medical exam not to feature a question based around screening test statistics. Commit the following table to memory and spend time practising using it as you will be expected to make calculations using it in your exam.  
  
TP = true positive; FP = false positive; TN = true negative; FN = false negative  

|                   | **Disease present** | **Disease absent** |
| ----------------- | ------------------- | ------------------ |
| **Test positive** | TP                  | FP                 |
| **Test negative** | FN                  | TN                 |
 
The table below lists the main statistical terms used in relation to screening tests: 

| **Measure**                                     | **Formula**                     | **Plain english**                                                                          |
| ----------------------------------------------- | ------------------------------- | ------------------------------------------------------------------------------------------ |
| **Sensitivity**                                 | TP / (TP + FN )                 | Proportion of patients with the condition who have a positive test result                  |
| **Specificity**                                 | TN / (TN + FP)                  | Proportion of patients without the condition who have a negative test result               |
| **Positive predictive value**                   | TP / (TP + FP)                  | The chance that the patient has the condition if the diagnostic test is positive           |
| **Negative predictive value**                   | TN / (TN + FN)                  | The chance that the patient does not have the condition if the diagnostic test is negative |
| **Likelihood ratio for a positive test result** | sensitivity / (1 - specificity) | How much the odds of the disease increase when a test is positive                          |
| **Likelihood ratio for a negative test result** | (1 - sensitivity) / specificity | How much the odds of the disease decrease when a test is negative                          |
Positive and negative predictive values are prevalence dependent. 
Likelihood ratios are not prevalence dependent.  
![[stats- se, sp, ppv, npv.jpg|385]]
##### Precision
The precision quantifies a tests ability to produce the same measurements with repeated tests.

# Videos
|                         |                                                                                                                          |
| ----------------------- | ------------------------------------------------------------------------------------------------------------------------ |
| Arora Medical Education | [Statistics for the AKT](https://www.passmedicine.com/question/questions.php?q=0#)                                       |
| AT                      | [Biostatistics - Evaluation of Diagnostic Tests: Sensitivity & Specificity](https://www.youtube.com/watch?v=Sg6NKj3fYHM) |
| Medmastery              | [Positive Predictive Value - The role of prevalence](https://www.youtube.com/watch?v=SEcExAHTPqE)                        |
| ATP                     | [Biostatistics - Negative and Positive Predictive Values](https://www.youtube.com/watch?v=gRDh-PRmiq8)<br>               |

