# 7. Analysis of Variance (ANOVA)

## Meaning of Analysis of Variance (ANOVA)

Analysis of Variance (ANOVA) is a parametric statistical test used to compare the means (averages) of three or more groups to determine whether there is a statistically significant difference between them.

ANOVA helps researchers determine whether the observed differences between group means are likely to represent real population differences or may have occurred due to random variation.

In biostatistics, ANOVA is commonly used to compare blood pressure, blood glucose levels, haemoglobin levels, body weight, and other medical measurements across different treatment groups.

## Purpose of ANOVA

The main purposes of ANOVA are:

1. To compare the means of three or more groups.
2. To determine whether at least one group mean differs significantly from the others.
3. To evaluate the effectiveness of different medical treatments.
4. To compare health outcomes between different populations.
5. To analyse differences between groups in medical and clinical research.

## Example in Biostatistics

A researcher wants to compare the average blood glucose levels of patients receiving three different treatments.

The participants are divided into three groups:

- Group A: Patients following a diet programme.
- Group B: Patients following an exercise programme.
- Group C: Patients receiving medication.

The researcher measures the blood glucose levels of all three groups.

ANOVA is used to determine whether there is a statistically significant difference between the average blood glucose levels of the three treatment groups.

## Hypotheses of ANOVA

ANOVA involves two main hypotheses:

**1. Null Hypothesis (H₀):**

There is no significant difference between the population means of all groups.

H₀: μ₁ = μ₂ = μ₃

**2. Alternative Hypothesis (H₁):**

At least one group mean is significantly different from the others.

H₁: Not all population means are equal.

**Important:** ANOVA does not tell us exactly which groups are different. It only indicates whether there is evidence that at least one group mean differs.

## Types of ANOVA

There are different types of ANOVA used in biostatistics:

### 1. One-Way ANOVA

One-way ANOVA is used to compare the means of three or more independent groups based on one independent variable (factor).

**Example:**

Comparing the average blood glucose levels of patients receiving three different treatments:

- Diet programme.
- Exercise programme.
- Medication.

### 2. Two-Way ANOVA

Two-way ANOVA is used to examine the effects of two independent variables (factors) on one continuous dependent variable.

It can also determine whether there is an interaction between the two independent variables.

**Example:**

A researcher investigates the effects of:

- Gender (male and female).
- Treatment type (medication A and medication B).

The outcome measured is blood pressure.

Two-way ANOVA determines whether gender, treatment type, or their interaction is associated with differences in average blood pressure.

### 3. Repeated Measures ANOVA

Repeated Measures ANOVA is used when the same participants are measured three or more times under different conditions or at different time points.

**Example:**

A researcher measures the blood pressure of the same patients:

- Before treatment.
- After one month.
- After three months.

It determines whether the average blood pressure changes significantly across the three measurements.

## Formula of One-Way ANOVA

The main test statistic used in ANOVA is the F-statistic.

\[
F = \frac{\text{Between-group variation}}{\text{Within-group variation}}
\]

Where:

- F = F-statistic.
- Between-group variation = Variation between the group means.
- Within-group variation = Variation among observations within each group.

**Interpretation:**

- A large F-value suggests that the differences between group means are large relative to the variation within groups.
- A small F-value suggests that the differences between group means are small relative to the variation within groups.

The p-value is then used to determine statistical significance.

<LearningViz type_id="ANOVA_DECOMPOSITION" locale_override="en-US"/>

## Interpretation of p-Value in ANOVA

The p-value helps determine whether there is a statistically significant difference between the group means.

- If p < 0.05: The result is statistically significant. Reject the null hypothesis.
- If p ≥ 0.05: The result is not statistically significant. Fail to reject the null hypothesis.

**Example:**

A researcher compares the average blood glucose levels of patients receiving three different treatments.

If the ANOVA produces:

p = 0.02

Interpretation:

- 0.02 is less than 0.05.
- The result is statistically significant.
- Reject the null hypothesis.
- There is sufficient evidence that at least one treatment group has a different population mean blood glucose level.

**Important:** A significant ANOVA result does not identify which specific groups differ. Post-hoc tests, such as Tukey's test, are used to investigate this.

## Assumptions of ANOVA

Before performing ANOVA, the following assumptions should be considered:

1. **Numerical data:** The dependent variable should be continuous and measured on an interval or ratio scale.

2. **Independence of observations:** Observations should be independent between participants and groups.

3. **Normality:** The model residuals should be approximately normally distributed within the groups.

4. **Homogeneity of variance:** The population variances should be approximately equal across the groups for standard one-way ANOVA.

5. **No influential outliers:** There should be no extreme values that strongly influence the results.

**Note:** If the equal-variance assumption is not satisfied, Welch's ANOVA may be an appropriate alternative.

## When Do We Use ANOVA?

ANOVA is commonly used in biostatistics when comparing the means of three or more independent groups.

Examples include:

- Comparing blood pressure across three age groups.
- Comparing average body weight across three dietary programmes.
- Comparing haemoglobin levels across four treatment groups.
- Comparing blood glucose levels among patients receiving different medications.
- Comparing cholesterol levels across different lifestyle groups.

## Advantages of ANOVA

1. Allows researchers to compare three or more group means simultaneously.
2. Reduces the need to perform multiple separate t-tests.
3. Helps identify whether significant differences exist between groups.
4. Useful for analysing clinical trial results.
5. Can be applied to different research designs, including one-way, two-way, and repeated measures ANOVA.

## Difference Between t-Test and ANOVA

| t-Test | ANOVA |
|---|---|
| Generally compares one or two means, depending on the type of t-test. | Compares three or more means in the usual one-way ANOVA application. |
| Uses a t-statistic. | Uses an F-statistic. |
| Example: Comparing blood pressure between two treatment groups. | Example: Comparing blood pressure between three treatment groups. |
| Can be used for independent or paired observations. | Can be used for independent groups or repeated measurements, depending on the ANOVA design. |

## Summary

Analysis of Variance (ANOVA) is a parametric statistical test used to compare the means of three or more groups.

The main types include:

1. One-Way ANOVA.
2. Two-Way ANOVA.
3. Repeated Measures ANOVA.

ANOVA determines whether at least one group mean differs significantly from the others. If the result is statistically significant, post-hoc tests can identify which specific groups differ.

**Remember for examinations:**

- Two independent groups = Independent t-Test.
- Three or more independent groups = One-Way ANOVA.
- Same participants measured three or more times = Repeated Measures ANOVA.

**Important:** A significant ANOVA result tells us that at least one mean differs, but it does not tell us exactly which groups are different.

# 12. Post-Hoc Tests (Tukey's Test and Other Methods)

## Meaning of Post-Hoc Tests

Post-hoc tests are statistical tests performed after obtaining a statistically significant result from ANOVA.

They are used to identify exactly which groups differ significantly from one another.

ANOVA tells researchers whether at least one group mean is different, but it does not identify which specific groups are responsible for the difference.

Therefore, post-hoc tests are used to make further comparisons between individual groups.

In biostatistics, post-hoc tests are commonly used to compare the effectiveness of different medications, treatments, dietary programmes, and medical interventions.

## Purpose of Post-Hoc Tests

The main purposes are:

1. To identify which specific groups differ significantly after ANOVA.
2. To compare group means individually.
3. To determine which treatment is more effective.
4. To reduce the risk of false-positive results caused by performing multiple comparisons.
5. To provide a more detailed interpretation of ANOVA results.

## Example in Biostatistics

A researcher wants to compare the average blood glucose levels of patients receiving three different treatments.

The participants are divided into three groups:

- Group A: Diet programme.
- Group B: Exercise programme.
- Group C: Medication programme.

The researcher performs a one-way ANOVA.

The ANOVA result is:

p = 0.01

Since 0.01 is less than 0.05, the result is statistically significant.

However, ANOVA does not tell the researcher which treatment groups have significantly different mean blood glucose levels.

The researcher therefore performs a post-hoc test to compare:

1. Group A versus Group B.
2. Group A versus Group C.
3. Group B versus Group C.

These comparisons help identify exactly where the differences exist.

## Common Types of Post-Hoc Tests

There are several post-hoc tests used in statistical analysis.

### 1. Tukey's Honestly Significant Difference (HSD) Test

**Meaning:**

Tukey's HSD test is a post-hoc statistical test used to compare all possible pairs of group means after a significant ANOVA result.

It controls the overall family-wise error rate when performing multiple pairwise comparisons.

**Example:**

A researcher compares the average blood pressure of patients receiving three medications:

- Medication A.
- Medication B.
- Medication C.

Tukey's test compares:

- A versus B.
- A versus C.
- B versus C.

It identifies which medication groups have significantly different average blood pressure levels.

**When do we use it?**

- After a significant one-way ANOVA.
- When comparing all possible pairs of group means.
- When the equal-variance assumption is reasonably satisfied.

### 2. Bonferroni Correction

**Meaning:**

The Bonferroni correction is a method used to adjust the significance level when performing multiple statistical comparisons.

It reduces the probability of obtaining false-positive results.

**Example:**

A researcher performs five statistical comparisons.

The original significance level is:

α = 0.05

Using the Bonferroni correction:

Adjusted significance level = 0.05 / 5

Adjusted significance level = 0.01

Each comparison must therefore have a p-value below 0.01 to be considered statistically significant under this correction.

**When do we use it?**

- When performing multiple comparisons.
- When controlling the risk of false-positive findings.
- When a relatively simple and conservative adjustment is required.

### 3. Scheffé's Test

**Meaning:**

Scheffé's test is a post-hoc method used to compare group means and more complex combinations of group means (contrasts).

It is relatively conservative and provides protection against false-positive findings across a broad range of comparisons.

**Example:**

A researcher compares the effects of four different treatments on patients' blood glucose levels.

Scheffé's test can be used to investigate differences between individual treatment groups or combinations of groups.

**When do we use it?**

- When many different comparisons are of interest.
- When comparing individual means and more complex contrasts.
- When a conservative method is preferred.

### 4. Dunnett's Test

**Meaning:**

Dunnett's test is a post-hoc statistical test used to compare several treatment groups against one control group.

Unlike Tukey's test, it does not compare every possible pair of groups.

**Example:**

A researcher investigates the effectiveness of three new medications compared with a placebo.

The groups are:

- Group A: Placebo (control).
- Group B: Medication A.
- Group C: Medication B.
- Group D: Medication C.

Dunnett's test compares:

- Medication A versus placebo.
- Medication B versus placebo.
- Medication C versus placebo.

**When do we use it?**

- When several treatment groups are compared with one control group.
- In clinical trials and medical research.

## Comparison of Common Post-Hoc Tests

| Post-hoc test | Main purpose |
|---|---|
| Tukey's HSD | Compares all possible pairs of group means. |
| Bonferroni correction | Adjusts significance levels for multiple comparisons. |
| Scheffé's test | Allows comparisons of individual means and complex contrasts. |
| Dunnett's test | Compares several treatment groups with one control group. |

