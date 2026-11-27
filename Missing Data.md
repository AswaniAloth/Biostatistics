
# Missing Data in Biostatistics

Missing data occur when information is unavailable for some variables or observations in a dataset.

Missing data are important in medical research because they can reduce statistical power, introduce bias, and affect the validity of study conclusions.

A biostatistician must identify the missing data mechanism before choosing an appropriate statistical method.

---

## 1. Types of Missing Data Mechanisms

There are three main missing data mechanisms:

### A. MCAR – Missing Completely at Random

**Definition:**

Missingness is completely unrelated to observed or unobserved variables.

In other words, the probability of missing data is the same for every participant.

**Medical example:**

- A laboratory sample is accidentally lost during transportation.
- A computer system randomly fails to save some patient records.
- A questionnaire is accidentally damaged.

**Statistical implications:**

- Missingness does not systematically depend on patient characteristics or clinical outcomes.
- Complete-case analysis can be unbiased under MCAR, although statistical power decreases.
- The observed data represent a random subset of the original study population.

**Possible approaches:**

- Complete-case analysis.
- Multiple imputation, if appropriate.
- Sensitivity analysis.

### B. MAR – Missing at Random

**Definition:**

Missingness depends on observed variables but not on the missing value itself after accounting for the observed information.

**Medical example:**

- Older patients are more likely to miss follow-up appointments.
- Patients with lower income are less likely to complete questionnaires.
- Patients with severe baseline disease are more likely to have missing follow-up laboratory measurements.

**Statistical implications:**

- Missingness is associated with observed patient characteristics.
- Complete-case analysis may introduce bias.
- Multiple imputation can produce valid estimates when the imputation model is appropriately specified.
- The imputation model should include relevant predictors of missingness and the missing values.

**Possible approaches:**

- Multiple imputation (MI).
- Maximum likelihood estimation.
- Inverse probability weighting.
- Sensitivity analysis.

### C. MNAR – Missing Not at Random

**Definition:**

Missingness depends on the unobserved value itself, even after accounting for observed variables.

**Medical example:**

- Patients with very high pain scores are less likely to complete follow-up questionnaires.
- Patients experiencing severe treatment side effects are more likely to discontinue reporting symptoms.
- Patients with worsening disease may avoid follow-up examinations because of their condition.

**Statistical implications:**

- Missingness is related to the missing values themselves.
- Standard multiple imputation under MAR may produce biased results if MNAR is true.
- The mechanism cannot generally be identified from observed data alone.
- Specialized sensitivity analyses are necessary.

**Possible approaches:**

- Pattern-mixture models.
- Selection models.
- Shared-parameter models.
- Delta-adjusted multiple imputation.
- Sensitivity analysis under different MNAR assumptions.

---

## 2. Comparison of MCAR, MAR, and MNAR

| Mechanism | Depends on Observed Data? | Depends on Missing Values? | Medical Example |
|---|---|---|---|
| MCAR | No | No | Randomly lost blood samples |
| MAR | Yes | No, conditional on observed data | Older patients miss follow-up visits |
| MNAR | Possibly | Yes | Patients with severe symptoms avoid reporting them |

---

## 3. Simulating Different Missingness Patterns

A biostatistician can simulate missing data to understand how different mechanisms affect statistical results.

### Example: Clinical Study

Suppose a clinical study includes 1,000 patients.

The researchers collect:

- Age.
- Gender.
- Baseline blood pressure.
- Follow-up blood pressure.
- Treatment group.

The objective is to investigate whether a new treatment reduces blood pressure.

### A. MCAR Simulation

Randomly remove 20% of follow-up blood pressure measurements.

Example:

- 200 measurements are randomly deleted.
- Missingness is unrelated to age, treatment, or blood pressure.

Expected result:

- Reduced sample size.
- Reduced statistical power.
- No systematic selection bias from missingness.

### B. MAR Simulation

Make missingness depend on patient age.

Example:

- Older patients have a higher probability of missing follow-up measurements.
- Younger patients have a lower probability of missing follow-up measurements.

Expected result:

- The observed sample may contain proportionally more younger patients.
- Complete-case analysis may be biased.
- Multiple imputation can help address the missingness if the model includes age and other relevant predictors.

### C. MNAR Simulation

Make missingness depend on the actual follow-up blood pressure.

Example:

- Patients with very high follow-up blood pressure are more likely to have missing measurements.
- Patients with lower follow-up blood pressure are more likely to attend follow-up.

Expected result:

- The observed dataset may underestimate average follow-up blood pressure.
- Treatment effectiveness may appear greater than it actually is.
- Standard MAR-based imputation may not adequately correct the bias.

---

## 4. Clinical and Statistical Implications

| Issue | Clinical Implication | Statistical Implication |
|---|---|---|
| Reduced sample size | Fewer patients contribute information | Reduced statistical power |
| Selection bias | Certain patient groups may be underrepresented | Biased estimates |
| Missing follow-up | Clinical outcomes may be incompletely assessed | Uncertain treatment effects |
| MNAR mechanism | Patients with worse outcomes may be missing | Potentially misleading conclusions |
| Incorrect imputation | Clinical outcomes may be inaccurately represented | Biased estimates and confidence intervals |

