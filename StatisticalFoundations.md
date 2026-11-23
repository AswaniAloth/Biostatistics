# Biostatistics in Clinical Research
- Notes for Biostatisticians and Clinical Researchers Statistical foundations

## Topics covered:

- Null and Alternative Hypotheses (H₀ and H₁)
- Types of Alternative Hypotheses
- P-values and Statistical Significance
- Statistical Power
- Confidence Intervals (CI)
- Type I and Type II Errors
- Clinical Research Examples
- Medical and Nursing Documentation
- Practice Questions

## 1. Null and Alternative Hypotheses (H₀ and H₁)
### 1.1 Introduction

- In medical research, statistical hypotheses are used to investigate whether a new treatment, medication, or medical intervention has an effect.

-There are two competing hypotheses:

#### Null Hypothesis (H₀)

- The null hypothesis states that there is no effect, no difference, or no relationship between the variables being studied.

- Any observed difference may be explained by random variation.
- It usually contains an equality sign (=).
#### Alternative Hypothesis (H₁ or Hₐ)

- The alternative hypothesis states that there is an effect, difference, or relationship.

- It represents the research hypothesis.
- It uses one of three mathematical symbols: ≠, <, or >.

### 1.2 Medical Example: Does a New Drug Reduce Blood Pressure?

- Suppose researchers want to investigate whether a new medication reduces systolic blood pressure in patients with hypertension.

- Given:

- Average systolic blood pressure before treatment: 150 mmHg.
- Researchers administer a new medication.
- They want to investigate whether the medication reduces blood pressure.

## Null hypothesis (H₀):

- The medication does not reduce the average systolic blood pressure relative to the reference value.

- H₀: μ = 150 mmHg

## Alternative hypothesis (H₁):

- The medication reduces the average systolic blood pressure.

- H₁: μ < 150 mmHg

- Where:

- μ = True population mean systolic blood pressure after treatment.

## Understanding the Difference

| Hypothesis | Meaning |
|---|---|
| H₀ | No reduction from the reference value |
| H₁ | Average blood pressure is lower than the reference value |

**Important:** This is a one-sample comparison against a reference value. In a randomized clinical trial comparing two groups, the hypotheses should generally compare the treatment effect between groups.

### 1.3 Medical Example: Does a New Treatment Reduce Recovery Time?

Suppose a hospital introduces a new treatment for patients recovering from surgery.

**Traditional treatment:**

Average recovery time = 10 days.

Researchers want to investigate whether the new treatment reduces recovery time.

**Null hypothesis (H₀):**

H₀: μ = 10 days

**Alternative hypothesis (H₁):**

H₁: μ < 10 days

**Interpretation:**

- H₀: Average recovery time is equal to the reference value.
- H₁: Average recovery time is lower than the reference value.

### 1.4 Types of Alternative Hypotheses

There are three common types of alternative hypotheses.

| Type | Hypothesis | Meaning | Medical Example |
|---|---|---|---|
| Two-tailed | H₁: μ ≠ 150 | Any difference | Does a drug change blood pressure? |
| Left-tailed | H₁: μ < 150 | Decrease | Does a drug reduce blood pressure? |
| Right-tailed | H₁: μ > 150 | Increase | Does a treatment increase haemoglobin? |

#### 1. Two-Tailed Test

Used when researchers want to investigate whether a treatment produces any difference, regardless of direction.

**Example:**

Does a new medication change the average systolic blood pressure?

#### 2. Left-Tailed Test

Used when researchers specifically investigate whether a value decreases.

**Example:**

Does a new medication reduce blood glucose levels?

#### 3. Right-Tailed Test

Used when researchers specifically investigate whether a value increases.

**Example:**

Does iron supplementation increase haemoglobin levels?

**Exam Tip:** The direction of the alternative hypothesis should be determined before examining the study results.

---

### 1.5 How Do We Make a Statistical Decision?

