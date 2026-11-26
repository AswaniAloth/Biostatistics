# 1. Introduction to Parametric Testing in Biostatistics

## Meaning of Parametric Testing

Parametric tests are statistical methods used to analyse numerical data and make conclusions about a population based on sample data.

These tests are commonly used to compare means (averages), examine differences between groups, and investigate relationships between numerical variables.

Parametric tests are based on certain assumptions about the population distribution, particularly normality.

In biostatistics, parametric tests are widely used in medical and health research to compare treatment outcomes, blood pressure, blood glucose, haemoglobin levels, body weight, and other numerical measurements.

## Main Purpose of Parametric Tests

The main purposes are:

1. To compare the mean of a sample with a known or hypothesised population value.
2. To compare the means of two independent groups.
3. To compare measurements taken from the same individuals before and after an intervention.
4. To compare the means of three or more groups.
5. To determine whether observed differences are statistically significant.

## Characteristics of Parametric Tests

1. They are generally used with numerical data, especially continuous data.
2. They usually assume that the data or model residuals follow an approximately normal distribution.
3. They may require equal variances between groups.
4. They require an appropriate study design, including independence of observations where applicable.
5. They commonly use means and standard deviations to describe data.
6. They often have greater statistical power than non-parametric alternatives when their assumptions are satisfied.

## Four Main Parametric Tests

There are four important parametric tests commonly studied in biostatistics:

1. **One-Sample t-Test:** Compares the mean of one sample with a known or hypothesised population mean.

2. **Independent Two-Sample t-Test:** Compares the means of two separate and unrelated groups.

3. **Paired-Sample t-Test:** Compares two related measurements from the same participants or matched individuals.

4. **Analysis of Variance (ANOVA):** Compares the means of three or more groups.

## Examples in Biostatistics

Parametric tests can be used in medical research to investigate questions such as:

- Does the average haemoglobin level of pregnant women differ from the standard reference value?
- Does a new medication reduce patients' blood pressure?
- Is there a difference in average blood glucose levels between two treatment groups?
- Do three different dietary programmes produce different average weight-loss results?

## Importance of Parametric Tests in Biostatistics

Parametric tests are important because they help researchers:

1. Evaluate the effectiveness of medical treatments.
2. Compare health outcomes between different populations.
3. Analyse clinical trial results.
4. Identify statistically significant differences.
5. Make evidence-based decisions in healthcare and medical research.

**Important:** A statistically significant result does not automatically mean that a treatment is clinically important. Researchers should also consider the size and practical importance of the observed difference.

## Summary

Parametric testing is an important part of biostatistics. It allows researchers to analyse numerical data, compare group means, and determine whether observed differences are statistically significant.

The most commonly studied parametric tests are the one-sample t-test, independent t-test, paired-sample t-test, and ANOVA.

# 2. Overview of Parametric Tests

## Meaning of Parametric Tests

Parametric tests are statistical methods used to analyse numerical data and compare population parameters, particularly means (averages).

They are based on assumptions about the population distribution, especially that the data or relevant model residuals are approximately normally distributed.

In biostatistics, these tests are commonly used to compare the average blood pressure, blood glucose, haemoglobin levels, body weight, and other medical measurements.

## Main Types of Parametric Tests

There are four main parametric tests commonly used in biostatistics:

### 1. One-Sample t-Test

**Meaning:** A one-sample t-test compares the mean of one sample with a known or hypothesised population mean.

**Example:** A researcher wants to determine whether the average haemoglobin level of 30 pregnant women differs from the standard reference value of 12 g/dL.

**When do we use it?**
- When comparing one sample mean with a known or hypothesised value.

### 2. Independent Two-Sample t-Test

**Meaning:** An independent two-sample t-test compares the means of two separate and unrelated groups.

**Example:** A researcher wants to compare the average blood pressure of:
- Group A: 30 patients receiving medication A.
- Group B: 30 patients receiving medication B.

**When do we use it?**
- When comparing the means of two independent groups.

