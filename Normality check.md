Biostatistics Study Notes
Statistical Analysis for Biostatisticians – With Medical Examples

These notes explain how a biostatistician chooses the correct statistical analysis in medical research, including normality testing, parametric tests, non-parametric tests, regression and survival analysis.

The most important principle is:

First understand the research question, then identify the type of data, check the assumptions, and finally select the appropriate statistical test.
1. Understanding the types of data

Before performing any statistical analysis, a biostatistician must understand the data.

There are four important types of data:
A. Nominal data (categorical data)

Data that can be divided into categories without a specific order.

Medical examples:

    Gender categories.
    Blood group (A, B, AB, O).
    Disease status (Yes/No).
    Treatment group (Drug A / Drug B).

B. Ordinal data
Data that have a specific order, but the differences between categories are not necessarily equal.
Medical examples:
    Pain severity (mild, moderate, severe).
    Cancer stages (I, II, III, IV).
    Satisfaction levels (low, medium, high).

C. Continuous data

Numerical data that can take many possible values.

Medical examples:

    Blood pressure (120 mmHg).
    Body weight (70.5 kg).
    Blood glucose (95 mg/dL).
    Cholesterol (180 mg/dL).
    Body temperature (37.2°C).
D. Discrete data (count data)

Numerical data representing counts.

Medical examples:

    Number of hospital visits.
    Number of infections.
    Number of seizures.
    Number of patients admitted.

2. Normality testing (Normalverteilung)
What is normality?

Normality means that data follows approximately a normal distribution, which has a bell-shaped curve.

Normality means that data follows approximately a normal distribution, which has a symmetric, bell-shaped curve centered around the mean.
Key Properties of a Normal Distribution

    Symmetry: Mean, median, and mode are approximately equal, and the left and right sides mirror each other.

    Empirical Rule (68–95–99.7 Rule): Roughly 68% of observations fall within 1 standard deviation of the mean, 95% within 2 standard deviations, and 99.7% within 3 standard deviations.

    Medical examples: Adult height, resting heart rate in healthy cohorts, or systolic blood pressure in large homogeneous populations. Often skewed in medical data: hospital length of stay, biomarker concentrations (e.g., CRP, viral load), or treatment costs.

Why Normality Matters in Biostatistics

    Determines whether parametric tests (such as t-tests, ANOVA, or Pearson correlation) or non-parametric alternatives (such as Mann-Whitney U, Wilcoxon signed-rank, Kruskal-Wallis, or Spearman rank correlation) are appropriate.
    In regression and linear models, residual normality (errors around the fitted model) is generally more critical than raw input feature normality.
    With large sample sizes, the Central Limit Theorem means sampling distributions of means often approximate normality even when individual observations are skewed, though severe skew or extreme outliers still warrant caution.

How to Assess Normality

    Visual methods (essential):

        Histograms & density plots: Check symmetry, unimodality, skewness, and heavy tails.
        Q-Q plots (quantile-quantile plots): Compare sample quantiles against theoretical normal quantiles; points following a straight diagonal line indicate approximate normality.
        Boxplots: Highlight asymmetry and extreme outliers.

    Numerical & formal tests:

        Skewness and kurtosis: Quantify tail asymmetry and tail weight/peakedness.
        Shapiro-Wilk test: Widely used for small to moderate sample sizes; a small p-value (typically less than 0.05) suggests departure from normality.
        Kolmogorov-Smirnov / Anderson-Darling tests: Alternative goodness-of-fit tests (less sensitive than Shapiro-Wilk in small samples; sensitive to large sample sizes where tiny, practically unimportant deviations can become statistically significant).

Practical Workflow & Handling Non-Normality

    Never rely on a p-value alone: Always pair statistical tests with Q-Q plots, histograms, and clinical/domain context.
    Options when data are non-normal:
    Use non-parametric tests for rank/median comparisons.
    Apply transformations (such as log or square-root transforms for right-skewed positive lab values) when appropriate and clinically interpretable.
     Switch to generalized linear models or bootstrap methods when data are counts, proportions, or heavily skewed.
        
Quantile-Quantile (Q-Q) Plots for Biostatisticians

A normal Q-Q plot graphs sorted observed sample quantiles against expected quantiles from a theoretical normal distribution. When points cluster closely along the reference diagonal line, the distribution approximates normality; systematic deviations reveal specific distributional departures in biomedical data.

Reading Q-Q Plot Shapes in Medical Data

Q-Q Plot Pattern	                           Visual Shape	                                                   Biostatistics Meaning & Medical Example	
Normal alignment	                   Points track the diagonal line across center and tails  	              Approximate normality; supports parametric methods (e.g., resting heart rate or systolic BP in a uniform cohort).	
Right-skewed (positively skewed)	   Concave-up curve bending above the line at high quantiles	          Long upper tail with extreme high values; common in C-reactive protein (CRP), viral load, hospital stay, or healthcare costs.	
Left-skewed (negatively skewed)	      Concave-down curve dropping below the line at low quantiles	          Long lower tail; seen in floor-bounded scores or biomarkers approaching a lower assay limit.	
Heavy-tailed (leptokurtic)	          S-shaped curve dipping low on the left and rising high on the right	  More extreme values than a normal curve; signals outlier sensitivity in t-tests or linear regression.	
Light-tailed (platykurtic)	          Inverse S-shape flattening at both extremes	                          Fewer extreme values than expected under normality (e.g., bounded or truncated scores).	
Discrete / bimodal steps	          Staircase steps or distinct jumps/clusters	                          Integer counts, ordinal scales, or mixed subgroups (e.g., diseased vs. healthy patients combined).	