## Interpretation of Post-Hoc Test Results

Post-hoc tests produce adjusted p-values to help determine whether individual group comparisons are statistically significant.

- If adjusted p < 0.05: The difference between the two groups is statistically significant.
- If adjusted p ≥ 0.05: There is insufficient evidence of a statistically significant difference between the two groups.

**Example:**

After performing ANOVA, a researcher uses Tukey's HSD test and obtains the following results:

| Comparison | Adjusted p-value | Interpretation |
|---|---|---|
| Group A vs Group B | 0.30 | Not significant |
| Group A vs Group C | 0.01 | Significant |
| Group B vs Group C | 0.02 | Significant |

**Interpretation:**

- Group A and Group B do not differ significantly.
- Group A and Group C differ significantly.
- Group B and Group C differ significantly.

Therefore, Group C has a significantly different mean from both Group A and Group B.

## When Should We Perform Post-Hoc Tests?

Post-hoc tests are generally performed when:

1. ANOVA has produced a statistically significant result.
2. The researcher wants to identify which specific groups differ.
3. Multiple pairwise comparisons are required.

**Important:** The choice of post-hoc test depends on the research question, study design, variance assumptions, and type of comparisons planned. If variances are unequal, methods such as Games-Howell may be more appropriate than Tukey's HSD.

## Difference Between ANOVA and Post-Hoc Tests

| ANOVA | Post-Hoc Tests |
|---|---|
| Compares three or more group means overall. | Identifies which specific groups differ. |
| Uses an F-statistic. | Uses adjusted pairwise comparisons or contrasts. |
| Determines whether at least one mean differs. | Determines where the differences exist. |
| Usually performed first. | Usually performed after a significant ANOVA result. |

## Advantages of Post-Hoc Tests

1. Identify specific differences between groups.
2. Provide more detailed information after ANOVA.
3. Help researchers compare different treatment outcomes.
4. Reduce the risk of false-positive results through appropriate multiple-comparison adjustments.
5. Support better interpretation of clinical research findings.

## Summary

Post-hoc tests are statistical methods performed after ANOVA to identify exactly which groups differ significantly.

The four commonly studied methods are:

1. Tukey's HSD: Compares all possible pairs of group means.
2. Bonferroni: Adjusts for multiple comparisons.
3. Scheffé's test: Allows comparisons of means and complex contrasts.
4. Dunnett's test: Compares several treatment groups with one control group.

**Remember for examinations:**

- ANOVA = Determines whether at least one group mean differs.
- Post-hoc tests = Identify which specific groups differ.

**Important examination tip:**

If a question asks which test compares all possible pairs of group means after ANOVA, the answer is Tukey's HSD test.


# 13. Interpretation of p-Values in Parametric Tests

## Meaning of p-Value

A p-value is a statistical measure used to determine whether the results of a study are statistically significant.

It indicates how likely it is to obtain the observed results, or results more extreme, if the null hypothesis (H₀) is assumed to be true.

In biostatistics, p-values are commonly used in parametric tests such as:

- One-Sample t-Test.
- Independent Two-Sample t-Test.
- Paired-Sample t-Test.
- Analysis of Variance (ANOVA).

## Purpose of p-Values

The main purposes are:

1. To determine whether the results are statistically significant.
2. To help researchers decide whether to reject or fail to reject the null hypothesis.
3. To evaluate whether an observed difference could reasonably be explained by random variation under the null hypothesis.
4. To support the interpretation of clinical and medical research findings.

## Understanding the Significance Level (α)

The significance level is the threshold used to determine whether a result is statistically significant.

The most commonly used significance level is:

α = 0.05 (5%)

This means that the researcher accepts a 5% risk of rejecting a true null hypothesis (Type I error).

Other commonly used significance levels include:

- 0.01 (1%).
- 0.05 (5%).
- 0.10 (10%).

## Interpretation of p-Values

There are two main situations:

### 1. When p < 0.05

The result is statistically significant.

- Reject the null hypothesis (H₀).
- There is sufficient statistical evidence against the null hypothesis.
- The observed result is unlikely under the null hypothesis.

**Example:**

If p = 0.02:

- 0.02 is less than 0.05.
- The result is statistically significant.
- Reject the null hypothesis.

### 2. When p ≥ 0.05

The result is not statistically significant.

- Fail to reject the null hypothesis (H₀).
- There is insufficient statistical evidence against the null hypothesis.
- The study has not demonstrated a statistically significant difference.

**Example:**

If p = 0.08:

- 0.08 is greater than 0.05.
- The result is not statistically significant.
- Fail to reject the null hypothesis.

**Important:** A non-significant result does not prove that there is no difference between the groups.

## Examples of p-Value Interpretation in Biostatistics

### Example 1: One-Sample t-Test

A researcher wants to determine whether the average haemoglobin level of pregnant women differs from the reference value of 12 g/dL.

Result:

p = 0.02

Interpretation:

- 0.02 is less than 0.05.
- The result is statistically significant.
- Reject the null hypothesis.
- There is sufficient evidence that the population mean haemoglobin level differs from 12 g/dL.

### Example 2: Independent Two-Sample t-Test

A researcher compares the average blood pressure of patients receiving medication A and medication B.

Result:

p = 0.03

Interpretation:

- 0.03 is less than 0.05.
- The result is statistically significant.
- Reject the null hypothesis.
- There is sufficient evidence of a difference in mean blood pressure between the two treatment groups.

### Example 3: Paired-Sample t-Test

A researcher measures the blood glucose levels of the same patients before and after treatment.

Result:

p = 0.01

Interpretation:

- 0.01 is less than 0.05.
- The result is statistically significant.
- Reject the null hypothesis.
- There is sufficient evidence that the mean blood glucose level changed after treatment.

### Example 4: ANOVA

A researcher compares the average blood glucose levels of patients receiving three different treatments.

Result:

p = 0.004

Interpretation:

- 0.004 is less than 0.05.
- The result is statistically significant.
- Reject the null hypothesis.
- There is sufficient evidence that at least one treatment group has a different population mean blood glucose level.

Post-hoc tests are needed to identify which specific groups differ.

## Summary Table of p-Value Interpretation

| p-Value | Interpretation | Decision |
|---|---|---|
| 0.001 | Highly statistically significant | Reject H₀ |
| 0.01 | Statistically significant | Reject H₀ |
| 0.02 | Statistically significant | Reject H₀ |
| 0.04 | Statistically significant | Reject H₀ |
| 0.05 | Not significant under the strict p < 0.05 rule | Fail to reject H₀ |
| 0.08 | Not statistically significant | Fail to reject H₀ |
| 0.10 | Not statistically significant | Fail to reject H₀ |
| 0.50 | Not statistically significant | Fail to reject H₀ |

## Difference Between Statistical Significance and Clinical Significance

**Statistical significance:**

Indicates whether the observed result provides sufficient evidence against the null hypothesis.

**Clinical significance:**

Indicates whether the observed difference is large enough to be meaningful or important for patient health and medical practice.

**Example:**

A new medication reduces blood pressure by an average of only 1 mmHg, with p = 0.001.

- The result is statistically significant.
- However, a reduction of 1 mmHg may have limited clinical importance for an individual patient.

Therefore, statistical significance does not automatically mean clinical importance.

## Important Things to Remember About p-Values

1. A p-value below 0.05 is commonly considered statistically significant.
2. A p-value equal to or above 0.05 is not statistically significant under the conventional 0.05 threshold.
3. A p-value does not measure the size of an effect.
4. A p-value does not indicate the probability that the null hypothesis is true.
5. A small p-value does not automatically mean that the finding is clinically important.
6. A large p-value does not prove that there is no difference.
7. Results should also be interpreted using effect sizes and confidence intervals.

## Summary

The p-value helps researchers determine whether the results of a parametric statistical test are statistically significant.

The conventional significance level is 0.05.

**Remember for examinations:**

- p < 0.05 = Statistically significant = Reject H₀.
- p ≥ 0.05 = Not statistically significant = Fail to reject H₀.

**Important examination tip:**

Never say that you accept the null hypothesis when p ≥ 0.05. The correct expression is: "Fail to reject the null hypothesis."

markdown

# 14. How to Choose the Correct Statistical Test

## Meaning of Choosing the Correct Statistical Test

Choosing the correct statistical test means selecting an appropriate statistical method to analyse data and answer a research question.

The choice depends on several factors, including:

- The type of data collected.
- The number of groups being compared.
- Whether the groups are independent or related.
- The research question.
- Whether the assumptions of the statistical test are satisfied.

In biostatistics, selecting the correct test is important because it helps researchers obtain valid and reliable results.

## Factors to Consider When Choosing a Statistical Test

### 1. Type of Data

The first step is to identify the type of data collected.

There are two main types:

**A. Numerical Data**

Numerical data represent measurable quantities.

Examples:
- Blood pressure.
- Blood glucose levels.
- Haemoglobin levels.
- Body weight.
- Height.
- Cholesterol levels.

Parametric tests are commonly used to analyse numerical data when their assumptions are satisfied.

**B. Categorical Data**

Categorical data represent groups or categories.

Examples:
- Gender.
- Blood group.
- Smoking status.
- Disease status.
- Treatment category.

Categorical data are commonly analysed using tests such as the Chi-square test or Fisher's exact test.

### 2. Number of Groups

The number of groups or measurements being compared is another important factor.

- One sample compared with a known value: One-Sample t-Test.
- Two independent groups: Independent Two-Sample t-Test.
- Two related measurements: Paired-Sample t-Test.
- Three or more independent groups: One-Way ANOVA.
- Three or more related measurements: Repeated Measures ANOVA.

### 3. Relationship Between Groups

Researchers must determine whether the groups are independent or related.

**A. Independent Groups**

Independent groups consist of different participants who belong to separate groups.

Example:
- Group A: Patients receiving medication A.
- Group B: Patients receiving medication B.

Correct test: Independent Two-Sample t-Test.

**B. Related Groups**

Related groups involve the same participants measured more than once or appropriately matched individuals.

Example:
- Blood pressure before treatment.
- Blood pressure after treatment.

Correct test: Paired-Sample t-Test.

### 4. Distribution of Data

Researchers should consider whether the data or relevant model residuals are approximately normally distributed.

- If the assumptions of normality and other required conditions are satisfied, a parametric test may be appropriate.
- If the assumptions are seriously violated, a suitable non-parametric alternative may be considered.

### 5. Equality of Variances

When comparing independent groups, researchers should consider whether the population variances are approximately equal.

- Equal variances: Standard Independent t-Test or One-Way ANOVA may be appropriate.
- Unequal variances: Welch's t-Test or Welch's ANOVA may be appropriate.

## Choosing the Correct Parametric Test

The following table helps identify the appropriate parametric test.