### 3. Paired-Sample t-Test

**Meaning:** A paired-sample t-test compares two related measurements from the same participants or matched individuals.

**Example:** A researcher measures the blood glucose levels of 20 patients before and after receiving treatment.

**When do we use it?**
- Before and after treatment.
- Before and after exercise.
- Before and after medication.
- When comparing two measurements from the same individuals.

**Important:** Normality is assessed using the differences between the paired measurements.

### 4. Analysis of Variance (ANOVA)

**Meaning:** ANOVA is a parametric statistical test used to compare the means of three or more groups.

**Example:** A researcher wants to compare the average blood glucose levels of patients receiving three different treatments:
- Group A: Diet programme.
- Group B: Exercise programme.
- Group C: Medication programme.

**When do we use it?**
- When comparing the means of three or more independent groups using one-way ANOVA.

**Important:** If ANOVA produces a p-value below 0.05, it indicates that at least one group mean differs significantly. Post-hoc tests, such as Tukey's test, can identify which groups differ.

## Comparison of the Four Main Parametric Tests

| Test | Number of groups or measurements | Main purpose |
|---|---|---|
| One-sample t-test | One sample | Compare a sample mean with a known value |
| Independent t-test | Two independent groups | Compare two unrelated means |
| Paired-sample t-test | Two related measurements | Compare two related means |
| ANOVA | Three or more independent groups | Compare three or more means |

## General Assumptions of Parametric Tests

Before using parametric tests, researchers should consider the following assumptions:

1. **Numerical data:** Data should generally be continuous or measured on an interval or ratio scale.
2. **Normality:** Data or relevant model residuals should be approximately normally distributed.
3. **Independence:** Observations should be independent where required by the study design.
4. **Homogeneity of variance:** Groups should generally have equal variances when using standard independent t-tests and one-way ANOVA.
5. **No influential outliers:** Extreme values should not unduly influence the results.

**Note:** Not every parametric test has exactly the same assumptions. For example, a paired t-test assesses normality of the differences rather than the individual measurements.

## Importance of Parametric Tests in Biostatistics

Parametric tests are important because they help researchers:

- Compare the effectiveness of different medical treatments.
- Analyse clinical trial results.
- Compare health measurements between populations.
- Identify statistically significant differences.
- Support evidence-based medical decisions.

## Summary

The four main parametric tests are:

1. One-sample t-test.
2. Independent two-sample t-test.
3. Paired-sample t-test.
4. Analysis of Variance (ANOVA).

The correct test depends on the research question, the number of groups, whether observations are independent or related, and whether the relevant statistical assumptions are satisfied.

# 3. One-Sample t-Test

## Meaning of One-Sample t-Test

A one-sample t-test is a parametric statistical test used to compare the mean (average) of one sample with a known or hypothesised population mean.

It helps researchers determine whether the difference between the sample mean and the expected population mean is statistically significant.

In biostatistics, it is commonly used to compare medical measurements, such as haemoglobin levels, blood pressure, body weight, and blood glucose levels, with established reference values.

## Purpose of One-Sample t-Test

The main purposes are:

1. To compare a sample mean with a known or hypothesised population mean.
2. To determine whether the observed difference is statistically significant.
3. To test whether a sample comes from a population with a particular mean.

## Example in Biostatistics

A researcher wants to determine whether the average haemoglobin level of 30 pregnant women differs from the standard reference value of 12 g/dL.

The following information is available:

- Sample size: 30 pregnant women.
- Sample mean: 11 g/dL.
- Hypothesised population mean: 12 g/dL.
- Significance level: 0.05.

The researcher uses a one-sample t-test to determine whether the average haemoglobin level is significantly different from 12 g/dL.

## Hypotheses of One-Sample t-Test

A statistical test involves two hypotheses:

**1. Null Hypothesis (H₀):**

There is no significant difference between the sample population mean and the hypothesised population mean.

H₀: μ = 12 g/dL

**2. Alternative Hypothesis (H₁):**