After collecting patient data, researchers perform an appropriate statistical test and calculate a **p-value**.

A commonly used significance level is:

$$
\alpha = 0.05
$$

#### Decision Rules

- If p < 0.05: **Reject H₀.**
- If p ≥ 0.05: **Fail to reject H₀.**

#### Clinical Example

A study investigates whether a new blood pressure medication reduces systolic blood pressure.

**Results:**

- Significance level: α = 0.05
- P-value: p = 0.02

Since:

$$
0.02 < 0.05
$$

**Decision:** Reject H₀.

**Conclusion:**

There is statistically significant evidence that the medication reduces average systolic blood pressure, assuming the study design and statistical test are appropriate.

**Important:** Rejecting H₀ does not prove that the medication works. Statistical significance does not automatically indicate clinical importance.

### 1.6 Important Points for Exams

- **H₀:** Represents the null hypothesis.
- **H₁:** Represents the alternative hypothesis.
- **H₀** usually contains equality (=).
- **H₁** uses ≠, <, or >.
- The **p-value** helps researchers make a statistical decision.
- Statistical significance does not necessarily mean clinical significance.
- Failure to reject H₀ does not prove that H₀ is true.
## 2. Statistical Power

### 2.1 Definition

Statistical power is the probability that a statistical test correctly detects a specified true treatment effect when that effect exists.

In simple terms, power tells us how likely a clinical study is to detect a treatment effect of the size specified in the study design.

### 2.2 Formula

$$
\text{Power} = 1 - \beta
$$

Where:

- **β** = Probability of Type II error.
- **1 − β** = Statistical power.

### 2.3 Clinical Example

A clinical researcher wants to investigate whether a new medication reduces blood pressure in patients with hypertension.

The researcher plans a clinical trial with 200 patients.

**Study Design:**

- Significance level (α): 0.05.
- Statistical power: 80%.
- Type II error (β): 20%.

**Interpretation:**

If the treatment truly has the effect specified in the study design, the study has an 80% probability of detecting a statistically significant result under the planned assumptions.

### 2.4 Understanding 80% Statistical Power

| Statistical Concept | Value |
|---|---:|
| Statistical power | 80% |
| Type II error (β) | 20% |
| Significance level (α) | 5% |

Power and Type II error are complementary:

$$
\text{Power} = 1 - \beta
$$

### 2.5 Factors Affecting Statistical Power

#### 1. Sample Size

Larger sample sizes generally increase statistical power.

**Example:**

A study involving 500 patients will generally have greater power than a comparable study involving 50 patients.

#### 2. Effect Size

Larger treatment effects are generally easier to detect.

**Example:**

A medication that reduces systolic blood pressure by 20 mmHg may be easier to detect statistically than one that reduces it by 2 mmHg.

#### 3. Variability

Lower variability generally increases statistical power.

When patient measurements are highly variable, identifying a true treatment effect becomes more difficult.

#### 4. Significance Level (α)

Increasing α generally increases statistical power but also increases the risk of Type I error.

#### 5. Study Design

Appropriate study design and efficient statistical methods can improve statistical power.
**Examples:**

- Randomized controlled trials.
- Appropriate outcome measurements.
- Stratification where appropriate.
- Repeated measurements where appropriate.

### 2.6 Important Points

- Commonly used statistical power levels are **80% and 90%**.
- Power should be calculated before starting a clinical trial.
- Insufficient power may result in missing a clinically important treatment effect.
- Sample size calculation depends on power, significance level, effect size, variability, and study design.
- Power is conditional on the assumed treatment effect and statistical model.
## 3. Confidence Interval (CI)

### 3.1 Definition

A confidence interval is a range of values used to estimate an unknown population parameter based on sample data.

In simple terms, a confidence interval tells us how precise our estimate is.

The most commonly used confidence interval in clinical research is the **95% confidence interval**.

### 3.2 Formula

