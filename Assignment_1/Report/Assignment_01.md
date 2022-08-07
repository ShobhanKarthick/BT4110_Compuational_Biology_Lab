<h1 style="text-align:center">BT4110 - Assignment 01</h1>
<h2 style="text-align:center">BE19B009</h2>

### Question 1 & 2

PDBTM database was not working. Hence, fasta sequences were taken from Moodle

### Question 3 & 4

`cd-hit` was used in the local machine with the following commands

**For TMB_Redundant.fasta file,**

```cd-hit -i TMB_Redundant.fasta -o TMB_output.fasta -c 0.4 -n 2```

**For TMB_Redundant.fasta file,**

```cd-hit -i TMB_Redundant.fasta -o TMB_output.fasta -c 0.4 -n 2```

### Question 5-8

For questions 5, 6, 7, 8, functions have been written to get the **overall composition** and also retrieve the **compostion of each sequence** from the fasta file for TMB and TMH. Python functions were also written in order to find the absolute deviations with respect to TMB and TMH. Along with this, few other values such as *True Positives*, *False Negatives*, *True Negatives*, *False Positives* were also found. Using these values, **sensitivity**, **specificity** and **accuracy** was also found as shown below.

**Overall compostion of TMH:**


'T': 5.40
'S': 6.79
'N': 3.63
'P': 4.49
'Q': 3.37
'E': 4.82
'V': 7.44
'Y': 3.40
'I': 6.65
'F': 5.56
'R': 4.46
'W': 1.79
'A': 8.48
'H': 2.26
'L': 11.5
'G': 7.13
'M': 2.82
'D': 4.04
'K': 4.45
'C': 1.34


**Overall compostion of TMB:**

'S': 7.65
'G': 9.45
'F': 4.21
'E': 4.71
'H': 1.98
'Y': 4.87
'A': 7.87
'R': 5.03
'V': 6.13
'I': 4.09
'M': 1.57
'N': 6.07
'D': 6.65
'T': 6.68
'K': 4.72
'P': 3.80
'L': 7.93
'Q': 4.32
'W': 1.66
'C': 0.53


**True Positives (TP)**: 1238 
**True Negatives (TN)**: 128
**False Positives (FP)**: 17
**False Negatives (FN)**: 137

Using the below formulae, sensitivity, specificity and accuracy was found.

**Sensitivity** = $$ \frac{TP}{(TP+FN)} $$ <br>
**Specificity** = $$ \frac{TN}{(TN+FP)} $$ <br>
**Accuracy** = $$ \frac{(TP+TN)}{(TP+TN+FP+FN)} $$ <br>

The results were, 

**Sensitivity**: 90.03%
**Specificity**: 88.27%
**Accuracy**: 89.87%

### Question 9

The dataset was reduced by 50% and the same was repeated to obtain the following results.

**True Positives (TP)**: 620
**True Negatives (TN)**: 60
**False Positives (FP)**: 12
**False Negatives (FN)**: 67

Using the formulae from previous questions, sensitivity, specificity and accuracy was found again.

The results were, 

**Sensitivity**: 90.25%
**Specificity**: 83.33%
**Accuracy**: 89.59%

*When these 2 results are compared, there is only minimal difference however it is significant. To be precise, the specificity in the second case increased and accuracy and sensitivity has decreased. This thereby shows that, the whole dataset has to be used.*