There is a significant difference between the sample population mean and the hypothesised population mean.

H₁: μ ≠ 12 g/dL

This is a two-tailed test because the researcher wants to know whether the mean is either higher or lower than 12 g/dL.

## Formula of One-Sample t-Test

The formula is:

t = (x̄ − μ) / (s / √n)

Where:

- t = Calculated t-value.
- x̄ = Sample mean.
- μ = Hypothesised population mean.
- s = Sample standard deviation.
- n = Sample size.

## Interpretation of p-Value

The p-value helps determine whether the result is statistically significant.

- If p < 0.05: The result is statistically significant. Reject the null hypothesis.
- If p ≥ 0.05: The result is not statistically significant. Fail to reject the null hypothesis.

**Example:**

If the calculated p-value is 0.02:

- 0.02 is less than 0.05.
- The result is statistically significant.
- Reject the null hypothesis.
- There is sufficient evidence that the population mean differs from 12 g/dL.

Important: A p-value does not measure the size or clinical importance of the difference.

## Assumptions of One-Sample t-Test

Before performing a one-sample t-test, the following assumptions should be considered:

1. **Numerical data:** The variable should be continuous and measured on an interval or ratio scale.
2. **Random sampling:** The sample should ideally be randomly selected from the target population.
3. **Independence:** Observations should be independent of one another.
4. **Normality:** The sample data should be approximately normally distributed, particularly when the sample size is small.
5. **No influential outliers:** Extreme values should not strongly influence the sample mean.

**Note:** With sufficiently large samples, the Central Limit Theorem often allows the sampling distribution of the mean to be approximately normal, provided the observations are independent and the population has a finite variance. However, severe outliers can still cause problems.

## When Do We Use a One-Sample t-Test?

A one-sample t-test is used when:

- Comparing the average haemoglobin level with a standard reference value.
- Comparing average blood pressure with an established population value.
- Comparing average body weight with a known standard.
- Comparing average blood glucose levels with a hypothesised value.

## Advantages of One-Sample t-Test

1. Simple and easy to perform.
2. Useful for comparing sample means with established reference values.
3. Requires only one sample.
4. Helps determine whether an observed difference is statistically significant.

## Summary

A one-sample t-test is a parametric test used to compare the mean of one sample with a known or hypothesised population mean.

**Remember for examinations:**

One sample + one known or hypothesised mean = One-Sample t-Test.

# 4. Two-Sample (Independent) t-Test

## Meaning of Independent Two-Sample t-Test

An independent two-sample t-test is a parametric statistical test used to compare the means (averages) of two separate and unrelated groups.

It helps researchers determine whether there is a statistically significant difference between the average values of two independent populations.

In biostatistics, it is commonly used to compare medical measurements such as blood pressure, blood glucose levels, haemoglobin levels, body weight, and cholesterol levels between two different groups.

## Purpose of Independent Two-Sample t-Test

The main purposes are:

1. To compare the means of two independent groups.
2. To determine whether the difference between two group means is statistically significant.
3. To investigate the effectiveness of different medical treatments.
4. To compare health outcomes between two different populations.

## Example in Biostatistics

A researcher wants to compare the average blood pressure of patients receiving two different medications.

The participants are divided into two independent groups:

- Group A: 30 patients receiving medication A.
- Group B: 30 patients receiving medication B.

The researcher measures the blood pressure of both groups and uses an independent two-sample t-test to determine whether there is a statistically significant difference between their average blood pressure levels.

**Important:** The participants in Group A must be different from those in Group B. The same individuals should not be included in both groups as independent observations.

## Hypotheses of Independent Two-Sample t-Test

A statistical test involves two hypotheses:

**1. Null Hypothesis (H₀):**

There is no significant difference between the mean values of the two independent groups.

H₀: μ₁ = μ₂

**2. Alternative Hypothesis (H₁):**

There is a significant difference between the mean values of the two independent groups.

H₁: μ₁ ≠ μ₂

This is a two-tailed test because the researcher wants to determine whether the mean of one group is either higher or lower than the other.

