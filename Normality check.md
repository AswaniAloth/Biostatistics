# Biostatistics Study Notes
## Statistical Analysis for Biostatisticians – With Medical Examples

These notes explain how a biostatistician chooses the correct statistical analysis in medical research, including normality testing, parametric tests, non-parametric tests, regression, and survival analysis.

The most important principle is:

> First understand the research question, then identify the type of data, check the assumptions, and finally select the appropriate statistical test.

---

# 1. Understanding the Types of Data

Before performing any statistical analysis, a biostatistician must understand the data.

There are four important types of data:

## A. Nominal Data (Categorical Data)

Data that can be divided into categories without a specific order.

**Medical examples:**
- Gender categories.
- Blood group (A, B, AB, O).
- Disease status (Yes/No).
- Treatment group (Drug A / Drug B).

## B. Ordinal Data

Data that have a specific order, but the differences between categories are not necessarily equal.

**Medical examples:**
- Pain severity (mild, moderate, severe).
- Cancer stages (I, II, III, IV).
- Satisfaction levels (low, medium, high).

## C. Continuous Data

Numerical data that can take many possible values.

**Medical examples:**
- Blood pressure (120 mmHg).
- Body weight (70.5 kg).
- Blood glucose (95 mg/dL).
- Cholesterol (180 mg/dL).
- Body temperature (37.2°C).

## D. Discrete Data (Count Data)

Numerical data representing counts.

**Medical examples:**
- Number of hospital visits.
- Number of infections.
- Number of seizures.
- Number of patients admitted.

---

# 2. Normality Testing (Normalverteilung)

## What Is Normality?

Normality means that data follows approximately a normal distribution, which has a symmetric, bell-shaped curve centered around the mean.

## Key Properties of a Normal Distribution

1. **Symmetry:** Mean, median, and mode are approximately equal, and the left and right sides mirror each other.

2. **Empirical Rule (68–95–99.7 Rule):**
   - Approximately 68% of observations fall within 1 standard deviation of the mean.
   - Approximately 95% fall within 2 standard deviations.
   - Approximately 99.7% fall within 3 standard deviations.

3. **Medical examples:**
   - Adult height.
   - Resting heart rate in healthy cohorts.
   - Systolic blood pressure in large homogeneous populations.

**Often skewed in medical data:**
- Hospital length of stay.
- Biomarker concentrations (e.g., CRP, viral load).
- Treatment costs.

## Why Normality Matters in Biostatistics

Normality helps determine whether parametric tests or non-parametric alternatives are appropriate.

**Parametric tests:**
- Independent samples t-test.
- Paired samples t-test.
- ANOVA.
- Pearson correlation.

**Non-parametric tests:**
- Mann-Whitney U test.
- Wilcoxon signed-rank test.
- Kruskal-Wallis test.
- Spearman rank correlation.

**Important considerations:**

- In regression and linear models, residual normality (errors around the fitted model) is generally more critical than raw input feature normality.
- With large sample sizes, the Central Limit Theorem means sampling distributions of means often approximate normality even when individual observations are skewed.
- Severe skewness or extreme outliers still warrant caution.

## How to Assess Normality

### A. Visual Methods (Essential)

**1. Histograms and Density Plots**

Check:
- Symmetry.
- Unimodality.
- Skewness.
- Heavy tails.

**2. Q-Q Plots (Quantile-Quantile Plots)**

Compare sample quantiles against theoretical normal quantiles.

- Points following a straight diagonal line indicate approximate normality.
- Systematic deviations indicate departures from normality.

**3. Boxplots**

Highlight:
- Asymmetry.
- Extreme outliers.
- Distribution spread.

### B. Numerical and Formal Tests

**1. Skewness and Kurtosis**

Quantify:
- Skewness: Tail asymmetry.
- Kurtosis: Tail weight and peakedness.

**2. Shapiro-Wilk Test**

- Widely used for small to moderate sample sizes.
- A small p-value (typically less than 0.05) suggests departure from normality.

**3. Kolmogorov-Smirnov and Anderson-Darling Tests**

Alternative goodness-of-fit tests.

- Kolmogorov-Smirnov test compares empirical and theoretical distributions.
- Anderson-Darling test gives greater weight to distributional differences in the tails.
- Both can be sensitive to sample size, where tiny, practically unimportant deviations may become statistically significant.

## Practical Workflow and Handling Non-Normality

**Important principle:**

Never rely on a p-value alone. Always combine statistical tests with Q-Q plots, histograms, and clinical or domain knowledge.