| Research situation | Correct statistical test |
|---|---|
| One sample compared with a known value | One-Sample t-Test |
| Two independent groups compared | Independent Two-Sample t-Test |
| Two related measurements compared | Paired-Sample t-Test |
| Three or more independent groups compared | One-Way ANOVA |
| Effects of two independent factors examined | Two-Way ANOVA |
| Same participants measured three or more times | Repeated Measures ANOVA |

## Examples in Biostatistics

### Example 1: One-Sample t-Test

Research question:

Is the average haemoglobin level of pregnant women different from the standard reference value of 12 g/dL?

Correct test:

One-Sample t-Test.

Reason:

One sample is compared with a known reference value.

### Example 2: Independent Two-Sample t-Test

Research question:

Is there a difference in average blood pressure between patients receiving medication A and medication B?

Correct test:

Independent Two-Sample t-Test.

Reason:

Two separate and unrelated groups are compared.

### Example 3: Paired-Sample t-Test

Research question:

Does medication reduce the blood glucose level of patients?

The same patients are measured before and after treatment.

Correct test:

Paired-Sample t-Test.

Reason:

The same participants are measured twice.

### Example 4: One-Way ANOVA

Research question:

Is there a difference in average blood glucose levels among patients receiving three different treatments?

Correct test:

One-Way ANOVA.

Reason:

Three independent groups are compared using one factor.

### Example 5: Repeated Measures ANOVA

Research question:

Does the average blood pressure of patients change over three different measurement periods?

The same patients are measured:

- Before treatment.
- After one month.
- After three months.

Correct test:

Repeated Measures ANOVA.

Reason:

The same participants are measured three or more times.

### Example 6: Two-Way ANOVA

Research question:

Do gender and treatment type influence average blood pressure?

Correct test:

Two-Way ANOVA.

Reason:

Two independent factors are examined in relation to one numerical outcome.

## Simple Decision Guide for Choosing the Correct Test

Ask yourself the following questions:

**Question 1: Are you comparing one sample with a known or hypothesised value?**

- Yes → One-Sample t-Test.

**Question 2: Are you comparing two different and unrelated groups?**

- Yes → Independent Two-Sample t-Test.

**Question 3: Are you comparing the same participants twice?**

- Yes → Paired-Sample t-Test.

**Question 4: Are you comparing three or more independent groups?**

- Yes → One-Way ANOVA.

**Question 5: Are you comparing the same participants three or more times?**

- Yes → Repeated Measures ANOVA.

**Question 6: Are you examining the effects of two independent factors?**

- Yes → Two-Way ANOVA.

## Quick Comparison Table for Examinations

| Situation | Statistical test |
|---|---|
| One sample vs. standard value | One-Sample t-Test |
| Two unrelated groups | Independent t-Test |
| Same people before and after treatment | Paired t-Test |
| Three or more unrelated groups | One-Way ANOVA |
| Two independent factors | Two-Way ANOVA |
| Same people measured three or more times | Repeated Measures ANOVA |

## Important: What If Parametric Assumptions Are Not Satisfied?

If the assumptions of a parametric test are seriously violated, researchers may consider non-parametric alternatives.

| Parametric test | Non-parametric alternative |
|---|---|
| One-Sample t-Test | One-Sample Wilcoxon Signed-Rank Test (under suitable assumptions) |
| Independent t-Test | Mann–Whitney U Test |
| Paired-Sample t-Test | Wilcoxon Signed-Rank Test |
| One-Way ANOVA | Kruskal–Wallis Test |
| Repeated Measures ANOVA | Friedman Test |

The choice of an alternative also depends on the data structure and research question.

## Summary

Choosing the correct statistical test depends on the type of data, number of groups, relationship between observations, and statistical assumptions.

**Remember for examinations:**

1. One sample + reference value = One-Sample t-Test.
2. Two independent groups = Independent t-Test.
3. Same people measured twice = Paired-Sample t-Test.
4. Three or more independent groups = One-Way ANOVA.
5. Same people measured three or more times = Repeated Measures ANOVA.
6. Two independent factors = Two-Way ANOVA.

**Important examination tip:**

Before selecting a statistical test, always ask:

- What type of data do I have?
- How many groups am I comparing?
- Are the groups independent or related?
- Are the assumptions of the test satisfied?

These four questions will help you choose the correct statistical test in most basic biostatistics examination questions.


markdown

```markdown
# 15. Assumptions of Parametric Tests

## Meaning of Assumptions of Parametric Tests

Assumptions of parametric tests are the conditions that should be satisfied for statistical tests to produce valid and reliable results.

Parametric tests are statistical methods used to analyse numerical data, particularly when comparing means (averages) between groups or comparing a sample mean with a known population value.

Before performing a parametric test, researchers should check whether the data meet the required assumptions.

In biostatistics, these assumptions are important when analysing medical measurements such as blood pressure, blood glucose levels, haemoglobin levels, body weight, and cholesterol levels.

## Main Assumptions of Parametric Tests

There are five important assumptions commonly considered when performing parametric tests.

### 1. Numerical Data (Continuous Data)

Parametric tests are generally used with numerical data, particularly continuous data measured on an interval or ratio scale.

Examples:
- Blood pressure.
- Blood glucose levels.
- Haemoglobin levels.
- Body weight.
- Height.
- Cholesterol levels.

**Example:**

A researcher wants to compare the average blood pressure of two groups of patients.

Blood pressure is numerical data, so an appropriate parametric test may be used if the other assumptions are satisfied.

### 2. Normality (Normal Distribution)

Normality means that the data or relevant model residuals should follow an approximately normal, bell-shaped distribution.

A normal distribution is symmetrical around the mean, with most observations concentrated near the centre.

**Example:**

A researcher measures the haemoglobin levels of 50 healthy individuals.

If the measurements are approximately normally distributed, a parametric test may be appropriate.

**How can normality be checked?**

- Histogram.
- Q-Q plot (Quantile-Quantile plot).
- Shapiro-Wilk test.

**Important:** Normality must be assessed differently depending on the statistical test:

- One-Sample t-Test: Sample values.
- Independent t-Test: Values within each group or relevant model residuals.
- Paired-Sample t-Test: Differences between paired measurements.
- ANOVA: Model residuals.

### 3. Independence of Observations

Independence means that one observation should not influence another observation in a way that violates the study design assumptions.

For independent-group tests, participants in one group should not be treated as independent observations of participants in another group if the measurements are actually related.

**Example:**

A researcher compares the blood pressure of:

- Group A: 30 different patients receiving medication A.
- Group B: 30 different patients receiving medication B.

The observations should be independent between participants.

**Important:**

In a paired-sample t-test, the two measurements from the same person are intentionally related. However, the differences between different participants should be independent.

### 4. Homogeneity of Variance (Equal Variances)

Homogeneity of variance means that the groups being compared should have approximately equal population variances.

Variance measures how spread out the observations are around the mean.

**Example:**

A researcher compares the blood pressure of patients receiving three different treatments.

The standard one-way ANOVA assumes that the population variances are approximately equal across the three treatment groups.

**How can equal variances be checked?**

- Levene's test.
- Brown-Forsythe test.
- Comparison of group variances.

**Interpretation of Levene's test:**

- If p > 0.05: There is insufficient evidence that the group variances differ.
- If p < 0.05: There is evidence that the group variances differ.

**Important:**

Equal variances are generally required for:

- Standard Independent Two-Sample t-Test.
- Standard One-Way ANOVA.

If variances are unequal, researchers may use:

- Welch's t-Test.
- Welch's ANOVA.

### 5. Absence of Influential Outliers

Outliers are unusually high or low observations that differ considerably from the other values in a dataset.

Extreme observations can influence the sample mean, standard deviation, and statistical test results.

**Example:**

A researcher measures the body weight of 20 patients.

Most patients weigh between 50 kg and 85 kg, but one patient weighs 180 kg.

This observation may be an outlier and should be investigated.

**How can outliers be identified?**

- Box plots.
- Scatter plots.
- Examination of the raw data.
- Standardised residuals, where appropriate.

**Important:** Outliers should not automatically be removed. Researchers should investigate whether they are genuine observations, measurement errors, or data-entry mistakes.

## Normality and Different Parametric Tests

Normality is one of the most important assumptions, but it is not checked in exactly the same way for every test.

| Parametric test | What should be approximately normally distributed? |
|---|---|
| One-Sample t-Test | Sample values |
| Independent t-Test | Values within each group or model residuals |
| Paired-Sample t-Test | Differences between paired measurements |
| One-Way ANOVA | Model residuals within the groups |
| Repeated Measures ANOVA | Relevant model residuals and, additionally, sphericity |

## Summary Table of Assumptions

| Assumption | Meaning |
|---|---|
| Numerical data | Data should generally be continuous and numerical. |
| Normality | Relevant data or model residuals should be approximately normally distributed. |
| Independence | Observations or independent units should be independent as required by the study design. |
| Homogeneity of variance | Group variances should be approximately equal for standard independent-group tests. |
| No influential outliers | Extreme values should not unduly influence the results. |

## What Happens If the Assumptions Are Not Satisfied?

If the assumptions of a parametric test are seriously violated, researchers may consider alternative statistical methods.

Examples:

| Parametric test | Possible alternative |
|---|---|
| One-Sample t-Test | One-Sample Wilcoxon Signed-Rank Test |
| Independent t-Test | Mann-Whitney U Test |
| Paired-Sample t-Test | Wilcoxon Signed-Rank Test |
| One-Way ANOVA | Kruskal-Wallis Test |
| Repeated Measures ANOVA | Friedman Test |

However, the choice of an alternative depends on the type of violation and the research question.

For example, if equal variances are violated but other assumptions are reasonably satisfied, Welch's t-test or Welch's ANOVA may be preferable to switching directly to a non-parametric test.

## Importance of Checking Assumptions

Checking assumptions is important because it helps researchers:

1. Obtain valid statistical results.
2. Reduce the risk of incorrect conclusions.
3. Select the appropriate statistical test.
4. Improve the reliability of research findings.
5. Make accurate interpretations of medical and clinical data.

## Summary

Parametric tests are based on certain statistical assumptions that should be considered before analysing numerical data.

The five main assumptions are:

1. Numerical data.
2. Normality.
3. Independence of observations.
4. Homogeneity of variance.
5. Absence of influential outliers.

**Remember for examinations:**

- Normality = Approximately normal distribution.
- Independence = Observations are independent where required.
- Homogeneity of variance = Approximately equal group variances.
- Outliers = Extreme values that may influence results.

**Very Important Examination Tip:**

For a paired-sample t-test, normality is checked on the differences between the paired measurements, not on the individual measurements.

For ANOVA, normality is assessed using the model residuals, not simply by checking whether all the raw data combined follow a normal distribution.
```

# 16. Normality and the Normal Distribution

## Meaning of Normality

Normality is a statistical assumption that means numerical data or relevant model residuals follow an approximately normal distribution.