For a population mean with an estimated standard error, using a normal approximation:

$$
95\% \ CI = \bar{x} \pm 1.96 \times SE
$$

Where:

- **x̄** = Sample mean.
- **SE** = Standard error.
- **1.96** = Approximate critical value for a two-sided 95% confidence interval under a normal approximation.

For small samples with an estimated standard deviation, a **t-distribution critical value** is generally used instead.

### 3.3 Clinical Example: Blood Pressure Reduction

A researcher investigates whether a new medication reduces systolic blood pressure.

**Study Results:**

- Mean blood pressure reduction = 10 mmHg.
- 95% CI = 7 to 13 mmHg.

**Interpretation:**

We are 95% confident that the true average reduction in systolic blood pressure lies between 7 and 13 mmHg, under the assumptions of the statistical method.

### 3.4 How to Interpret Confidence Intervals

#### 1. Narrow Confidence Interval

A narrow CI indicates a more precise estimate.

#### 2. Wide Confidence Interval

A wide CI indicates a less precise estimate.

#### 3. Confidence Interval Containing the Null Value

Usually indicates that the result is not statistically significant at the corresponding two-sided 5% significance level.

#### 4. Confidence Interval Excluding the Null Value

Usually indicates statistical significance at the corresponding two-sided 5% significance level.

### 3.5 Null Values for Different Statistical Measures

The null value depends on the statistical measure.

| Statistical Measure | Null Value |
|---|---:|
| Mean difference | 0 |
| Risk difference | 0 |
| Relative risk (RR) | 1 |
| Odds ratio (OR) | 1 |
| Hazard ratio (HR) | 1 |

**Explanation:**

- A mean difference of zero means no difference between groups.
- A risk difference of zero means no difference in risk.
- An RR of one means equal risk between groups.
- An OR of one means equal odds between groups.
- An HR of one means equal hazards between groups.

### 3.6 Clinical Example: Comparing Two Drugs

Suppose a clinical trial compares Drug A with Drug B.

**Results:**

- Mean difference in blood pressure reduction = 5 mmHg.
- 95% CI = 2 to 8 mmHg.

Since the confidence interval does not contain zero, the difference is statistically significant at the 5% level using the corresponding two-sided test.

**Interpretation:**

Drug A produces an estimated 5 mmHg greater reduction in blood pressure than Drug B, assuming the difference is defined as Drug A minus Drug B.
## 4. Type I Error (False Positive)

### 4.1 Definition

Type I error occurs when researchers reject the null hypothesis (H₀), even though it is actually true.

In simple terms, researchers conclude that a treatment has an effect when no effect exists under the null hypothesis.

### 4.2 Formula

$$
P(\text{Type I Error}) = \alpha
$$

Usually:

$$
\alpha = 0.05 = 5\%
$$

### 4.3 Clinical Example

Researchers conduct a clinical trial to evaluate a new cancer medication.

**Hypotheses:**

- H₀: The new medication does not improve survival compared with standard treatment.
- H₁: The new medication improves survival.

Suppose the new medication actually has no improvement in survival.

However, the statistical analysis produces a significant result.

Researchers reject H₀ and conclude that the medication improves survival.

This is a **Type I error (false positive).**

### 4.4 Consequences in Clinical Research

- An ineffective drug may be considered effective.
- Patients may receive unnecessary treatment.
- Healthcare costs may increase.
- Incorrect findings may influence future clinical guidelines.
- Further research may be based on misleading conclusions.
  ## 5. Type II Error (False Negative)

### 5.1 Definition

Type II error occurs when researchers fail to reject the null hypothesis (H₀), even though it is actually false.

In simple terms, researchers fail to detect a real treatment effect.

### 5.2 Formula

$$
P(\text{Type II Error}) = \beta
$$

For example:

$$
\beta = 0.20 = 20\%
$$

### 5.3 Clinical Example

