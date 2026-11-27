
# Multiple Imputation (MI) in Biostatistics

## 1. What Is Multiple Imputation?

Multiple Imputation (MI) is a statistical technique used to handle missing data by replacing missing values with several plausible values rather than a single estimated value.

Instead of creating one completed dataset, multiple imputation generates several completed datasets, analyzes each dataset separately, and combines the results to account for uncertainty caused by missing data.

**Why is Multiple Imputation Important in Medical Research?**

Missing data can:
- Reduce statistical power.
- Introduce selection bias.
- Distort treatment-effect estimates.
- Reduce the reliability of clinical conclusions.

Multiple imputation helps preserve statistical information and reduce bias when its assumptions and imputation models are appropriate.

---

## 2. Clinical Example: Missing Blood Pressure Measurements

Imagine a clinical trial investigating whether a new antihypertensive drug reduces systolic blood pressure.

The study includes 500 patients divided into two groups:

- Treatment group: 250 patients.
- Control group: 250 patients.

The researchers collect:
- Age.
- Gender.
- BMI.
- Baseline systolic blood pressure.
- Follow-up systolic blood pressure.
- Treatment group.

At the end of the study, 15% of follow-up blood pressure measurements are missing.

### Clinical Problem

Some patients miss their follow-up appointments.

If the biostatistician analyzes only patients with complete measurements, the results may be biased, particularly if missingness is associated with patient characteristics.

### Multiple Imputation Approach

The biostatistician:

1. Investigates the missing data pattern.
2. Evaluates whether MAR is a plausible assumption.
3. Creates multiple imputed datasets.
4. Analyzes each completed dataset.
5. Combines estimates using Rubin's Rules.
6. Evaluates the clinical interpretation and sensitivity of the results.

---

## 3. Rubin's Rules

Rubin's Rules are mathematical rules used to combine statistical results from multiple imputed datasets.

Suppose the biostatistician generates 5 imputed datasets.

Each dataset produces:
- A treatment-effect estimate.
- A standard error.
- A variance estimate.

Rubin's Rules combine these results into one overall estimate.

### A. Pooled Estimate

The pooled estimate is the average of the estimates across all imputed datasets.

\[
\bar{Q}=\frac{1}{m}\sum_{i=1}^{m}Q_i
\]

Where:

- \(\bar{Q}\) = pooled estimate.
- \(m\) = number of imputed datasets.
- \(Q_i\) = estimate from imputed dataset \(i\).

### B. Within-Imputation Variance

\[
\bar{U}=\frac{1}{m}\sum_{i=1}^{m}U_i
\]

Where:

- \(\bar{U}\) = average within-imputation variance.
- \(U_i\) = variance estimate from dataset \(i\).

### C. Between-Imputation Variance

\[
B=\frac{1}{m-1}\sum_{i=1}^{m}(Q_i-\bar{Q})^2
\]

Where:

- \(B\) = between-imputation variance.
- It measures how much the estimates differ across imputed datasets.

### D. Total Variance

\[
T=\bar{U}+\left(1+\frac{1}{m}\right)B
\]

Where:

- \(T\) = total variance.
- \(\bar{U}\) = within-imputation variance.
- \(B\) = between-imputation variance.

**Important:** Total variance includes both uncertainty within each dataset and uncertainty caused by missing data.

---

## 4. Multiple Imputation Workflow

### Step 1: Explore Missing Data

- Calculate missing percentages.
- Identify variables with missing values.
- Examine missingness patterns.
- Investigate possible MCAR, MAR, or MNAR mechanisms.

### Step 2: Select Variables for Imputation

Include relevant variables such as:

- Outcome variables.
- Treatment group.
- Age.
- Gender.
- Baseline measurements.
- Important clinical predictors.
- Variables associated with missingness.

Include auxiliary variables that help predict missing values when appropriate.

### Step 3: Select Imputation Methods

The method depends on the variable type.

| Variable Type | Possible Imputation Method | Medical Example |
|---|---|---|
| Continuous | Predictive Mean Matching (PMM) | Blood pressure |
| Binary | Logistic regression | Diabetes (Yes/No) |
| Nominal | Multinomial logistic regression | Blood group |
| Ordinal | Proportional odds model | Pain severity |
| Count | Appropriate count regression model | Number of hospital visits |

### Step 4: Generate Multiple Imputed Datasets

Create several completed versions of the original dataset.

For example:

- Imputation 1.
- Imputation 2.
- Imputation 3.
- Imputation 4.
- Imputation 5.

Each dataset contains different plausible values for the missing observations.

### Step 5: Analyze Each Dataset

Apply the same statistical model to every imputed dataset.

Example:

Linear regression:

\[
SBP_{follow-up} =
\beta_0+\beta_1 Treatment+\beta_2 Age+\beta_3 BMI
\]

### Step 6: Pool the Results

Use Rubin's Rules to combine:

- Regression coefficients.
- Standard errors.
- Confidence intervals.
- P-values.

### Step 7: Evaluate the Results

- Check imputation convergence.
- Assess plausibility of imputed values.
- Compare observed and imputed distributions.
- Evaluate sensitivity to alternative assumptions.
- Report the imputation procedure transparently.

---

## 5. Implement Multiple Imputation in R Using the mice Package

### Step 1: Install and Load the Package

```r
install.packages("mice")
library(mice)