It is one of the important assumptions of many parametric statistical tests, including:

- One-Sample t-Test.
- Independent Two-Sample t-Test.
- Paired-Sample t-Test.
- Analysis of Variance (ANOVA).

Normality is important because it helps ensure that statistical tests produce reliable results, particularly when sample sizes are small.

## Meaning of Normal Distribution

A normal distribution is a continuous probability distribution in which data are symmetrically distributed around the mean.

It is also called a bell-shaped curve because its shape resembles a bell.

In a normal distribution:

- Most observations are concentrated around the mean.
- Fewer observations occur as we move away from the mean.
- The distribution is symmetrical on both sides.
- The mean, median, and mode are equal.

## Characteristics of a Normal Distribution

A normal distribution has the following characteristics:

1. **Bell-shaped curve:** The distribution has a bell-shaped appearance.

2. **Symmetrical distribution:** Both sides of the curve are approximately identical.

3. **Mean = Median = Mode:** The three measures of central tendency have the same value.

4. **Equal tails:** Both ends of the distribution extend in opposite directions and approach, but never touch, the horizontal axis.

5. **Total area = 1:** The total area under the normal distribution curve represents 100% probability.

6. **Defined by two parameters:** A normal distribution is described by its mean (μ) and standard deviation (σ).

## Visual Representation of Normal Distribution

<LearningViz type_id="STANDARD_SCORE_Z" locale_override="en-US"/>

## The 68–95–99.7 Rule (Empirical Rule)

The empirical rule explains how data are distributed around the mean in a normal distribution.

Approximately:

- **68%** of observations fall within one standard deviation of the mean (±1 SD).
- **95%** of observations fall within two standard deviations of the mean (±2 SD).
- **99.7%** of observations fall within three standard deviations of the mean (±3 SD).

**Example:**

Suppose the average haemoglobin level in a population is 12 g/dL, with a standard deviation of 1 g/dL.

The distribution is assumed to be normal.

- Approximately 68% of individuals have haemoglobin levels between 11 and 13 g/dL.
- Approximately 95% have levels between 10 and 14 g/dL.
- Approximately 99.7% have levels between 9 and 15 g/dL.

## Importance of Normality in Parametric Tests

Normality is important because many parametric tests rely on the assumption that the relevant data or model residuals are approximately normally distributed.

It helps researchers:

1. Choose appropriate statistical tests.
2. Obtain reliable statistical conclusions.
3. Calculate accurate confidence intervals and p-values.
4. Compare means between different groups.
5. Interpret medical and clinical research findings correctly.

## How to Check Normality

Researchers can use graphical and statistical methods to assess normality.

### 1. Histogram

A histogram displays the frequency distribution of numerical data.

If the histogram has an approximately symmetrical, bell-shaped appearance, the data may be normally distributed.

### 2. Q-Q Plot (Quantile-Quantile Plot)

A Q-Q plot compares the observed data quantiles with the expected quantiles of a normal distribution.

- If the points follow approximately a straight diagonal line, the data may be normally distributed.
- If the points show substantial deviations from the line, the data may not be normally distributed.

### 3. Shapiro-Wilk Test

The Shapiro-Wilk test is a statistical test used to assess whether data are consistent with a normal distribution.

Interpretation:

- If p > 0.05: There is insufficient evidence to reject the assumption of normality.
- If p < 0.05: There is evidence that the data deviate from a normal distribution.

**Important:** A p-value greater than 0.05 does not prove that the data are normally distributed.

## Normality in Different Parametric Tests

Normality is not assessed in exactly the same way for every parametric test.

| Parametric test | What should be approximately normally distributed? |
|---|---|
| One-Sample t-Test | Sample values |
| Independent t-Test | Values within each group or relevant model residuals |
| Paired-Sample t-Test | Differences between paired measurements |
| One-Way ANOVA | Model residuals within groups |
| Repeated Measures ANOVA | Relevant model residuals, with additional assumptions such as sphericity |

## What Happens If Data Are Not Normally Distributed?

If data are not normally distributed, researchers should first consider:

1. The sample size.
2. The presence of extreme outliers.
3. The shape and severity of the distribution.
4. Whether the test is reasonably robust to departures from normality.

Depending on the situation, researchers may consider:

- Data transformation, such as logarithmic transformation.
- A suitable non-parametric test.
- A robust statistical method.

Examples of non-parametric alternatives include:

| Parametric test | Non-parametric alternative |
|---|---|
| One-Sample t-Test | One-Sample Wilcoxon Signed-Rank Test |
| Independent t-Test | Mann-Whitney U Test |
| Paired-Sample t-Test | Wilcoxon Signed-Rank Test |
| One-Way ANOVA | Kruskal-Wallis Test |
| Repeated Measures ANOVA | Friedman Test |

**Important:** A large sample size can make t-tests and ANOVA more robust to moderate departures from normality, but it does not automatically solve problems caused by severe outliers or other assumption violations.

## Difference Between Normality and Normal Distribution

| Normality | Normal Distribution |
|---|---|
| Refers to the assumption that data follow an approximately normal distribution. | Refers to a specific probability distribution. |
| It is a condition considered before using certain statistical tests. | It describes the shape and properties of the data distribution. |
| Can be assessed using histograms, Q-Q plots, and statistical tests. | Has a symmetrical, bell-shaped curve. |

## Summary

Normality is an important assumption in parametric testing. It means that the relevant data or model residuals should follow an approximately normal distribution.

A normal distribution is symmetrical and bell-shaped, with the mean, median, and mode having the same value.

**Remember for examinations:**

- Normal distribution = Bell-shaped and symmetrical curve.
- Mean = Median = Mode.
- 68% = Within ±1 SD.
- 95% = Within ±2 SD.
- 99.7% = Within ±3 SD.
- Shapiro-Wilk p > 0.05 = No statistically significant evidence against normality.

**Very Important Examination Tip:**

For a paired-sample t-test, check the normality of the differences between measurements, not the individual measurements.

For ANOVA, assess the normality of the model residuals rather than simply testing all observations combined.

markdown

```markdown
# 17. Homogeneity of Variance (Equal Variances)

## Meaning of Homogeneity of Variance

Homogeneity of variance is a statistical assumption stating that the variances of different groups being compared should be approximately equal.

In simple terms, it means that the spread or variation of numerical measurements should be similar across the groups.

This assumption is important in parametric statistical tests, particularly:

- Independent Two-Sample t-Test (standard Student's t-test).
- One-Way ANOVA.
- Two-Way ANOVA.

## Understanding Variance

Variance is a statistical measure that describes how far individual observations are spread out from the mean (average).

- Low variance: Data values are close to the mean.
- High variance: Data values are widely spread out from the mean.

For example:

Two groups of patients have the following blood pressure measurements:

**Group A:**
120, 122, 124, 126, 128

**Group B:**
121, 123, 125, 127, 129

Both groups have similar variability, suggesting that their variances are approximately equal.

However, if Group B had measurements of:

100, 110, 125, 140, 150

Its variability would be much greater than Group A.

This would suggest unequal variances.

<LearningViz type_id="VARIANCE" locale_override="en-US"/>

## Purpose of Homogeneity of Variance

The main purposes are:

1. To ensure that group variances are approximately equal.
2. To help select the correct parametric statistical test.
3. To improve the reliability of statistical results.
4. To reduce the risk of incorrect statistical conclusions.
5. To determine whether standard t-tests and ANOVA are appropriate.

## Example in Biostatistics

A researcher wants to compare the average blood glucose levels of patients receiving three different treatments.

The participants are divided into:

- Group A: Diet programme.
- Group B: Exercise programme.
- Group C: Medication programme.

Before performing a standard one-way ANOVA, the researcher checks whether the variances of blood glucose levels are approximately equal across the three groups.

If the variances are approximately equal, the homogeneity of variance assumption is satisfied.

If the variances are substantially different, the researcher may consider Welch's ANOVA.

## How to Check Homogeneity of Variance

There are several methods used to assess whether group variances are equal.

### 1. Levene's Test

Levene's test is a statistical test used to determine whether the variances of two or more groups are approximately equal.

It is commonly used before performing independent t-tests and ANOVA.

**Hypotheses:**

Null Hypothesis (H₀):

The variances of all groups are equal.

Alternative Hypothesis (H₁):

At least one group has a different variance.

**Interpretation of Levene's Test:**

- If p > 0.05: There is insufficient evidence that the group variances differ. The equal-variance assumption is considered reasonable.
- If p < 0.05: There is evidence that the group variances differ. The equal-variance assumption may be violated.

**Example:**

A researcher performs Levene's test before comparing blood pressure across three treatment groups.

Result:

p = 0.32

Interpretation:

- 0.32 is greater than 0.05.
- There is insufficient evidence of unequal variances.
- The homogeneity of variance assumption is considered satisfied.

### 2. Brown-Forsythe Test

The Brown-Forsythe test is another statistical method used to assess equality of variances.

It is based on deviations from group medians and is more resistant to non-normality than the traditional Levene's test based on group means.

### 3. Comparing Group Variances

Researchers can also compare the spread of observations across groups using:

- Box plots.
- Standard deviations.
- Variance estimates.
- Graphical examination of the data.

These methods help identify whether the variability is similar across groups.

## What Happens If Homogeneity of Variance Is Violated?

If the variances of the groups are substantially different, the standard parametric test may not be appropriate.

Researchers can consider alternative statistical methods.

**1. Welch's t-Test**

Used when comparing the means of two independent groups with unequal variances.

**2. Welch's ANOVA**

Used when comparing the means of three or more independent groups with unequal variances.

These tests do not require the equal-variance assumption.

## Difference Between Equal and Unequal Variances

| Equal Variances | Unequal Variances |
|---|---|
| Groups have approximately similar variability. | Groups have substantially different variability. |
| Homogeneity of variance assumption is satisfied. | Homogeneity of variance assumption is violated. |
| Standard Student's t-test may be appropriate. | Welch's t-test may be appropriate. |
| Standard One-Way ANOVA may be appropriate. | Welch's ANOVA may be appropriate. |

## When Is Homogeneity of Variance Important?

This assumption is particularly important when:

- Comparing blood pressure between two independent treatment groups.
- Comparing blood glucose levels across three different treatment groups.
- Comparing haemoglobin levels between different populations.
- Evaluating the effectiveness of several medical treatments.

**Important:** Homogeneity of variance is not a general requirement of every parametric test.

For example:
- One-Sample t-Test does not require comparing variances between groups.
- Paired-Sample t-Test does not require equal variances between the two measurements.
- Standard Independent t-Test assumes equal population variances.
- Standard One-Way ANOVA assumes equal population variances across groups.

## Summary

Homogeneity of variance is an important assumption of certain parametric tests.

It means that the groups being compared should have approximately equal variances.

The most commonly used statistical test for checking this assumption is Levene's test.

**Remember for examinations:**

- p > 0.05 in Levene's test = No significant evidence of unequal variances.
- p < 0.05 in Levene's test = Evidence of unequal variances.
- Equal variances = Standard Student's t-test or standard ANOVA may be appropriate.
- Unequal variances = Consider Welch's t-test or Welch's ANOVA.

**Important examination tip:**

Homogeneity of variance means equal spread or variability between groups. It does NOT mean that the group means must be equal.
```