A clinical researcher investigates whether a new medication reduces blood glucose levels in diabetic patients.

**Hypotheses:**

- H₀: The medication has no treatment effect.
- H₁: The medication reduces blood glucose.

Suppose the medication truly reduces blood glucose, but the clinical trial includes too few participants to detect the effect reliably.

The study produces a non-significant result, and researchers fail to reject H₀.

This is a **Type II error (false negative).**

### 5.4 Consequences in Clinical Research

- An effective treatment may be overlooked.
- Further research may be delayed.
- Patients may miss a potentially beneficial treatment.
- Resources may be spent repeating underpowered studies.
## 6. Difference Between Type I and Type II Errors

| Feature | Type I Error | Type II Error |
|---|---|---|
| Meaning | False positive | False negative |
| Decision | Reject true H₀ | Fail to reject false H₀ |
| Probability | α | β |
| Common value | 5% | 20% |
| Related concept | Significance level | Statistical power |

### Easy Way to Remember

**Type I Error (False Positive):**

Finding an effect that is not really there.

**Type II Error (False Negative):**

Missing an effect that is really there.
## 7. P-value

### 7.1 Definition

A p-value is the probability, assuming the null hypothesis is true and the statistical model assumptions hold, of obtaining results at least as extreme as those observed.

In simple terms, the p-value helps us assess how compatible the observed data are with the null hypothesis.

### 7.2 Common Significance Threshold

A commonly used threshold is:

$$
p < 0.05
$$

This is conventionally considered statistically significant when α = 0.05.

### 7.3 Clinical Example

Researchers investigate whether a new medication reduces blood pressure.

**Study Results:**

- Mean blood pressure reduction = 8 mmHg.
- P-value = 0.03.
- Significance level = 0.05.

**Decision:**

$$
0.03 < 0.05
$$

Therefore:

- Reject H₀.
- The result is statistically significant.

**Interpretation:**

There is statistically significant evidence that the medication reduces average blood pressure, assuming the study was appropriately designed and analysed.

### 7.4 Understanding Different P-values

| P-value | General Interpretation |
|---|---|
| 0.001 | Strong evidence against H₀ |
| 0.01 | Statistically significant |
| 0.03 | Statistically significant |
| 0.05 | At the conventional threshold |
| 0.08 | Not statistically significant at α = 0.05 |
| 0.20 | Not statistically significant at α = 0.05 |

**Important:** The strength of evidence should not be interpreted using rigid p-value categories alone.

### 7.5 Important Mistakes to Avoid

A p-value of 0.03 does **NOT** mean:

- There is a 3% probability that H₀ is true.
- There is a 97% probability that the treatment works.
- The treatment is clinically important.
- The result is free from bias.
- There is a 3% probability that the finding occurred by chance in the everyday sense.

**Remember:** A p-value does not measure the size or clinical importance of a treatment effect.
## 8. How These Concepts Work Together in Clinical Research

Consider a randomized controlled trial (RCT) evaluating a new medication for hypertension.

### 8.1 Application of Statistical Concepts

| Concept | Application in Clinical Research |
|---|---|
| Hypothesis testing | Defines the research question using H₀ and H₁ |
| Statistical power | Determines the probability of detecting the planned treatment effect |
| Confidence interval | Estimates the treatment effect and its precision |
| Type I error | Risk of falsely concluding that a treatment has an effect |
| Type II error | Risk of failing to detect a real treatment effect |
| P-value | Measures compatibility of the observed data with H₀ |

### 8.2 Complete Clinical Trial Example

Suppose researchers conduct a randomized controlled trial to evaluate a new medication for hypertension.

**Study Characteristics:**

- Total sample size: 300 patients.
- Statistical power: 80%.
- Significance level: 5%.
- Mean treatment effect: 8 mmHg greater reduction with the new medication.
- 95% CI: 4 to 12 mmHg.
- P-value: 0.001.

