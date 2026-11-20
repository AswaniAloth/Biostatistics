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

    make a good note with medical exsample
    How to Write a Good Medical Note (With Examples)

    A good medical note should be clear, accurate, professional, and easy to understand. It should document the patient's condition, symptoms, assessment, treatment, and plan.
    1. Example of a good medical note

    Patient: John Smith
    Age: 45 years
    Date: 20 November 2026

    Chief Complaint:
    Patient presents with fever, cough, and difficulty breathing for the past three days.

    History of Present Illness (HPI):
    Patient reports a three-day history of fever, dry cough, and mild shortness of breath. Symptoms have gradually worsened. Patient denies chest pain or vomiting.

    Vital Signs:

        Blood pressure: 125/80 mmHg

        Heart rate: 96 bpm

        Temperature: 38.2°C

        Respiratory rate: 22/min

        Oxygen saturation: 95% on room air.

    Physical Examination:

        General: Patient appears tired but alert and oriented.

        Respiratory: Mild crackles heard in the right lower lung field.

        Cardiovascular: Regular heart rhythm.

        Abdomen: Soft and non-tender.

    Assessment / Diagnosis:
    Suspected lower respiratory tract infection. Further assessment may be required to exclude pneumonia.

    Treatment / Management Plan:

        Monitor vital signs regularly.

        Encourage adequate fluid intake.

        Assess oxygen saturation.

        Arrange further investigations as clinically indicated.

        Administer medication as prescribed.

        Review the patient's condition and response to treatment.

    Evaluation:
    Patient remains alert and stable. Continue monitoring and reassess symptoms.
    2. Example of a nursing progress note

    Date/Time: 20/11/2026 – 10:00

    Patient received in bed, awake, alert, and oriented to time, place, and person. Patient complains of mild abdominal pain (4/10). Vital signs checked and documented. Medication administered as prescribed. Patient encouraged to increase oral fluid intake. No signs of acute distress observed. Patient remains under observation.

    Nurse's signature: __________
    3. Important tips for writing good medical notes

        Use professional medical language.

        Write short, clear sentences.

        Document facts, not assumptions.

        Include date and time.

        Record vital signs accurately.

        Document medications and treatments given.

        Record the patient's response to treatment.

        Avoid unclear abbreviations.

        Never document care that was not provided.

        Maintain patient confidentiality.
    4. Useful medical documentation phrases

    Situation
    	

    Professional wording

    Patient is okay
    	

    Patient appears clinically stable.

    Patient has pain
    	

    Patient reports pain rated 6/10.

    Patient is sleeping
    	

    Patient observed resting comfortably.

    Patient refuses medication
    	

    Patient declined medication; reason documented.

    Patient has fever
    	

    Patient noted to be febrile.

    Patient is improving
    	

    Patient shows clinical improvement.

    Patient has difficulty breathing
    	

    Patient reports shortness of breath.

    Doctor was informed
    	

    Physician notified of patient's condition.

    Remember: A good medical note answers five important questions:

        What happened?

        What did the patient complain about?

        What did you observe?

        What action did you take?

        What was the patient's response?

    I can also teach you how to write professional nursing notes, patient reports, and hospital documentation with more practical examples.

    H₀ and H₁: Null and Alternative Hypotheses

    In statistics, we start with two competing statements.

    H₀ (Null hypothesis): There is no effect, no difference, or no relationship.

    H₁ (Alternative hypothesis): There is an effect, a difference, or a relationship.make a good note with medical exsample

    Example: Does a new teaching method improve exam scores?

    Suppose the average exam score with the traditional teaching method is 70.

    We want to test whether a new teaching method improves the average score.

    Our hypotheses are:
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
    H₀

    The medication has no reduction effect.
    H₁

    The medication reduces blood pressure.
    3. Another Medical Example: Does a New Treatment Improve Recovery?

    Suppose a hospital introduces a new treatment for patients recovering from surgery.

    Researchers want to determine whether the new treatment reduces the average recovery time.

        Traditional treatment: Average recovery time is 10 days.

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

    Type
    	

    Hypothesis
    	

    Meaning

    Two-tailed
    	

    H1:μ≠150H1​:μ=150
    	

    There is a difference.

    Left-tailed
    	

    H1:μ<150H1​:μ<150
    	

    The value decreases.

    Right-tailed
    	

    H1:μ>150H1​:μ>150
    	

    The value increases.

    Medical examples:

        Two-tailed: Does a new drug change blood pressure?

        Left-tailed: Does a new drug reduce blood pressure?

        Right-tailed: Does a new treatment increase haemoglobin levels?
    Understanding the Key Stages of Clinical Trials
     
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
    7. Practice Question

    A researcher wants to investigate whether a new medication reduces the average blood glucose level in diabetic patients.

    The average blood glucose level before treatment is 180 mg/dL.

    What are the correct hypotheses?

    Choose the correct answer:
    A. H₀: μ = 180; H₁: μ less than 180
    B. H₀: μ less than 180; H₁: μ = 180
    C. H₀: μ greater than 180; H₁: μ = 180
    D. H₀: μ ≠ 180; H₁: μ = 180

    Exam tip: Always identify what the researcher wants to investigate first. If the aim is to reduce something, use a left-tailed alternative hypothesis (H1:μ<μ0
    H1​:μ<μ0​).

    Power, CI, Type I & II Error, p -values make a note for biostatatistician in clinical research
    Biostatistics in Clinical Research: Power, Confidence Intervals, Type I & Type II Errors, and P-values

    STUDY NOTES FOR BIOSTATISTICIANS AND CLINICAL RESEARCHERS
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

    Understanding 80% power

    80% Power
    80%

    20% Type II error

    80% Power
    Factors affecting statistical power

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

    Estimated treatment effect
    10 mmHg

    95% Confidence Interval: 7–13 mmHg
    Illustration of the estimated effect and confidence interval.

    Interpretation:

    We are 95% confident that the true average reduction in systolic blood pressure lies between 7 and 13 mmHg, under the assumptions of the statistical method.
    How to interpret confidence intervals

        Narrow CI: More precise estimate.

        Wide CI: Less precise estimate.

        CI containing the null value: Usually not statistically significant at the corresponding two-sided 5% level.

        CI excluding the null value: Usually statistically significant at the corresponding two-sided 5% level.

    Important: The null value depends on the measure.

    Statistical measure   Null value
    Mean difference             0
    Risk difference             0
    Relative risk (RR)          1
    Odds ratio (OR)             1 	
    Hazard ratio (HR)           1

    Clinical example: Comparing two drugs

    Suppose a clinical trial compares Drug A with Drug B.

    The mean difference in blood pressure reduction is 5 mmHg.

    95% CI = 2 to 8 mmHg.

    Since the confidence interval does not contain zero, the difference is statistically significant at the 5% level using a corresponding two-sided test.
	
    3. Type I Error (False Positive)
    Definition

    Type I error occurs when researchers reject the null hypothesis (H₀) even though it is actually true.

    In simple words, we conclude that a treatment works when, in reality, it does not have the effect being tested.
    Formula
    P(Type I Error)=α

    Usually:
    α=0.05=5%

    Clinical example

    Researchers conduct a clinical trial to evaluate a new cancer medication.
        H₀: The new medication does not improve survival compared with the standard treatment.
        H₁: The new medication improves survival.

    Suppose the new drug actually has no improvement in survival, but the statistical analysis shows a significant result.
    The researchers reject H₀ and conclude that the medication improves survival.
    This is a Type I error (false positive).