markdown

```markdown
# 18. Independence of Observations and Outliers

Independence of observations and the absence of influential outliers are two important considerations when performing parametric statistical tests.

They help ensure that statistical results are reliable and that researchers make appropriate conclusions from their data.

# Part A: Independence of Observations

## Meaning of Independence of Observations

Independence of observations means that one observation should not influence another observation.

In simple terms, each participant's measurement should be independent of the measurements of other participants, unless the statistical method specifically accounts for their relationship.

This assumption is important in parametric tests such as:

- One-Sample t-Test.
- Independent Two-Sample t-Test.
- Analysis of Variance (ANOVA).

## Purpose of Independence of Observations

The main purposes are:

1. To ensure that each observation provides independent information.
2. To prevent misleading statistical results.
3. To improve the reliability of statistical conclusions.
4. To ensure that the selected statistical test is appropriate for the study design.

## Example in Biostatistics

A researcher wants to compare the average blood pressure of two groups of patients.

- Group A: 30 patients receiving medication A.
- Group B: 30 patients receiving medication B.

For an independent two-sample t-test, the participants in Group A should be different from those in Group B.

Each patient's blood pressure measurement should also be independent of the measurements of other patients.

If the same patients are included in both groups, the independence assumption is violated because the observations are related.

## Examples of Independent and Dependent Observations

### 1. Independent Observations

Different individuals are measured in separate groups.

Example:

- Group A: Blood pressure of 20 men.
- Group B: Blood pressure of 20 different women.

The observations are independent if the participants' measurements do not influence one another.

### 2. Dependent (Related) Observations

The same individuals are measured more than once.

Example:

- Blood pressure before treatment.
- Blood pressure after treatment.

These measurements are related because they come from the same patients.

A paired-sample t-test is appropriate because it accounts for this relationship.

## How to Ensure Independence of Observations

Researchers can improve independence by:

1. Selecting participants appropriately.
2. Avoiding unnecessary duplication of participants.
3. Using suitable sampling methods.
4. Ensuring that participants are not incorrectly treated as independent when they belong to related groups.
5. Considering clustering, such as patients treated within the same hospital or clinic.

**Important:** Independence is mainly determined by the research design, not by a statistical test performed after data collection.

## What Happens If Independence Is Violated?

If observations are dependent but analysed as independent, the standard errors, p-values, and confidence intervals may be incorrect.

This can lead to misleading statistical conclusions.

Researchers may need to use methods that account for the relationship, such as:

- Paired-Sample t-Test.
- Repeated Measures ANOVA.
- Mixed-Effects Models.
- Cluster-adjusted statistical methods.

# Part B: Outliers

## Meaning of Outliers

Outliers are observations that are unusually high or low compared with most other values in a dataset.

They are measurements that differ considerably from the general pattern of the data.

Outliers can influence the mean, standard deviation, and results of parametric statistical tests.

## Purpose of Identifying Outliers

The main purposes are:

1. To identify unusual observations.
2. To prevent extreme values from misleading the analysis.
3. To improve the reliability of statistical results.
4. To detect possible measurement or data-entry errors.
5. To determine whether the selected statistical test is appropriate.

## Example in Biostatistics

A researcher measures the body weight of five patients.

The measurements are:

60 kg, 62 kg, 64 kg, 65 kg, 180 kg.

Most patients weigh between 60 kg and 65 kg.

However, one patient weighs 180 kg.

The value of 180 kg is unusually high compared with the other measurements and may be an outlier.

The researcher should investigate whether this value is correct before performing statistical analysis.

## How to Identify Outliers

There are several methods used to identify outliers.

### 1. Box Plot

A box plot is a graphical method used to identify unusually high or low observations.

It displays:

- Median.
- First quartile (Q1).
- Third quartile (Q3).
- Interquartile range (IQR).
- Potential outliers.

Values outside the whiskers are commonly marked as potential outliers.

### 2. Interquartile Range (IQR) Method

The interquartile range is the difference between the third quartile and the first quartile.

Formula:

IQR = Q3 − Q1

Where:

- Q1 = First quartile (25th percentile).
- Q3 = Third quartile (75th percentile).
- IQR = Interquartile range.

The common rule for identifying potential outliers is:

- Lower boundary = Q1 − 1.5 × IQR.
- Upper boundary = Q3 + 1.5 × IQR.

Any observation below the lower boundary or above the upper boundary is considered a potential outlier.

### 3. Z-Score Method

A Z-score indicates how many standard deviations an observation is from the mean.

Formula:

Z = (X − μ) / σ

Where:

- Z = Z-score.
- X = Individual observation.
- μ = Population mean.
- σ = Population standard deviation.

A common guideline is:

- Z-score greater than +3: Potentially unusually high observation.
- Z-score less than −3: Potentially unusually low observation.

This is a guideline, not a universal rule, and is most suitable when the distribution is approximately normal.

### 4. Scatter Plot

A scatter plot displays individual observations as points.

It helps researchers identify values that are far away from the general pattern of the data.

## Effects of Outliers on Parametric Tests

Outliers can affect statistical analysis in several ways:

1. They can increase or decrease the sample mean.
2. They can increase the standard deviation.
3. They can affect the assumption of normality.
4. They can influence the calculated t-statistic or F-statistic.
5. They can produce misleading p-values and confidence intervals.

**Example:**

If one patient has an extremely high blood glucose measurement, it may increase the average blood glucose level of the group and influence the statistical comparison.

## What Should Researchers Do When Outliers Are Found?

When an outlier is identified, researchers should:

1. Check whether the value was entered incorrectly.
2. Investigate whether there was a measurement error.
3. Determine whether the observation is a genuine value.
4. Assess how strongly it influences the statistical results.
5. Consider an appropriate robust or alternative statistical method if necessary.

**Important:** Outliers should not automatically be removed. Genuine extreme observations may contain important medical information.

# Difference Between Independence of Observations and Outliers

| Independence of Observations | Outliers |
|---|---|
| Refers to the relationship between observations. | Refers to unusually high or low observations. |
| One observation should not influence another where independence is required. | An observation differs considerably from the general pattern of the data. |
| Mainly depends on the study design. | Can be identified using statistical and graphical methods. |
| Violation can produce incorrect standard errors and p-values. | Can influence means, standard deviations, and test results. |
| Example: The same patients incorrectly treated as two independent groups. | Example: One patient has an unusually high blood pressure measurement. |

# Summary

Independence of observations and the absence of influential outliers are important considerations in parametric testing.

**1. Independence of Observations:**

Means that observations should be independent of one another where required by the statistical test.

**2. Outliers:**

Are unusually high or low values that may influence statistical results.

Common methods for identifying outliers include:

- Box plots.
- Interquartile Range (IQR).
- Z-scores.
- Scatter plots.

**Remember for examinations:**

- Independence = Observations should not influence one another.
- Related measurements from the same people = Use an appropriate paired or repeated-measures test.
- Outliers = Unusually high or low observations.
- IQR = Q3 − Q1.
- Potential outlier boundaries = Q1 − 1.5 × IQR and Q3 + 1.5 × IQR.

**Important examination tip:**

Independence is a condition determined mainly by the study design, whereas outliers are unusual observations identified during data analysis. Both should be considered before interpreting parametric test results.
```

markdown

```markdown
# 19. Central Limit Theorem (CLT)

## Meaning of the Central Limit Theorem

The Central Limit Theorem (CLT) is an important statistical principle stating that when sufficiently large random samples are taken from a population, the distribution of their sample means becomes approximately normal, regardless of the original population distribution, provided certain conditions are satisfied.

In simple terms, even if the original population data are not normally distributed, the averages calculated from many sufficiently large random samples will tend to follow a normal distribution.

The Central Limit Theorem is particularly important in biostatistics because it helps researchers perform statistical tests and make conclusions about populations using sample data.

## Purpose of the Central Limit Theorem

The main purposes are:

1. To explain why sample means tend to follow a normal distribution.
2. To help researchers make conclusions about population means.
3. To support the use of confidence intervals.
4. To provide the theoretical foundation for many hypothesis tests.
5. To explain why many parametric statistical methods can be used with sufficiently large samples, even when the original population is not normally distributed.

## Understanding the Central Limit Theorem

Imagine a researcher wants to study the average blood pressure of a large population.

Instead of measuring every individual, the researcher selects several random samples from the population.

For example:

- Sample 1: 30 patients.
- Sample 2: 30 patients.
- Sample 3: 30 patients.
- Sample 4: 30 patients.
- Sample 5: 30 patients.

The researcher calculates the mean blood pressure for each sample.

If this process is repeated many times, the distribution of these sample means will become approximately normal, even if the original blood pressure measurements are not normally distributed, provided the CLT conditions are met.

## Example in Biostatistics

A researcher wants to investigate the average blood glucose level of a population of diabetic patients.

The population blood glucose measurements are positively skewed rather than normally distributed.

The researcher repeatedly selects random samples of 50 patients and calculates the mean blood glucose level for each sample.

After collecting many sample means, the distribution of those means will tend to become approximately normal.

This demonstrates the Central Limit Theorem.

## Main Conditions of the Central Limit Theorem

The following conditions are important:

### 1. Random Sampling

Samples should be selected randomly from the population to reduce selection bias and support valid statistical inference.

### 2. Independent Observations

Observations should be independent, or the sampling design must account for any dependence.

### 3. Sufficiently Large Sample Size

The sample size should be sufficiently large for the sampling distribution of the mean to become approximately normal.

A commonly used general guideline is:

- n ≥ 30: Often considered sufficiently large.
- n < 30: Normality of the population may be more important.

**Important:** A sample size of 30 is only a general guideline, not a strict rule. Highly skewed distributions, extreme outliers, or heavy-tailed populations may require much larger samples.

## The Formula of the Central Limit Theorem

The standard error of the sample mean is calculated as:

\[
SE = \frac{\sigma}{\sqrt{n}}
\]

Where:

- SE = Standard error of the sample mean.
- σ = Population standard deviation.
- n = Sample size.

The sampling distribution of the sample mean has:

- Mean = μ (population mean).
- Standard deviation = σ/√n (standard error).

As the sample size increases, the standard error decreases.

This means that larger samples generally produce sample means that are more concentrated around the true population mean.

## Difference Between Population Distribution and Sampling Distribution

These two concepts are important for understanding the CLT.

| Population Distribution | Sampling Distribution |
|---|---|
| Describes the distribution of individual observations in a population. | Describes the distribution of a statistic, such as the sample mean, across repeated samples. |
| May be normal, skewed, or another shape. | Becomes approximately normal under the conditions of the CLT as sample size increases. |
| Example: Blood glucose levels of all diabetic patients. | Example: The distribution of average blood glucose levels from many random samples of 50 patients. |

## Relationship Between CLT and Parametric Tests

The Central Limit Theorem is important in parametric statistics because it helps explain why statistical tests based on sample means can often work well with sufficiently large samples.

For example:

1. One-Sample t-Test.
2. Independent Two-Sample t-Test.
3. Paired-Sample t-Test.
4. Analysis of Variance (ANOVA).

With sufficiently large samples, the sampling distributions of means and mean differences can be approximately normal, even when the original population measurements are not normally distributed.

However, the CLT does not automatically guarantee that every assumption of a parametric test is satisfied.

For example:
- Independence must still be considered.
- Outliers can still affect the results.
- Equal variances may still be required for standard independent-group tests.
- The study design must still be appropriate.

## Importance of the Central Limit Theorem in Biostatistics

The CLT is important because it allows researchers to:

1. Estimate population means using sample data.
2. Calculate confidence intervals.
3. Perform hypothesis testing.
4. Analyse medical and clinical research data.
5. Understand why larger sample sizes improve the precision of statistical estimates.

## Difference Between Normal Distribution and Central Limit Theorem

| Normal Distribution | Central Limit Theorem |
|---|---|
| A specific probability distribution. | A statistical theorem about sampling distributions. |
| Describes a symmetrical, bell-shaped distribution. | Explains why sample means become approximately normally distributed. |
| Applies to individual observations when their distribution is normal. | Applies to the distribution of sample means under suitable conditions. |
| Has a mean and standard deviation. | The sampling distribution has mean μ and standard error σ/√n. |

## Important Points to Remember

- The CLT applies to sample means and other suitable sample statistics.
- The original population does not have to be normally distributed.
- Larger sample sizes generally improve the normal approximation.
- The sample mean is centred around the population mean.
- The standard error decreases as sample size increases.
- Random sampling and independence are important conditions.

## Summary

The Central Limit Theorem (CLT) states that the distribution of sample means becomes approximately normal as the sample size increases, regardless of the original population distribution, under suitable conditions.

It is an important foundation of biostatistics because it supports hypothesis testing, confidence intervals, and many parametric statistical methods.

**Remember for examinations:**

1. CLT = Sampling distribution of means becomes approximately normal.
2. General sample-size guideline = 30 or more.
3. Mean of sampling distribution = Population mean (μ).
4. Standard error = σ/√n.
5. Larger sample size = Smaller standard error.

**Important examination tip:**

Do not confuse normality with the Central Limit Theorem.

- Normality concerns the distribution of the relevant data or model residuals.
- CLT concerns the distribution of sample means across repeated random samples.

The CLT does not mean that the original population data automatically become normally distributed when the sample size increases.
```

