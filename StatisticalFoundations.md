H₀ and H₁: Null and Alternative Hypotheses in Medical Research
1. Introduction

In medical research, we use statistical hypotheses to investigate whether a new treatment, medication, or medical intervention has an effect.

There are two competing hypotheses:

H₀ (Null Hypothesis):

    States that there is no effect, no difference, or no relationship.

    Any observed difference is assumed to be due to chance.

H₁ (Alternative Hypothesis):

    States that there is an effect, a difference, or a relationship.

    Suggests that the treatment or intervention produces a real change.

2. Medical Example: Does a New Drug Reduce Blood Pressure?

Suppose researchers want to investigate whether a new medication reduces blood pressure in patients with hypertension.

    Average blood pressure before treatment: 150 mmHg (systolic).

    Researchers give patients a new medication.

    They want to know whether the medication reduces the average systolic blood pressure.

Our hypotheses are:

Null hypothesis (H₀):

The new medication does not reduce the average systolic blood pressure.
H0:μ=150 mmHg
H0​:μ=150 mmHg

Alternative hypothesis (H₁):

The new medication reduces the average systolic blood pressure.
H1:μ<150 mmHg
H1​:μ<150 mmHg

Here, μ
μ represents the true average systolic blood pressure after treatment in the population being studied.

Understanding the difference
H₀ The medication has no reduction effect.
H1 The medication reduces blood pressure. 

3. Another Medical Example: Does a New Treatment Improve Recovery?

Suppose a hospital introduces a new treatment for patients recovering from surgery.
Researchers want to determine whether the new treatment reduces the average recovery time. Traditional treatment: Average recovery time is 10 days.
New treatment: Researchers want to investigate whether recovery is faster.

Null hypothesis (H₀):

The new treatment does not reduce recovery time.
H0:μ=10 days
H0​:μ=10 days

Alternative hypothesis (H₁):

The new treatment reduces recovery time.
H1:μ<10 days
H1​:μ<10 days

4. Types of Alternative Hypotheses

There are three common ways to formulate hypotheses:

Type               Hypothesis                 Meaning
Two-tailed	       H1:μ≠150                   There is a difference.
Left-tailed       H1:μ<150H1​:μ<150            The value decreases.
Right-tailed      H1:μ>150H1​:μ>150            The value increases.

Medical examples:
    Two-tailed: Does a new drug change blood pressure?
    Left-tailed: Does a new drug reduce blood pressure?
    Right-tailed: Does a new treatment increase haemoglobin levels?

5. How Do We Make a Decision?

After collecting patient data, researchers perform a statistical test and calculate a p-value.

A common significance level is:
α=0.05
α=0.05

    If p-value is less than 0.05: Reject H₀.
    If p-value is greater than or equal to 0.05: Fail to reject H₀.

Example:

A study tests a new blood pressure medication and obtains:
p=0.02
p=0.02

Since:
0.02<0.05
0.02<0.05
We reject H₀.

Conclusion: There is statistically significant evidence that the new medication reduces average blood pressure.
Remember: Rejecting H₀ does not automatically prove that the medication works or that the reduction is clinically important.
6. Important Points to Remember for Exams

    H₀ means no effect or no difference.

    H₁ means an effect or a difference exists.

    The null hypothesis usually contains equality (=).

    The alternative hypothesis uses ≠, less than (less than), or greater than (greater than).

    The p-value helps researchers decide whether to reject H₀.

    Statistical significance does not always mean clinical significance.
1. Statistical Power
Definition

Statistical power is the probability that a statistical test correctly detects a real effect or difference when that effect truly exists.

In simple words, power tells us how likely a clinical study is to find a statistically significant result when a real treatment effect exists.
Formula
Power=1−β
Power=1−β

Where:

    β
    β = Probability of Type II error.

    1−β
    1−β = Statistical power.

Clinical example

A clinical researcher wants to test whether a new drug reduces blood pressure in patients with hypertension.

The researcher plans a clinical trial with 200 patients.

The study is designed with:

    Significance level (α
    α): 0.05

    Statistical power: 80%

    Type II error (β
    β): 20%

Interpretation:

If the new drug truly has the treatment effect specified in the study design, the study has an 80% probability of detecting that effect as statistically significant, under the planned assumptions.
	
actors affecting statistical power

    Sample size: Larger sample sizes generally increase power.

    Effect size: Larger true treatment effects are easier to detect.

    Variability: Lower variability generally increases power.

    Significance level: A higher alpha increases power but also increases the risk of Type I error.

    Study design: Appropriate study design and statistical methods improve efficiency.

Important points

    Commonly used power levels are 80% and 90%.

    Power should be calculated before starting a clinical trial.

    Insufficient power may result in missing a clinically important treatment effect.

    Sample size calculation depends on power, alpha, effect size, variability, and study design.

	2. Confidence Interval (CI)
Definition

A confidence interval is a range of values used to estimate an unknown population parameter based on sample data.

In simple words, a confidence interval tells us how precise our estimate is.

The most commonly used confidence interval in clinical research is the 95% confidence interval.
Formula

For a population mean with an estimated standard error:
95% CI=xˉ±1.96×SE
95%CI=xˉ±1.96×SE

Where:

    xˉ = Sample mean.

    SE = Standard error.

    1.96 = Approximate critical value for a two-sided 95% CI under a normal approximation.

Clinical example

A researcher investigates whether a new medication reduces systolic blood pressure.

After conducting a clinical trial, the results show:

    Mean reduction in blood pressure = 10 mmHg.

    95% CI = 7 to 13 mmHg.

Interpretation:

We are 95% confident that the true average reduction in systolic blood pressure lies between 7 and 13 mmHg, under the assumptions of the statistical method.
How to interpret confidence intervals

    Narrow CI: More precise estimate.

    Wide CI: Less precise estimate.

    CI containing the null value: Usually not statistically significant at the corresponding two-sided 5% level.

    CI excluding the null value: Usually statistically significant at the corresponding two-sided 5% level.

Important: The null value depends on the measure.

Statistical measure                               Null value

Mean difference                                       0
Risk difference                                       0
Relative risk (RR)                                    1
Odds ratio (OR)                                       1
Hazard ratio (HR)                                     1
Clinical example: Comparing two drugs

Suppose a clinical trial compares Drug A with Drug B.
The mean difference in blood pressure reduction is 5 mmHg.

95% CI = 2 to 8 mmHg.

Since the confidence interval does not contain zero, the difference is statistically significant at the 5% level using a corresponding two-sided test.


	







	




	


	