Consequences in clinical research

    An ineffective drug may be considered effective.
    Patients may receive unnecessary treatment.
    Healthcare costs may increase.
    Future clinical guidelines may be influenced by incorrect findings.

4. Type II Error (False Negative)
   
Definition

Type II error occurs when researchers fail to reject the null hypothesis (H₀), even though it is actually false.
In simple words, we conclude that there is insufficient evidence of a treatment effect when a real effect exists.
Formula
P(Type II Error)=β

For example:
β=0.20=20%

Clinical example

A clinical researcher investigates a new medication for reducing blood glucose in diabetic patients.

    H₀: The new medication has no treatment effect.

    H₁: The new medication reduces blood glucose.

Suppose the medication truly reduces blood glucose, but the clinical trial includes too few participants to detect the effect.

The study produces a non-significant result, and researchers fail to reject H₀.

This is a Type II error (false negative).
Consequences in clinical research

    An effective treatment may be overlooked.

    Further research may be delayed.

    Patients may miss a potentially beneficial treatment.

    Resources may be spent repeating underpowered studies.

	5. Difference Between Type I and Type II Errors

Comparison table

Feature         Type I error          Type II error
Meaning          False positive        False negative
Decision         Reject true H₀        Fail to reject false H₀
Probability	       α                     β
Common value	  5%                 	20%
Related concept	Significance level	   Statistical power			