# 20. Non-Parametric Tests: Introduction and Overview

## Meaning of Non-Parametric Tests

Non-parametric tests are statistical methods that do not require the same strict distributional assumptions as parametric tests, particularly the assumption of normally distributed data.

They are commonly used when numerical data are not normally distributed, when sample sizes are small and distributional assumptions are not reasonable, or when data are measured using ordinal or categorical scales.

Unlike many parametric tests that compare means, non-parametric tests often use ranks, medians, or frequencies to analyse data.

In biostatistics, non-parametric tests are commonly used to analyse medical and clinical research data when parametric assumptions are not satisfied.

## Purpose of Non-Parametric Tests

The main purposes are:

1. To analyse data that do not satisfy the assumptions of certain parametric tests.
2. To analyse ordinal or ranked data.
3. To compare groups when distributional assumptions are not reasonable.
4. To analyse data from small samples when normality cannot reasonably be assumed.
5. To provide alternative statistical methods for medical and clinical research.

## Characteristics of Non-Parametric Tests

Non-parametric tests have the following characteristics:

1. They generally require fewer distributional assumptions than parametric tests.
2. Many non-parametric tests use ranks rather than raw numerical values.
3. They can be used with ordinal data.
4. They are useful for analysing skewed distributions.
5. They can be suitable for small samples, depending on the test and study design.
6. They do not always compare population means.

## Example in Biostatistics

A researcher wants to compare the pain levels of patients receiving two different treatments.

Pain is measured using a scale from:

0 = No pain.

10 = Severe pain.

The data are ordinal and may not follow a normal distribution.

Instead of using an independent t-test, the researcher may use the Mann-Whitney U test to compare the two independent groups.

## When Do We Use Non-Parametric Tests?

Non-parametric tests may be appropriate in the following situations:

- When numerical data are substantially skewed.
- When influential outliers make a parametric analysis unsuitable.
- When data are measured on an ordinal scale.
- When the assumptions of a particular parametric test are not satisfied.
- When the sample size is small and the normality assumption is not reasonable.

**Important:** Non-parametric tests are not automatically better than parametric tests. When parametric assumptions are reasonably satisfied, parametric tests can be more statistically powerful for detecting differences in means.

## Advantages of Non-Parametric Tests

1. Require fewer assumptions about the population distribution.
2. Can analyse ordinal and ranked data.
3. Can be useful for skewed numerical data.
4. Are less sensitive to some extreme observations because many use ranks.
5. Provide alternatives when certain parametric assumptions are violated.

## Limitations of Non-Parametric Tests

1. They may have lower statistical power than appropriate parametric tests.
2. They may provide less direct information about differences in means.
3. Some tests still have important assumptions, such as independence.
4. Interpretation may require additional care.
5. They do not eliminate the need to check the study design and data quality.

## Common Types of Non-Parametric Tests

The important non-parametric tests in biostatistics include:

1. Mann-Whitney U Test: Compares two independent groups.
2. Wilcoxon Signed-Rank Test: Compares two related measurements.
3. Kruskal-Wallis Test: Compares three or more independent groups.
4. Friedman Test: Compares three or more related measurements.
5. Spearman's Rank Correlation: Measures the strength and direction of a monotonic relationship between two variables.
6. Chi-Square Test: Examines associations between categorical variables.

## Summary

Non-parametric tests are statistical methods used when the assumptions required for certain parametric tests are not satisfied or when analysing ordinal data.

They are particularly useful in medical and clinical research involving skewed measurements, ranked data, and small samples.

**Remember for examinations:**

- Parametric tests commonly compare means.
- Non-parametric tests often use ranks or frequencies.
- Non-parametric tests require fewer distributional assumptions.
- Non-parametric tests can be used for ordinal data.
- The choice depends on the research question, study design, and data characteristics.

# 21. Non-Parametric Alternatives to Parametric Tests

## Meaning of Non-Parametric Alternatives

Non-parametric alternatives are statistical tests used instead of parametric tests when the assumptions of the parametric methods are not reasonably satisfied or when the data are ordinal.

They allow researchers to analyse data without relying on certain distributional assumptions, particularly normality.

In biostatistics, non-parametric alternatives are useful when analysing medical measurements, pain scores, patient satisfaction ratings, and other clinical data.

## Why Do We Need Non-Parametric Alternatives?

Parametric tests such as t-tests and ANOVA are commonly used to compare means.

However, some datasets may have:

- Highly skewed distributions.
- Influential outliers.
- Ordinal measurements.
- Small sample sizes with questionable normality assumptions.

In these situations, an appropriate non-parametric alternative may provide a more suitable analysis.

## Common Non-Parametric Alternatives to Parametric Tests

### 1. One-Sample t-Test → One-Sample Wilcoxon Signed-Rank Test

**Meaning:**

The one-sample Wilcoxon signed-rank test is used to compare a sample against a hypothesised population median or reference value under suitable assumptions.

It uses the ranks of the absolute differences between observations and the reference value.

**Example:**

A researcher wants to determine whether the median pain score of patients differs from a reference score of 5.

The pain scores are not normally distributed.

The researcher may use the one-sample Wilcoxon signed-rank test.

**When do we use it?**

- When comparing one sample with a hypothesised median.
- When the normality assumption for a one-sample t-test is not reasonable.
- When the differences from the reference value are appropriately distributed for the signed-rank method.

### 2. Independent Two-Sample t-Test → Mann-Whitney U Test

**Meaning:**

The Mann-Whitney U test is a non-parametric test used to compare two independent groups.

It compares the distributions of the two groups using ranked observations.

**Example:**

A researcher wants to compare pain scores between:

- Group A: Patients receiving medication A.
- Group B: Patients receiving medication B.

The pain scores are ordinal.

The researcher uses the Mann-Whitney U test to determine whether the distributions of pain scores differ between the groups.

**When do we use it?**

- When comparing two independent groups.
- When data are ordinal.
- When a rank-based comparison is more appropriate than an independent t-test.

**Important:** The Mann-Whitney U test does not automatically compare medians. It can be interpreted as a comparison of medians when the group distributions have similar shapes.

### 3. Paired-Sample t-Test → Wilcoxon Signed-Rank Test

**Meaning:**

The Wilcoxon signed-rank test is a non-parametric test used to compare two related measurements from the same participants or matched pairs.

It uses the ranks of the differences between paired observations.

**Example:**

A researcher measures the pain scores of the same patients:

- Before treatment.
- After treatment.

The pain scores are not normally distributed.

The researcher uses the Wilcoxon signed-rank test to determine whether there is a systematic change in pain scores.

**When do we use it?**

- Before-and-after studies.
- Two related measurements.
- Matched-pair studies.
- Ordinal or non-normally distributed paired data.

### 4. One-Way ANOVA → Kruskal-Wallis Test

**Meaning:**

The Kruskal-Wallis test is a non-parametric test used to compare three or more independent groups.

It compares the distributions of the groups using ranked observations.

**Example:**

A researcher wants to compare pain scores among patients receiving three different treatments:

- Group A: Medication A.
- Group B: Medication B.
- Group C: Medication C.

The researcher uses the Kruskal-Wallis test to determine whether there is evidence of a difference between the group distributions.

**When do we use it?**

- When comparing three or more independent groups.
- When data are ordinal.
- When the assumptions of standard one-way ANOVA are not reasonably satisfied.

**Important:** If the Kruskal-Wallis test is statistically significant, post-hoc comparisons, such as Dunn's test with an appropriate multiple-comparison correction, can identify which groups differ.

### 5. Repeated Measures ANOVA → Friedman Test

**Meaning:**

The Friedman test is a non-parametric test used to compare three or more related measurements.

It is suitable when the same participants are measured repeatedly under different conditions or at different times.

**Example:**

A researcher measures the pain scores of the same patients:

- Before treatment.
- After one month.
- After three months.

The researcher uses the Friedman test to determine whether pain scores differ across the three measurement periods.

**When do we use it?**