#### Statistical Interpretation

1. The study was designed with 80% power to detect the prespecified treatment effect under its assumptions.

2. The estimated treatment effect was an 8 mmHg greater reduction in systolic blood pressure.

3. The 95% CI suggests that the true mean treatment effect may plausibly lie between 4 and 12 mmHg.

4. The p-value of 0.001 indicates strong evidence against the null hypothesis.

5. Since p < 0.05 and the CI excludes zero, the result is statistically significant.

#### Clinical Interpretation

Researchers must also consider:

- Clinical relevance of the reduction.
- Adverse events and safety.
- Study limitations.
- Risk of bias.
- Patient characteristics.
- Generalizability of the findings.

**Important:** Statistical significance alone is not sufficient to recommend a medication.
## 9. Medical Documentation: How to Write a Good Medical Note

### 9.1 Definition

A good medical note should be clear, accurate, professional, and easy to understand.

It should document:

- Patient condition.
- Symptoms.
- Clinical assessment.
- Treatment.
- Management plan.
- Response to treatment.

### 9.2 Example of a Medical Note

**Patient:** Example Patient A  
**Age:** 45 years  
**Date:** 20 November 2026

#### Chief Complaint

Patient presents with fever, cough, and difficulty breathing for the past three days.

#### History of Present Illness (HPI)

Patient reports a three-day history of fever, dry cough, and mild shortness of breath. Symptoms have gradually worsened. Patient denies chest pain or vomiting.

#### Vital Signs

| Parameter | Measurement |
|---|---|
| Blood pressure | 125/80 mmHg |
| Heart rate | 96 bpm |
| Temperature | 38.2°C |
| Respiratory rate | 22/min |
| Oxygen saturation | 95% on room air |

#### Physical Examination

- **General:** Patient appears tired but alert and oriented.
- **Respiratory:** Mild crackles heard in the right lower lung field.
- **Cardiovascular:** Regular heart rhythm.
- **Abdomen:** Soft and non-tender.

#### Assessment / Diagnosis

Suspected lower respiratory tract infection. Further assessment may be required to exclude pneumonia.

#### Treatment / Management Plan

- Monitor vital signs regularly.
- Encourage adequate fluid intake, if clinically appropriate.
- Assess oxygen saturation.
- Arrange further investigations as clinically indicated.
- Administer medication as prescribed.
- Review the patient's condition and response to treatment.

#### Evaluation

Patient remains alert and clinically stable at the time of assessment. Continue monitoring and reassess symptoms.

### 9.3 Example of a Nursing Progress Note

**Date/Time:** 20/11/2026 – 10:00

Patient received in bed, awake, alert, and oriented to time, place, and person.

Patient complains of mild abdominal pain (4/10). Vital signs checked and documented. Medication administered as prescribed. Patient encouraged to increase oral fluid intake where appropriate.

No signs of acute distress observed. Patient remains under observation.

**Nurse's signature:** __________

### 9.4 Important Tips for Writing Good Medical Notes

- Use professional medical language.
- Write short, clear sentences.
- Document facts, not assumptions.
- Include date and time.
- Record vital signs accurately.
- Document medications and treatments actually given.
- Record the patient's response to treatment.
- Avoid unclear abbreviations.
- Never document care that was not provided.
- Maintain patient confidentiality.

### 9.5 Useful Medical Documentation Phrases

| Situation | Professional Wording |
|---|---|
| Patient is okay | Patient appears clinically stable. |
| Patient has pain | Patient reports pain rated 6/10. |
| Patient is sleeping | Patient observed resting comfortably. |
| Patient refuses medication | Patient declined medication; reason documented where available. |
| Patient has fever | Patient noted to be febrile. |
| Patient is improving | Patient shows clinical improvement. |
| Patient has difficulty breathing | Patient reports shortness of breath. |
| Doctor was informed | Physician notified of patient's condition. |