Easy way to remember:

    Type I = Finding an effect that is not really there.
    Type II = Missing an effect that is really there.


6. P-value
Definition

A p-value is the probability, assuming the null hypothesis is true and the statistical model assumptions hold, of obtaining results at least as extreme as those observed.

In simple words, the p-value helps us assess how compatible our observed data are with the null hypothesis.
Common threshold
p<0.05

This is commonly considered statistically significant.

Clinical example
Researchers investigate whether a new drug reduces blood pressure.
The study results are:
Mean reduction in blood pressure: 8 mmHg.
p-value: 0.03.
Significance level: 0.05.
Decision:
0.03<0.05
Statistically significant

Interpretation:
Reject H₀. There is statistically significant evidence that the new medication reduces average blood pressure, assuming the study was appropriately designed and analysed.

Understanding different p-values

P-value                      Interpretation
0.001	                     Strong evidence against H₀
0.01                         Statistically significant
0.03                         Statistically significant
0.05                         At the conventional threshold	
0.08                         Not statistically significant
0.20                         Not statistically significant  
	
Important mistakes to avoid

A p-value of 0.03 does NOT mean:
    There is a 3% probability that H₀ is true.
    There is a 97% probability that the treatment works.
    The treatment is clinically important.
    The result is free from bias.
A p-value does not measure the size or clinical importance of a treatment effect.
	
7. How These Five Concepts Work Together in Clinical Research
Consider a randomized controlled trial (RCT) evaluating a new medication for hypertension

Concept                                   Application in the clinical trial 
Power                                     Determines the probability of detecting the planned treatment effect.
Confidence interval                       Estimates the range of plausible treatment effects.
Type I error                              Risk of falsely concluding that the drug works.
Type II error                             Risk of failing to detect a real treatment effect.
P-value                                   Measures compatibility of the observed results with H₀.
		      

Example of complete clinical trial results

Suppose the researchers report:
Sample size: 300 patients.
    Statistical power: 80%.
    Significance level: 5%.
    Mean blood pressure reduction difference: 8 mmHg.
    95% CI: 4–12 mmHg.
    p-value: 0.001.

Statistical interpretation:

    The study was designed with 80% power to detect the prespecified effect under its assumptions.
    The estimated treatment effect was an 8 mmHg reduction.
    The 95% confidence interval suggests that the true mean treatment effect may plausibly lie between 4 and 12 mmHg.
    The p-value of 0.001 indicates strong evidence against the null hypothesis.
    Since the p-value is below 0.05 and the CI excludes zero, the result is statistically significant.
However, researchers must also consider adverse events, clinical relevance, study limitations, and risk of bias before deciding whether the medication should be recommended.

	






	



	





	






	






	




	


	