---

## 5. How Should a Biostatistician Handle Missing Data?

### Step 1: Identify Missing Data

Calculate the percentage of missing observations for each variable.

Example:

| Variable | Missing Values | Missing Percentage |
|---|---:|---:|
| Age | 5 | 0.5% |
| Gender | 10 | 1% |
| Baseline blood pressure | 20 | 2% |
| Follow-up blood pressure | 200 | 20% |
| Cholesterol | 100 | 10% |

### Step 2: Investigate Missingness Patterns

- Determine which variables have missing observations.
- Identify whether missingness occurs in specific patient groups.
- Examine whether missingness is associated with observed clinical characteristics.
- Investigate reasons for missing follow-up measurements.

### Step 3: Assess the Missingness Mechanism

Consider whether the data are:

- MCAR.
- MAR.
- Potentially MNAR.

**Important:** Statistical tests, such as Little's MCAR test, can help assess evidence against MCAR, but they cannot prove that data are MAR or MNAR.

### Step 4: Select an Appropriate Method

| Missing Data Mechanism | Possible Statistical Approach |
|---|---|
| MCAR | Complete-case analysis or multiple imputation |
| MAR | Multiple imputation or maximum likelihood estimation |
| MNAR | Selection models, pattern-mixture models, or sensitivity analysis |

### Step 5: Perform Sensitivity Analysis

Compare results under different assumptions about missingness.

For example:

- Primary analysis assuming MAR.
- Sensitivity analysis assuming MNAR.
- Compare treatment effects and confidence intervals.

This helps determine whether the study conclusions are robust to missing data assumptions.

---

## 6. Important Concepts for Biostatisticians

**Complete-Case Analysis:**
Uses only participants with complete information for the variables required in the analysis.

**Multiple Imputation:**
Creates several plausible completed datasets, analyzes each dataset, and combines the results to account for uncertainty due to missing data.

**Last Observation Carried Forward (LOCF):**
Uses a participant's last observed measurement to replace a missing later measurement. This method can introduce bias and is generally not recommended as a default approach.

**Sensitivity Analysis:**
Examines whether conclusions change under different assumptions about missing data.

---

## 7. Key Takeaways

1. MCAR: Missingness is unrelated to observed and unobserved data.
2. MAR: Missingness depends on observed information.
3. MNAR: Missingness depends on unobserved values, even after accounting for observed information.
4. Always calculate and report missing data percentages.
5. Investigate why clinical measurements are missing.
6. Do not automatically replace missing values with the mean.
7. Multiple imputation is commonly used under a plausible MAR assumption.
8. MNAR requires additional assumptions and sensitivity analyses.
9. Report the missing data strategy transparently.

**Golden Rule:**

Before handling missing data, understand WHY the data are missing. The missingness mechanism determines which statistical methods are appropriate and how confidently clinical conclusions can be interpreted.

# Study Plan: Missing Data in Biostatistics

## 1. Study Topics and Learning Outcomes

| Study Topic | What to Study / Practice | Expected Learning Outcome |
|---|---|---|
| Missing Data Basics | Definition, causes, types, and patterns of missing data | Understand why missing data occur in clinical research |
| MCAR | Missing Completely at Random; simulate random missingness | Explain statistical and clinical implications of MCAR |
| MAR | Missing at Random; simulate missingness based on observed variables | Understand how observed patient characteristics influence missingness |
| MNAR | Missing Not at Random; simulate missingness based on unobserved values | Understand potential selection bias and limitations of standard imputation |
| Missingness Comparison | Compare MCAR, MAR, and MNAR | Identify and distinguish the three mechanisms |
| Missing Data Visualization | Missing data patterns, heatmaps, and missingness percentages | Identify missingness patterns in clinical datasets |
| Missing Data Handling | Complete-case analysis, mean imputation, and multiple imputation | Select appropriate approaches to missing data |
| Advanced Methods | Maximum likelihood, inverse probability weighting, pattern-mixture models | Understand advanced missing data techniques |
| Sensitivity Analysis | Compare results under MAR and MNAR assumptions | Evaluate the robustness of clinical conclusions |
| Clinical Interpretation | Effects of missing data on treatment effectiveness, bias, and statistical power | Explain clinical and statistical implications |

---

## 2. Practical Exercise

**Objective:** Simulate and analyze different missing data mechanisms using a clinical dataset.

### Tasks

1. Use a simulated dataset of 1,000 patients.
2. Generate MCAR, MAR, and MNAR missingness patterns.
3. Compare missing data percentages.
4. Apply appropriate missing data methods.
5. Compare statistical results before and after handling missing data.
6. Interpret the clinical implications.

---

## 3. Final Study Objective

Understand missing data mechanisms, simulate different missingness patterns, select appropriate statistical methods, and explain their impact on clinical research findings.

**Expected competency:** Be able to identify missing data mechanisms, implement appropriate statistical approaches, perform sensitivity analyses, and interpret the results in medical research.