- When comparing three or more related measurements.
- In repeated-measures studies.
- When data are ordinal or the assumptions of repeated measures ANOVA are not reasonable.

### 6. Pearson Correlation → Spearman's Rank Correlation

**Meaning:**

Spearman's rank correlation is a non-parametric statistical method used to measure the strength and direction of a monotonic relationship between two variables.

It uses ranked values rather than relying on the original numerical measurements.

**Example:**

A researcher wants to investigate the relationship between:

- Physical activity level.
- Pain severity.

The measurements are ordinal or the relationship is monotonic but not necessarily linear.

The researcher uses Spearman's rank correlation.

**When do we use it?**

- When analysing ordinal data.
- When data are not suitable for Pearson correlation.
- When the relationship is monotonic but not necessarily linear.

## Comparison of Parametric Tests and Their Non-Parametric Alternatives

| Parametric test | Non-parametric alternative | Main purpose |
|---|---|---|
| One-Sample t-Test | One-Sample Wilcoxon Signed-Rank Test | Compare one sample with a reference value |
| Independent t-Test | Mann-Whitney U Test | Compare two independent groups |
| Paired-Sample t-Test | Wilcoxon Signed-Rank Test | Compare two related measurements |
| One-Way ANOVA | Kruskal-Wallis Test | Compare three or more independent groups |
| Repeated Measures ANOVA | Friedman Test | Compare three or more related measurements |
| Pearson Correlation | Spearman's Rank Correlation | Assess a relationship between two variables |

## Examples in Biostatistics

| Research question | Appropriate non-parametric test |
|---|---|
| Is the median pain score different from 5? | One-Sample Wilcoxon Signed-Rank Test |
| Do pain scores differ between two independent treatment groups? | Mann-Whitney U Test |
| Do pain scores change after treatment in the same patients? | Wilcoxon Signed-Rank Test |
| Do pain scores differ among three independent treatment groups? | Kruskal-Wallis Test |
| Do pain scores change across three time periods in the same patients? | Friedman Test |
| Is there a monotonic relationship between age and a ranked health score? | Spearman's Rank Correlation |

## Important Differences Between Parametric and Non-Parametric Tests

| Parametric Tests | Non-Parametric Tests |
|---|---|
| Often compare means. | Often compare ranks or distributions. |
| Require certain distributional assumptions. | Require fewer distributional assumptions. |
| Commonly used with continuous numerical data. | Can be used with ordinal and numerical data. |
| May be more powerful when their assumptions are satisfied. | Can be more appropriate when parametric assumptions are seriously violated. |
| Examples: t-tests and ANOVA. | Examples: Mann-Whitney and Kruskal-Wallis. |

## Advantages of Non-Parametric Alternatives

1. Useful when data are not normally distributed.
2. Suitable for ordinal measurements.
3. Can be less sensitive to extreme values when rank-based methods are used.
4. Provide alternatives when parametric assumptions are violated.
5. Useful in clinical research involving pain scores and patient satisfaction ratings.

## Limitations of Non-Parametric Alternatives

1. May have lower statistical power than suitable parametric tests.
2. Often do not directly test differences in means.
3. Some tests require additional assumptions, such as independence.
4. Interpretation can be more difficult when group distributions have different shapes.

## Summary

Non-parametric alternatives are used when parametric assumptions are not reasonably satisfied or when the data are ordinal.

The most important alternatives to remember are:

1. One-Sample t-Test → One-Sample Wilcoxon Signed-Rank Test.
2. Independent t-Test → Mann-Whitney U Test.
3. Paired-Sample t-Test → Wilcoxon Signed-Rank Test.
4. One-Way ANOVA → Kruskal-Wallis Test.
5. Repeated Measures ANOVA → Friedman Test.
6. Pearson Correlation → Spearman's Rank Correlation.

**Important examination tip:**

Remember the difference between independent and related groups:

- Two independent groups = Mann-Whitney U Test.
- Two related measurements = Wilcoxon Signed-Rank Test.
- Three or more independent groups = Kruskal-Wallis Test.
- Three or more related measurements = Friedman Test.

These distinctions are particularly important in biostatistics examinations.

markdown

```markdown
# 22. Correlation in Biostatistics (Pearson's Correlation)

## Meaning of Correlation

Correlation is a statistical method used to measure the strength and direction of the relationship between two variables.

In biostatistics, correlation helps researchers understand whether changes in one variable are associated with changes in another variable.

For example:
- Height and body weight.
- Age and blood pressure.
- Physical activity and body weight.
- Cholesterol levels and cardiovascular risk factors.

Correlation does not necessarily mean that one variable causes changes in another variable.

## Meaning of Pearson's Correlation

Pearson's correlation coefficient is a parametric statistical method used to measure the strength and direction of a linear relationship between two continuous numerical variables.

It is represented by the letter **r**.

The Pearson correlation coefficient ranges from:

\[
-1 \leq r \leq +1
\]

Where:
- r = +1: Perfect positive correlation.
- r = −1: Perfect negative correlation.
- r = 0: No linear correlation.

## Types of Correlation

There are three main types of correlation.

### 1. Positive Correlation

Positive correlation occurs when two variables move in the same direction.

This means that when one variable increases, the other variable also tends to increase.

**Example:**

A researcher investigates the relationship between height and body weight.

Generally, taller individuals may have higher body weights.

Therefore, height and body weight may show a positive correlation.

\[
r > 0
\]

<LearningViz type_id="CORRELATION" initial_values={{"pattern":"positive"}} locale_override="en-US"/>

### 2. Negative Correlation

Negative correlation occurs when two variables move in opposite directions.

This means that when one variable increases, the other variable tends to decrease.

**Example:**

A researcher investigates the relationship between physical activity and resting heart rate.

Higher levels of physical activity may be associated with lower resting heart rates.

This may demonstrate a negative correlation.

\[
r < 0
\]

<LearningViz type_id="CORRELATION" initial_values={{"pattern":"negative"}} locale_override="en-US"/>

### 3. No Correlation

No correlation means that there is no clear linear relationship between two variables.

Changes in one variable are not associated with a consistent linear change in the other variable.

**Example:**

A researcher investigates the relationship between shoe size and blood glucose level.

There may be no meaningful linear relationship between these variables.

\[
r \approx 0
\]

<LearningViz type_id="CORRELATION" initial_values={{"pattern":"none"}} locale_override="en-US"/>

## Pearson's Correlation Coefficient (r)

Pearson's correlation coefficient measures the strength and direction of a linear relationship between two continuous variables.

The interpretation depends on the value of r.

### Interpretation of Pearson's Correlation

| Correlation coefficient (r) | Interpretation |
|---|---|
| +1.00 | Perfect positive correlation |
| +0.70 to +0.99 | Strong positive correlation |
| +0.40 to +0.69 | Moderate positive correlation |
| +0.10 to +0.39 | Weak positive correlation |
| 0 | No linear correlation |
| −0.10 to −0.39 | Weak negative correlation |
| −0.40 to −0.69 | Moderate negative correlation |
| −0.70 to −0.99 | Strong negative correlation |
| −1.00 | Perfect negative correlation |

**Note:** These strength categories are general guidelines. Their interpretation depends on the research field and context.

## Formula of Pearson's Correlation

Pearson's correlation coefficient is calculated using the following formula:

\[
r = \frac{\sum (X-\bar X)(Y-\bar Y)}
{\sqrt{\sum(X-\bar X)^2\sum(Y-\bar Y)^2}}
\]

Where:

- r = Pearson's correlation coefficient.
- X = Values of the first variable.
- Y = Values of the second variable.
- X̄ = Mean of the first variable.
- Ȳ = Mean of the second variable.
- Σ = Sum of the values.

## Example in Biostatistics

A researcher wants to investigate the relationship between the number of hours spent exercising per week and body weight.

After collecting data from participants, the researcher calculates Pearson's correlation coefficient.

The result is:

\[
r = -0.75
\]

**Interpretation:**

- The correlation coefficient is negative.
- The relationship is strong.
- Higher exercise levels are associated with lower body weight in the sample.

This indicates a strong negative linear association.

However, it does not prove that exercise alone causes weight reduction.

## Hypothesis Testing in Pearson's Correlation

Pearson's correlation can also be used to determine whether the observed linear association is statistically significant.

There are two main hypotheses:

**1. Null Hypothesis (H₀):**

There is no linear correlation between the two population variables.

\[
H_0: \rho = 0
\]

**2. Alternative Hypothesis (H₁):**

There is a linear correlation between the two population variables.

\[
H_1: \rho \neq 0
\]

Where ρ (rho) represents the population correlation coefficient.

## Interpretation of p-Value in Pearson's Correlation

The p-value determines whether there is sufficient statistical evidence of a linear relationship.

- If p < 0.05: The correlation is statistically significant. Reject H₀.
- If p ≥ 0.05: The correlation is not statistically significant. Fail to reject H₀.

**Example:**

A researcher investigates the relationship between age and blood pressure.

Results:

- Pearson's r = 0.65.
- p = 0.01.

Interpretation:

1. The correlation is positive.
2. The strength of the correlation is moderate to strong.
3. The p-value is less than 0.05.
4. The correlation is statistically significant.

Therefore, there is sufficient evidence of a positive linear relationship between age and blood pressure.

## Assumptions of Pearson's Correlation

Before performing Pearson's correlation, researchers should consider the following assumptions:

### 1. Continuous Numerical Data

Both variables should generally be measured on a continuous numerical scale.

Examples:
- Age.
- Height.
- Weight.
- Blood pressure.
- Cholesterol levels.

### 2. Linear Relationship

The relationship between the two variables should be approximately linear.

This can be assessed using a scatter plot.

### 3. Normality

For conventional hypothesis testing and confidence intervals, the variables should be approximately jointly normally distributed (bivariate normality).

### 4. Independence of Observations

Each participant's pair of measurements should be independent of other participants' measurements.

### 5. Homoscedasticity

The variability of one variable should remain approximately constant across the values of the other variable.

### 6. No Influential Outliers

There should be no extreme observations that strongly influence the correlation coefficient.

## How to Interpret a Scatter Plot

A scatter plot is a graphical method used to examine the relationship between two numerical variables.

- Points moving upwards from left to right indicate positive correlation.
- Points moving downwards from left to right indicate negative correlation.
- Randomly scattered points suggest little or no linear correlation.

## Difference Between Pearson's and Spearman's Correlation

| Pearson's Correlation | Spearman's Rank Correlation |
|---|---|
| Parametric correlation method. | Non-parametric correlation method. |
| Measures linear relationships. | Measures monotonic relationships. |
| Uses original numerical values. | Uses ranked values. |
| Generally used with continuous numerical data. | Can be used with ordinal or numerical data. |
| Sensitive to influential outliers. | Often less sensitive to extreme values because it uses ranks. |
| Represented by r. | Represented by ρ or rₛ. |

## Difference Between Correlation and Causation

**Correlation:**

Means that two variables are associated with each other.

**Causation:**

Means that a change in one variable directly produces a change in another variable.

**Example:**

There may be a positive correlation between ice cream sales and the number of people swimming.

However, buying ice cream does not cause people to swim.

Both may increase because of warmer weather.

**Important:** Correlation does not prove causation.

## Applications of Pearson's Correlation in Biostatistics

Pearson's correlation is commonly used to investigate relationships between:

1. Height and body weight.
2. Age and blood pressure.
3. Cholesterol levels and other cardiovascular risk factors.
4. Exercise duration and resting heart rate.
5. Body mass index (BMI) and blood pressure.
6. Blood glucose levels and insulin levels.

## Summary

Pearson's correlation is a parametric statistical method used to measure the strength and direction of a linear relationship between two continuous numerical variables.

The correlation coefficient ranges from −1 to +1.

**Remember for examinations:**

- r = +1: Perfect positive correlation.
- r = −1: Perfect negative correlation.
- r = 0: No linear correlation.
- Positive correlation: Both variables move in the same direction.
- Negative correlation: Variables move in opposite directions.
- Pearson's correlation: Measures linear relationships.
- Spearman's correlation: Measures monotonic relationships.

**Important examination tip:**

Always remember that correlation does not mean causation. A statistically significant correlation indicates evidence of an association, not proof that one variable causes the other.
```