### Options When Data Are Non-Normal

1. **Use non-parametric tests:**
   - Appropriate for rank-based comparisons and certain ordinal or non-normally distributed outcomes.

2. **Apply transformations:**
   - Log transformation.
   - Square-root transformation.
   - Particularly useful for positively skewed laboratory values when clinically interpretable.

3. **Use alternative statistical models:**
   - Generalized linear models (GLMs).
   - Bootstrap methods.
   - Appropriate models for count data, proportions, or heavily skewed outcomes.

---

# 3. Quantile-Quantile (Q-Q) Plots for Biostatisticians

A normal Q-Q plot graphs sorted observed sample quantiles against expected quantiles from a theoretical normal distribution.

When points cluster closely along the reference diagonal line, the distribution approximates normality.

Systematic deviations reveal specific distributional departures in biomedical data.

## Reading Q-Q Plot Shapes in Medical Data

| Q-Q Plot Pattern | Visual Shape | Biostatistics Meaning and Medical Example |
|---|---|---|
| Normal alignment | Points track the diagonal line across the center and tails. | Approximate normality; supports parametric methods (e.g., resting heart rate or systolic BP in a uniform cohort). |
| Right-skewed (positively skewed) | Concave-up curve bending above the line at high quantiles. | Long upper tail with extreme high values; common in C-reactive protein (CRP), viral load, hospital stay, or healthcare costs. |
| Left-skewed (negatively skewed) | Concave-down curve dropping below the line at low quantiles. | Long lower tail; seen in floor-bounded scores or biomarkers approaching a lower assay limit. |
| Heavy-tailed (leptokurtic) | S-shaped curve dipping low on the left and rising high on the right. | More extreme values than a normal curve; signals outlier sensitivity in t-tests or linear regression. |
| Light-tailed (platykurtic) | Inverse S-shape flattening at both extremes. | Fewer extreme values than expected under normality (e.g., bounded or truncated scores). |
| Discrete / bimodal steps | Staircase steps or distinct jumps/clusters. | Integer counts, ordinal scales, or mixed subgroups (e.g., diseased vs. healthy patients combined). |

---

# Key Takeaway

The correct statistical analysis depends on:

1. The research question.
2. The type of data.
3. The distribution of the data.
4. The number of groups being compared.
5. Whether observations are independent or paired.
6. Whether statistical assumptions are satisfied.

**Remember:** Normality testing is one part of statistical analysis. Choosing the correct test requires understanding the study design, outcome variable, and research hypothesis.

# Practical Guidance for Biostatisticians

## 1. Inspect the Tails First

- Center deviations often matter less than tail departures.
- Tail departures can drive outliers, variance inflation, and parametric test error rates.
- Pay particular attention to extreme observations in medical datasets.

## 2. Pair with Residual Diagnostics

- In linear models, check Q-Q plots of model residuals rather than raw outcome variables alone.
- Residual diagnostics help determine whether model assumptions are satisfied.

## 3. Account for Sample Size

- **Small cohorts:** Show wider natural sampling variation around the diagonal in Q-Q plots.
- **Large cohorts:** Can make minor tail deviations look prominent, even when mean-based inference remains robust.
- Always interpret normality tests in the context of sample size.

## 4. Choose Action Based on Shape and Study Design

- Consider a **log transformation** for right-skewed positive laboratory values when clinically interpretable.
- Switch to **non-parametric rank tests** or **generalized linear models (GLMs)** when skewness or count-data characteristics persist.
- Avoid discarding genuine outliers without clinical review.
- Consider the clinical meaning of the variable before transforming it.

---

# Biostatistics Checklist: Parametric vs. Non-Parametric Tests

## 1. Confirm the Estimand and Research Question

Check whether you want to compare:

- **Means / mean differences:** Often addressed using parametric methods.
- **Ranks / medians / distributional shifts:** Often addressed using non-parametric methods.

## 2. Check Normality on the Right Quantity

Inspect:

- Histograms.
- Q-Q plots of group distributions (for two-group or multi-group comparisons).
- Model residuals (for regression and ANOVA).

Do not rely on a standalone p-value.

## 3. Evaluate Sample Size and Skewness

- **Large samples with mild skewness:** Mean-based parametric tests are often robust because of the Central Limit Theorem, unless extreme skewness or heavy tails distort power or precision.
- **Small samples or strong skewness/outliers:** Consider non-parametric methods or appropriate transformations/GLMs.

## 4. Check Variance Equality and Outliers