## Formula of Independent Two-Sample t-Test

For the standard independent t-test assuming equal population variances, the formula is:

t = (x̄₁ − x̄₂) / [sₚ √(1/n₁ + 1/n₂)]

Where:

- t = Calculated t-value.
- x̄₁ = Mean of Group 1.
- x̄₂ = Mean of Group 2.
- sₚ = Pooled standard deviation.
- n₁ = Sample size of Group 1.
- n₂ = Sample size of Group 2.

**Note:** When the two groups have unequal variances, Welch's t-test is generally more appropriate.

## Interpretation of p-Value

The p-value helps determine whether the difference between the two group means is statistically significant.

- If p < 0.05: The result is statistically significant. Reject the null hypothesis.
- If p ≥ 0.05: The result is not statistically significant. Fail to reject the null hypothesis.

**Example:**

A researcher compares the average blood pressure of patients receiving medication A and medication B.

If the calculated p-value is 0.03:

- 0.03 is less than 0.05.
- The result is statistically significant.
- Reject the null hypothesis.
- There is sufficient evidence that the average blood pressure differs between the two treatment groups.

Important: Statistical significance does not automatically mean that the difference is clinically important.

## Assumptions of Independent Two-Sample t-Test

Before performing an independent t-test, the following assumptions should be considered:

1. **Numerical data:** The dependent variable should be continuous and measured on an interval or ratio scale.
2. **Independent observations:** The two groups must be separate and unrelated.
3. **Normality:** The outcome should be approximately normally distributed within each group, particularly when sample sizes are small.
4. **Homogeneity of variance:** For the standard independent t-test, the two groups should have approximately equal population variances.
5. **No influential outliers:** Extreme values should not strongly influence the group means.

**Note:** If the equal-variance assumption is not satisfied, Welch's t-test can be used. It does not require equal population variances.

## When Do We Use an Independent Two-Sample t-Test?

It is used when comparing the means of two unrelated groups, such as:

- Blood pressure in men versus women.
- Blood glucose levels in smokers versus non-smokers.
- Haemoglobin levels in treatment A versus treatment B.
- Body weight in two different dietary groups.
- Cholesterol levels in two independent patient groups.

## Advantages of Independent Two-Sample t-Test

1. Simple and widely used in medical research.
2. Helps compare two independent groups.
3. Determines whether the difference between two means is statistically significant.
4. Useful for evaluating the effectiveness of different treatments.
5. Provides information about the difference between group averages.

## Difference Between One-Sample and Independent Two-Sample t-Tests

| One-Sample t-Test | Independent Two-Sample t-Test |
|---|---|
| Uses one sample. | Uses two independent groups. |
| Compares a sample mean with a known or hypothesised value. | Compares the means of two unrelated groups. |
| Example: Haemoglobin level compared with 12 g/dL. | Example: Blood pressure in medication A versus medication B. |

## Summary

An independent two-sample t-test is a parametric test used to compare the means of two separate and unrelated groups.

**Remember for examinations:**

Two independent groups + comparison of two means = Independent Two-Sample t-Test.

# 5. Paired-Sample t-Test

## Meaning of Paired-Sample t-Test

A paired-sample t-test (also called a dependent t-test) is a parametric statistical test used to compare two related measurements from the same participants or matched individuals.

It helps researchers determine whether there is a statistically significant difference between two measurements taken under different conditions or at different times.

In biostatistics, it is commonly used to compare medical measurements before and after treatment, exercise, medication, or a health intervention.

## Purpose of Paired-Sample t-Test

The main purposes are:

1. To compare two related measurements from the same participants.
2. To determine whether a treatment or intervention produces a significant change.
3. To examine differences between measurements taken at two different times.
4. To reduce the influence of individual differences because the same participants are measured twice.

## Example in Biostatistics

A researcher wants to determine whether a new medication reduces the blood pressure of patients.

The researcher measures the blood pressure of 20 patients at two different times:

- Before treatment: Blood pressure is measured before taking the medication.
- After treatment: Blood pressure is measured after taking the medication.

The same 20 patients are measured twice.

The researcher uses a paired-sample t-test to determine whether the average blood pressure has changed significantly after treatment.

**Important:** The two measurements must be related. In this example, both measurements come from the same patients.

## Hypotheses of Paired-Sample t-Test

A statistical test involves two hypotheses:

**1. Null Hypothesis (H₀):**

There is no significant difference between the mean of the two related measurements.

H₀: μd = 0

**2. Alternative Hypothesis (H₁):**

There is a significant difference between the mean of the two related measurements.

H₁: μd ≠ 0

Where:

- μd = Population mean of the differences between paired measurements.
- 0 = No average difference between the two measurements.

This is a two-tailed test because the researcher wants to determine whether the measurements have either increased or decreased.

## Formula of Paired-Sample t-Test

The formula is:

t = d̄ / (sd / √n)

Where:

- t = Calculated t-value.
- d̄ = Mean of the differences between paired measurements.
- sd = Standard deviation of the differences.
- n = Number of pairs or participants.

**Note:** The differences are calculated for each participant by subtracting one measurement from the other.

For example:

Difference = After-treatment measurement − Before-treatment measurement.

## Interpretation of p-Value

The p-value helps determine whether the average difference between the paired measurements is statistically significant.

- If p < 0.05: The result is statistically significant. Reject the null hypothesis.
- If p ≥ 0.05: The result is not statistically significant. Fail to reject the null hypothesis.

**Example:**

A researcher measures the blood pressure of 20 patients before and after medication.

If the calculated p-value is 0.01:

- 0.01 is less than 0.05.
- The result is statistically significant.
- Reject the null hypothesis.
- There is sufficient evidence that the average blood pressure changed after treatment.

Important: A statistically significant change does not automatically prove that the medication caused the change. Other factors may also influence the results.

## Assumptions of Paired-Sample t-Test

Before performing a paired-sample t-test, the following assumptions should be considered:

1. **Numerical data:** The measurements should be continuous and measured on an interval or ratio scale.
2. **Related observations:** The two measurements must come from the same participants or appropriately matched individuals.
3. **Independence between pairs:** Each participant's pair of measurements should be independent of the other participants' pairs.
4. **Normality of differences:** The differences between the paired measurements should be approximately normally distributed, particularly when the sample size is small.
5. **No influential outliers:** There should be no extreme outliers in the differences between paired measurements.

**Very Important for Examinations:**

For a paired-sample t-test, normality is assessed on the differences between the two measurements, NOT on each measurement separately.

## When Do We Use a Paired-Sample t-Test?

It is used when comparing two related measurements, such as:

- Blood pressure before and after treatment.
- Blood glucose levels before and after medication.
- Body weight before and after a dietary programme.
- Heart rate before and after exercise.
- Cholesterol levels before and after a lifestyle intervention.

## Advantages of Paired-Sample t-Test

1. Useful for analysing before-and-after studies.
2. Controls for individual differences because the same participants are measured twice.
3. Can provide greater statistical power than an independent t-test when measurements are strongly correlated.
4. Helps evaluate changes following medical treatments or interventions.
5. Simple to perform and interpret.

## Difference Between Independent and Paired-Sample t-Tests

| Independent t-Test | Paired-Sample t-Test |
|---|---|
| Compares two unrelated groups. | Compares two related measurements. |
| Uses different participants in each group. | Uses the same participants twice or matched individuals. |
| Example: Medication A versus medication B. | Example: Before and after medication. |
| Normality is assessed within each group. | Normality is assessed on the differences. |

## Summary

A paired-sample t-test is a parametric statistical test used to compare two related measurements from the same participants or matched individuals.

It is commonly used in medical research to determine whether a treatment or intervention produces a significant change.

**Remember for examinations:**

Same people + two measurements + before and after = Paired-Sample t-Test.


# 6. Comparison of the Three Types of t-Tests

## Introduction