markdown

```markdown
# 23. Regression Analysis (Linear Regression)

## Meaning of Regression Analysis

Regression analysis is a statistical method used to examine the relationship between a dependent variable (outcome variable) and one or more independent variables (predictor variables).

It helps researchers understand how changes in one or more predictor variables are associated with changes in an outcome variable.

In biostatistics, regression analysis is commonly used to predict medical outcomes and investigate relationships between health-related variables.

Examples:
- Predicting blood pressure based on age.
- Predicting body weight based on height.
- Predicting blood glucose levels based on BMI.
- Investigating the relationship between cholesterol levels and cardiovascular risk factors.

## Meaning of Linear Regression

Linear regression is a statistical method used to model the linear relationship between a dependent variable and one or more independent variables.

It produces a straight-line equation that describes the relationship between the variables.

There are two main types:

1. Simple Linear Regression.
2. Multiple Linear Regression.

## 1. Simple Linear Regression

### Meaning

Simple linear regression examines the relationship between one independent variable (predictor) and one dependent variable (outcome).

**Example in Biostatistics:**

A researcher wants to investigate whether age predicts systolic blood pressure.

- Independent variable (X): Age.
- Dependent variable (Y): Systolic blood pressure.

The researcher collects data from patients and uses simple linear regression to estimate how blood pressure changes with age.

### Linear Regression Equation

The general equation of simple linear regression is:

\[
Y = a + bX
\]

Where:

- Y = Predicted dependent variable.
- a = Intercept.
- b = Regression coefficient (slope).
- X = Independent variable.

**Explanation of the terms:**

- Intercept (a): The predicted value of Y when X equals zero.
- Slope (b): The expected change in Y for every one-unit increase in X.

### Example

Suppose a researcher develops the following regression equation:

\[
Y = 80 + 0.5X
\]

Where:

- Y = Predicted systolic blood pressure (mmHg).
- X = Age (years).
- 80 = Intercept.
- 0.5 = Slope.

If a patient is 40 years old:

\[
Y = 80 + (0.5 \times 40)
\]

\[
Y = 100 \text{ mmHg}
\]

**Interpretation:**

The predicted systolic blood pressure for a 40-year-old patient is 100 mmHg.

The slope of 0.5 means that each additional year of age is associated with an estimated increase of 0.5 mmHg in systolic blood pressure.

This is an illustrative model, not a clinical prediction rule.

## 2. Multiple Linear Regression

### Meaning

Multiple linear regression examines the relationship between one dependent variable and two or more independent variables.

It allows researchers to investigate several predictors simultaneously.

**Example in Biostatistics:**

A researcher wants to predict blood pressure using:

- Age.
- Body mass index (BMI).
- Physical activity level.
- Cholesterol level.

The dependent variable is blood pressure.

The independent variables are age, BMI, physical activity, and cholesterol level.

### Multiple Linear Regression Equation

The general equation is:

\[
Y = a + b_1X_1 + b_2X_2 + b_3X_3 + \cdots + b_nX_n
\]

Where:

- Y = Dependent variable.
- a = Intercept.
- b₁, b₂, b₃ = Regression coefficients.
- X₁, X₂, X₃ = Independent variables.
- n = Number of independent variables.

## Difference Between Simple and Multiple Linear Regression

| Simple Linear Regression | Multiple Linear Regression |
|---|---|
| Uses one independent variable. | Uses two or more independent variables. |
| Predicts one dependent variable. | Predicts one dependent variable. |
| Examines one predictor's relationship with the outcome. | Examines several predictors simultaneously. |
| Example: Age and blood pressure. | Example: Age, BMI and blood pressure. |

## Purpose of Regression Analysis

Regression analysis is used to:

1. Predict outcomes using independent variables.
2. Examine relationships between health-related variables.
3. Identify factors associated with medical conditions.
4. Estimate how much an outcome changes when a predictor changes.
5. Adjust for other variables when investigating associations.

## Important Components of Linear Regression

### 1. Dependent Variable

The dependent variable is the outcome that the researcher wants to explain or predict.

Examples:
- Blood pressure.
- Blood glucose level.
- Body weight.
- Cholesterol level.

### 2. Independent Variable

The independent variable is the predictor used to explain or predict changes in the dependent variable.

Examples:
- Age.
- Height.
- BMI.
- Exercise duration.

### 3. Intercept

The intercept is the predicted value of the dependent variable when all independent variables equal zero.

### 4. Regression Coefficient (Slope)

The regression coefficient represents the expected change in the dependent variable for a one-unit increase in the independent variable, holding other predictors constant in multiple regression.

### 5. Residuals

Residuals are the differences between the actual observed values and the values predicted by the regression model.

\[
Residual = Observed\ Value - Predicted\ Value
\]

Small residuals generally indicate that the model's predictions are close to the observed values.

## Assumptions of Linear Regression

Before performing linear regression, researchers should consider the following assumptions:

### 1. Linearity

There should be an approximately linear relationship between the predictors and the outcome.

### 2. Independence of Observations and Errors

Observations and model errors should be independent, according to the study design.

### 3. Homoscedasticity

The variance of the residuals should remain approximately constant across the range of predicted values.

### 4. Normality of Residuals

For conventional hypothesis tests and confidence intervals, regression residuals should be approximately normally distributed.

### 5. No Serious Multicollinearity

In multiple linear regression, independent variables should not be excessively correlated with one another.

### 6. No Highly Influential Outliers

Extreme observations should not have an undue influence on the regression model.

## Interpretation of Regression Results

Researchers commonly examine several statistical results.

### 1. Regression Coefficient (β)

The regression coefficient indicates the direction and size of the association between a predictor and the outcome.

- Positive coefficient: As X increases, Y tends to increase.
- Negative coefficient: As X increases, Y tends to decrease.
- Zero coefficient: No linear association is indicated by that coefficient.

### 2. P-Value

The p-value helps determine whether there is statistical evidence of an association between a predictor and the outcome.

- p < 0.05: Statistically significant evidence of an association.
- p ≥ 0.05: Insufficient evidence of an association at the 5% significance level.

### 3. R-Squared (R²)

R-squared measures the proportion of variation in the dependent variable explained by the regression model.

It ranges from 0 to 1 in ordinary least-squares regression with an intercept.

**Example:**

If:

\[
R^2 = 0.75
\]

This means that 75% of the observed variation in the outcome is explained by the model.

The remaining 25% is not explained by the model.

### 4. Confidence Interval

A confidence interval provides a range of plausible values for a population regression coefficient.

For example, a 95% confidence interval for a regression coefficient may be:

\[
95\% \ CI = 0.2 \text{ to } 0.8
\]

This indicates that the estimated coefficient is positive, with the interval excluding zero.

## Example in Biostatistics

A researcher investigates whether BMI is associated with systolic blood pressure in 100 adults.

The regression analysis produces:

\[
Y = 90 + 1.2X
\]

Where:

- Y = Predicted systolic blood pressure (mmHg).
- X = BMI.
- 90 = Intercept.
- 1.2 = Regression coefficient.

**Interpretation:**

For every one-unit increase in BMI, systolic blood pressure is estimated to increase by 1.2 mmHg on average.

This describes an association, not necessarily a causal relationship.

## Difference Between Correlation and Regression

| Correlation | Regression |
|---|---|
| Measures the strength and direction of an association. | Models the relationship between predictors and an outcome. |
| Does not distinguish between dependent and independent variables. | Distinguishes between outcome and predictor variables. |
| Uses a correlation coefficient (r). | Uses regression coefficients (β). |
| Does not directly predict an outcome. | Can be used to predict an outcome. |
| Pearson's correlation measures linear association. | Linear regression estimates a linear relationship. |

## Applications of Linear Regression in Biostatistics

Linear regression is commonly used in:

1. Predicting blood pressure based on age.
2. Estimating body weight based on height.
3. Investigating the relationship between BMI and cholesterol levels.
4. Predicting blood glucose levels using clinical measurements.
5. Examining factors associated with lung function.
6. Studying the relationship between exercise duration and resting heart rate.

## Advantages of Linear Regression

1. Helps predict numerical outcomes.
2. Examines relationships between variables.
3. Allows researchers to study multiple predictors.
4. Helps adjust for potential confounding variables.
5. Provides interpretable regression coefficients.

## Limitations of Linear Regression

1. Assumes a linear relationship between predictors and the outcome.
2. Can be influenced by extreme observations.
3. Requires appropriate model assumptions for reliable statistical inference.
4. Does not automatically establish causation.
5. Predictions may be unreliable when used outside the range of the observed data.

## Summary

Regression analysis is a statistical method used to examine relationships between dependent and independent variables.

Linear regression is particularly useful when the outcome variable is continuous and the relationship can reasonably be modelled as linear.

The two main types are:

1. Simple Linear Regression: One independent variable and one dependent variable.
2. Multiple Linear Regression: Two or more independent variables and one dependent variable.

**Remember for examinations:**

- Regression = Examines relationships and predicts outcomes.
- Simple linear regression = One predictor.
- Multiple linear regression = Two or more predictors.
- Dependent variable = Outcome.
- Independent variable = Predictor.
- Slope = Expected change in the outcome for a one-unit increase in the predictor.
- R² = Proportion of outcome variation explained by the model.
- Residual = Observed value − Predicted value.

**Important examination tip:**

Do not confuse correlation with regression.

Correlation measures the strength and direction of a relationship, whereas regression models the relationship and can be used to predict an outcome.

Also remember that regression identifies statistical associations; it does not automatically prove that one variable causes another.
```


**