- Look for marked variance differences across groups (heteroscedasticity).
- Identify clinically genuine extreme values.
- Assess whether outliers influence the statistical results.
- Do not automatically remove outliers without clinical review.

## 5. Verify Matching and Pairing Structure

Match the statistical test to:

- Independent groups versus paired/repeated measurements.
- Two groups versus three or more groups.
- The specific study design.

## 6. Preserve Clinical Interpretability

- Avoid unnecessary transformations that make results difficult to interpret.
- Avoid switching to rank tests if the resulting summary obscures clinical meaning.
- Consider generalized linear models when appropriate.

**Examples:**

- Gamma regression: Positive, right-skewed continuous outcomes.
- Negative binomial regression: Overdispersed count data.

---

# Quick Reference: Q-Q Plot Patterns in Biostatistics

| Q-Q Plot Pattern | Visual Shape | Biostatistics Meaning and Medical Example |
|---|---|---|
| Normal alignment | Points follow the diagonal line across the center and tails. | Approximate normality; supports parametric methods. Example: Resting heart rate or systolic blood pressure. |
| Right-skewed (positively skewed) | Curve bends upward above the line at higher quantiles. | Long upper tail with extreme high values. Examples: CRP, viral load, hospital stay, and healthcare costs. |
| Left-skewed (negatively skewed) | Curve bends downward below the line at lower quantiles. | Long lower tail. Examples: Floor-bounded scores or biomarkers approaching a lower assay limit. |
| Heavy-tailed (leptokurtic) | S-shaped curve, dipping below the line on the left and rising above it on the right. | More extreme values than expected under normality; indicates potential outlier sensitivity in t-tests and linear regression. |
| Light-tailed (platykurtic) | Inverse S-shape, flattening at both extremes. | Fewer extreme values than expected under normality. Examples: Bounded or truncated clinical scores. |
| Discrete / bimodal steps | Staircase-like steps, distinct jumps, or separate clusters. | Indicates discrete values, repeated measurements, or two underlying populations. Examples: Ordinal clinical scores or mixed patient subgroups. |

---

# Key Selection Notes for Biostatisticians

## 1. Normality Applies to the Appropriate Target

- Check group distributions or model residuals.
- Consider sample size and potential outliers.
- Do not rely on a normality-test p-value alone.
- Use histograms and Q-Q plots to assess distribution patterns.

**Important:** In linear regression and ANOVA, residual normality is generally more relevant than the normality of the raw outcome variable.

## 2. Non-Parametric Tests Compare Ranks and Distributions, Not Automatically Means

- Non-parametric tests generally compare ranks or distributions rather than directly comparing means.
- They do not automatically test differences in medians.
- If group distributions have markedly different shapes, rank tests may evaluate stochastic dominance or rank shifts rather than pure differences in medians or means.

**Important:** Interpret non-parametric test results according to the specific test and the underlying distributional assumptions.

## 3. Beyond Basic Two-Group and Multi-Group Tests

When adjusting for covariates, handling time-to-event data, or modeling counts and proportions directly, consider regression models, generalized linear models (GLMs), or survival analysis.

### A. Regression Analysis

Use regression models when adjusting for covariates or investigating relationships between variables.

### B. Generalized Linear Models (GLMs)

Use GLMs when modeling outcomes such as counts, proportions, and binary variables.

### C. Survival Analysis

Common survival analysis methods include:

1. **Kaplan-Meier Analysis**
   - Estimates survival probabilities over time.

2. **Log-Rank Test**
   - Compares survival distributions between groups.

3. **Cox Proportional Hazards Regression**
   - Evaluates the association between predictors and time-to-event outcomes.
   - Allows adjustment for multiple covariates.

**Medical examples:**
- Time until death.
- Time until cancer recurrence.
- Time until disease progression.
- Time until hospital readmission.

---

## Key Takeaway

Choose the statistical method according to the research question, outcome variable, study design, and required adjustments.

# Key Takeaways for Biostatisticians

1. Inspect the distribution using histograms and Q-Q plots.
2. Pay particular attention to extreme values and tail deviations.
3. Evaluate normality on the appropriate quantity.
4. Consider sample size when interpreting normality tests.
5. Check variance equality and outliers.
6. Identify whether observations are independent or paired.
7. Choose the appropriate parametric, non-parametric, or regression method.
8. Preserve clinical interpretability.
9. Never select a statistical test based only on the Shapiro-Wilk p-value.

**Golden Rule:**

The choice between parametric and non-parametric tests should depend on the research question, study design, data distribution, sample size, and statistical assumptions—not on a normality-test p-value alone.