### Five Important Questions a Good Medical Note Should Answer

1. What happened?
2. What did the patient complain about?
3. What did you observe?
4. What action did you take?
5. What was the patient's response?

**Important:** Medical documentation must reflect actual observations and care provided. Use anonymized or fictional patient details in educational examples.

# 10. Practice Questions for Revision

## Question 1: Null and Alternative Hypotheses

A researcher wants to investigate whether a new medication reduces average blood glucose levels in diabetic patients.

The reference average blood glucose level is 180 mg/dL.

Which are the correct hypotheses?

A. H₀: μ = 180; H₁: μ < 180

B. H₀: μ < 180; H₁: μ = 180

C. H₀: μ > 180; H₁: μ = 180

D. H₀: μ ≠ 180; H₁: μ = 180

**Correct answer: A**

**Explanation:** Since the research objective is to investigate a reduction, the alternative hypothesis is left-tailed.

---

## Question 2: Statistical Power

A clinical trial has 90% statistical power.

What is the probability of Type II error?

A. 5%

B. 10%

C. 20%

D. 90%

**Correct answer: B**

**Explanation:**

β = 1 − Power

β = 1 − 0.90 = 0.10 = 10%

---

## Question 3: Confidence Interval

A clinical trial reports a mean treatment difference of 5 mmHg with a 95% CI of 2 to 8 mmHg.

What does this indicate?

A. The confidence interval includes zero.

B. The result is statistically significant at the corresponding two-sided 5% level.

C. The treatment has no effect.

D. There is a 95% probability that the null hypothesis is true.

**Correct answer: B**

**Explanation:** The confidence interval excludes zero, indicating statistical significance at the corresponding two-sided 5% level.

---

## Question 4: Type I Error

Researchers conclude that a new medication is effective when, in reality, it has no effect under the null hypothesis.

What type of error has occurred?

A. Type I error

B. Type II error

C. Sampling error

D. Measurement error

**Correct answer: A**

**Explanation:** Type I error occurs when researchers reject a true null hypothesis.

---

## Question 5: Type II Error

A clinical trial fails to detect a genuine treatment effect.

What type of error may have occurred?

A. Type I error

B. Type II error

C. False positive

D. None of the above

**Correct answer: B**

**Explanation:** Type II error occurs when researchers fail to reject a false null hypothesis.

---

## Question 6: P-value

A clinical trial produces a p-value of 0.02.

The significance level is 0.05.

What is the correct decision?

A. Accept H₀ as true.

B. Reject H₀.

C. The treatment has a 98% probability of working.

D. The study has 98% statistical power.

**Correct answer: B**

**Explanation:** Since 0.02 < 0.05, researchers reject H₀.

---

# 11. Quick Revision Summary

| Concept | Key Definition / Formula |
|---|---|
| Null hypothesis | H₀: No effect or difference |
| Alternative hypothesis | H₁: Effect or difference exists |
| Significance level | α, commonly 0.05 |
| P-value | Probability of equally or more extreme data, assuming H₀ and model assumptions |
| Statistical power | 1 − β |
| Type I error | α |
| Type II error | β |
| Confidence interval | Estimate ± critical value × SE |
| Mean difference null value | 0 |
| Risk difference null value | 0 |
| Relative risk null value | 1 |
| Odds ratio null value | 1 |
| Hazard ratio null value | 1 |

---

# 12. Final Exam Tips

- H₀ = No effect or no difference.
- H₁ = Effect or difference.
- p < 0.05 = Conventionally statistically significant at α = 0.05.
- Power = 1 − β.
- Type I error = False positive.
- Type II error = False negative.
- Narrow CI = Greater precision.
- Wide CI = Lower precision.
- Mean difference null value = 0.
- RR, OR and HR null value = 1.
- Statistical significance does not necessarily mean clinical significance.

---

# End of Study Notes

**Prepared for revision in biostatistics and clinical research.**