There are three main types of t-tests commonly used in biostatistics:

1. One-Sample t-Test.
2. Independent Two-Sample t-Test.
3. Paired-Sample t-Test.

All three are parametric statistical tests used to compare means (averages). However, they differ in the number of groups, the relationship between observations, and the research questions they answer.

Choosing the correct t-test depends on the study design and the type of comparison being made.

## 1. One-Sample t-Test

**Meaning:** Compares the mean of one sample with a known or hypothesised population mean.

**Example:** A researcher wants to determine whether the average haemoglobin level of 30 pregnant women differs from the standard reference value of 12 g/dL.

**When do we use it?**
- When comparing one sample mean with a known or hypothesised value.

## 2. Independent Two-Sample t-Test

**Meaning:** Compares the means of two separate and unrelated groups.

**Example:** A researcher wants to compare the average blood pressure of:
- Group A: Patients receiving medication A.
- Group B: Patients receiving medication B.

**When do we use it?**
- When comparing the means of two independent groups.

## 3. Paired-Sample t-Test

**Meaning:** Compares two related measurements from the same participants or matched individuals.

**Example:** A researcher measures the blood pressure of the same patients:
- Before treatment.
- After treatment.

**When do we use it?**
- When comparing two related measurements.
- Before-and-after studies.
- When the same participants are measured twice.

## Comparison of the Three Types of t-Tests

| Feature | One-Sample t-Test | Independent t-Test | Paired-Sample t-Test |
|---|---|---|---|
| Number of samples | One sample | Two groups | Two related measurements |
| Participants | One group | Different participants | Same participants or matched pairs |
| Main purpose | Compare a sample mean with a known value | Compare two unrelated means | Compare two related means |
| Relationship | One sample and a reference value | Independent groups | Related observations |
| Example | Haemoglobin vs. 12 g/dL | Medication A vs. B | Blood pressure before and after treatment |
| Normality assumption | Sample values | Values within each group or model residuals | Differences between paired measurements |

## How to Choose the Correct t-Test

Ask yourself the following questions:

**Question 1: Are you comparing one sample with a known or hypothesised value?**

- Yes → One-Sample t-Test.

**Question 2: Are you comparing two different and unrelated groups?**

- Yes → Independent Two-Sample t-Test.

**Question 3: Are you comparing the same participants at two different times or under two different conditions?**

- Yes → Paired-Sample t-Test.

## Examples in Biostatistics

| Research question | Correct statistical test |
|---|---|
| Is the average haemoglobin level different from 12 g/dL? | One-Sample t-Test |
| Is blood pressure different between men and women? | Independent t-Test |
| Does medication reduce blood glucose levels? (Before and after measurements in the same patients) | Paired-Sample t-Test |
| Is average body weight different between smokers and non-smokers? | Independent t-Test |
| Does exercise change the heart rate of the same participants? | Paired-Sample t-Test |

## Important Differences in Assumptions

**One-Sample t-Test:**
- Numerical data.
- Independent observations.
- Approximately normal sample values, particularly for small samples.
- No influential outliers.

**Independent Two-Sample t-Test:**
- Numerical data.
- Two independent groups.
- Approximate normality within each group, particularly for small samples.
- Equal variances for the standard Student's t-test.
- No influential outliers.

**Paired-Sample t-Test:**
- Numerical data.
- Two related measurements.
- Independent pairs.
- Approximately normally distributed differences.
- No influential outliers in the differences.

## Summary

The three types of t-tests are used for different research situations:

1. **One-Sample t-Test:** One sample compared with a known or hypothesised value.
2. **Independent t-Test:** Two separate and unrelated groups compared.
3. **Paired-Sample t-Test:** Two related measurements compared.

**Important examination tip:**

- One sample + one reference value = One-Sample t-Test.
- Two different groups = Independent t-Test.
- Same people measured twice = Paired-Sample t-Test.

Remember: The most important factor in selecting the correct t-test is the relationship between the samples or measurements.

This chapter continue with Analysis of Variance - Anova 



