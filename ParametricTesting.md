
Parametric Testing in Biostatistics

Parametric tests are statistical methods used to analyse numerical data, especially when assumptions about the population distribution are satisfied.
They are commonly used to compare means (averages) between groups or compare a sample mean with a known population value.
There are four important parametric tests to understand:

One-sample t-test
Two-sample (independent) t-test
Paired-sample t-test
Analysis of Variance (ANOVA)

1. One-sample t-test
Meaning: A one-sample t-test compares the mean of one sample with a known or hypothesised population mean.
Example:
A researcher wants to know whether the average haemoglobin level of 30 pregnant women differs from the standard reference value of 12 g/dL.

    Sample: 30 pregnant women.
    Sample mean: 11 g/dL.
    Hypothesised mean: 12 g/dL.
The researcher uses a one-sample t-test to determine whether the difference is statistically significant.
Simple interpretation
If p = 0.02:
    0.02 is less than 0.05.
    The sample mean is significantly different from 12 g/dL.
    Reject the null hypothesis.
When do we use it?
When comparing one sample mean with a known or hypothesised value.

2. Two-sample t-test (Independent t-test)
Meaning: An independent t-test compares the means of two separate, unrelated groups.
Example:
A researcher wants to compare the average blood pressure of:
    Group A: 30 patients receiving medication A.
    Group B: 30 patients receiving medication B.
The researcher uses an independent t-test to determine whether the mean blood pressure differs between the two groups.
When do we use it?
When comparing the means of two independent groups.

Other examples:
    Blood pressure in men versus women.
    Weight in smokers versus non-smokers.
    Haemoglobin in treatment A versus treatment B.

3. Paired-sample t-test
Meaning: A paired t-test compares the means of two related measurements from the same participants or matched pairs.
Example:
A researcher measures the blood pressure of 20 patients:
    Before treatment.
    After treatment.
The same patients are measured twice.
The paired t-test determines whether the average blood pressure changed significantly after treatment.
When do we use it?
    Before and after treatment.
    Before and after exercise.
    Blood glucose before and after medication.
    Weight before and after a dietary programme.
Important: For a paired t-test, normality is assessed on the differences between the paired measurements.

5. Analysis of Variance (ANOVA)
Meaning: ANOVA is a parametric test used to compare the means of three or more independent groups.
Example:
A researcher wants to compare the average blood glucose levels of patients receiving three different treatments.
    Group A: Diet programme.
    Group B: Exercise programme.
    Group C: Medication programme.
ANOVA determines whether there is a statistically significant difference between the group means.
When do we use ANOVA?
When comparing the means of three or more independent groups.
Other examples:
    Comparing blood pressure across three age groups.
    Comparing weight across three diet programmes.
    Comparing haemoglobin levels across four treatment groups.
Important: If ANOVA gives p less than 0.05, it means at least one group mean differs. It does not tell us which groups differ. We use post-hoc tests, such as Tukey's test, to identify the differences.

5. Comparison of the four parametric tests
   
How to choose the correct test
This table is especially important for examinations.

Test                        Number of groups/measurements                            Purpose
One-sample t-test           One sample                                              Compare sample mean with a known value                    
Independent t-test          Two independent groups                                  Compare two means
Paired t-test               Two related measurements                                Compare before and after  
ANOVA                       Three or more independent groups                        Compare three or more means

What is your research question?

One sample compared with a standard value?
One-sample t-test

Two different, unrelated groups?
Independent t-test

Same people measured twice?
Paired t-test

Three or more independent groups?
One-way ANOVA
	
7. Assumptions of parametric tests

Before using these tests, consider the following assumptions:
Data should be numerical (usually continuous).
Observations should be independent where required by the design.

Normality should be assessed appropriately:
One-sample t-test: Sample values.
Independent t-test: Values within each group or relevant residuals.
Paired t-test: Differences between paired measurements.
ANOVA: Model residuals within the groups.
Equal variances are generally required for the standard independent t-test and one-way ANOVA.
Check for influential outliers.
If variances are unequal, Welch's t-test or Welch's ANOVA may be appropriate.
	
8. Non-parametric alternatives              	
Parametric test                        Non-parametric alternative
One-sample t-test                      One-sample Wilcoxon signed-rank (under suitable assumptions)
Independent t-test                     Mann–Whitney U
Paired t-test                          Wilcoxon signed-rank
One-way ANOVA                          Kruskal–Wallis  
