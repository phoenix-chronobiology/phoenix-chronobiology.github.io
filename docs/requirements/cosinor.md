![Under Construction](../images/underconstruction.svg)

**Cosinor analysis** uses the [least squares method](../../glossary#least-squares) to fit a sine wave to a time series. Cosinor analysis is often used in the analysis of biologic time series that demonstrate predictible rhythms. This method can be used with an unequally spaced time series.

The Phoenix Biorhythms Platform applies cosinor analysis to a patient's blood pressure and heart rate measurements taken over a defined period, such as 1 day, 2 days, or 7 days. The analysis compares the blood pressure and heart rate profile to healthy peers of the same gender and age group.

The first objective of cosinor analysis is to measure the [MESOR](../../glossary#mesor) of the patient's blood pressure and to detect [MESOR-hypertension](../../glossary#mesor-hypertension). MESOR is a circadian rhythm-adjusted mean. MESOR-hypertension is an elevation of the blood pressure MESOR as validated statistically against the person's own MESOR at another time and/or against a peer reference standard.

The second objective of cosinor analysis is to detect [vascular variability anomalies (VVAs)](../../glossary#vascular-variability-anomaly), which are mathematically defined anomalies in the [circadian](../../glossary#circadian) phase, [amplitude](../../glossary#amplitude) and MESOR, of blood pressure and heart rate.

!!! bug
    Simplify the definitions of _CHAT_, _ecphasia_, and _ecfrequentia_, which come across as wordy jargon. Lean on physiology concepts rather than statistics. Use a follow-on section for each VVA to get into statistical details.

| VVA | Definition |
| --- | ---------- |
| Circadian hyper-amplitude-tension (CHAT) | :material-bug:{: style="color: red;" } An elevation of the 24-hour amplitude of blood pressure above the upper 95% prediction limit of clinically healthy peers matched by gender and age |
| Ecphasia | :material-bug:{: style="color: red;" } Odd circadian blood pressure timing. A deviation of the 24-hour acrophase above the 90% prediction limits of clinically healthy peers matched by gender and age | 
| Ecfrequentia<br>(frequency&nbsp;desynchronization) | :material-bug:{: style="color: red;" } Altered period of the circadian rhythm, by cosine fitting. A statistically significant deviation of the period from 24 hours, assessed by the nonoverlap of 24 hours by the 95% [confidence interval](../../glossary#confidence-interval) of the period assessed by nonlinear least squares |
| Excessive pulse pressure | The problem of too large a difference between [diastolic](../../glossary#diastolic-blood-pressure) and [systolic blood pressure](../../glossary#systolic-blood-pressure) (between when the heart contracts and relaxes, respectively) |
| Excessive pulse pressure product | The combined effect of [heart rate](../../glossary#heart-rate) and [pulse pressure](../../glossary#pulse-pressure), as either or both increase |
| Deficient heart rate variability (DHRV) | The problem of heart rate that does not vary enough, as indicated by the [standard deviation](../../glossary#standard-deviation) and when measured over a seven-day period |

MESOR-hypertension indicates a risk of stroke. The VVAs represent independent, additive risks of adverse cardiovascular events. Together, a patient with four of the conditions has a nearly 100% risk of stroke within six years. [^physiology]

The cosinor analysis produces a **Sphygmochron^&trade;^** &mdash; a report that provides an inferential statistical basis for diagnosising blood pressure disorders, by comparing the subject's blood pressure and heart rate profile with that of a clinically healthy peers.

[^cdc]: Centers for Disease Control and Prevention. "High Blood Pressure Symptoms and Causes". Website, reviewed 18 May 2021. [https://www.cdc.gov/bloodpressure/about.htm](https://www.cdc.gov/bloodpressure/about.htm){: target="_blank" }.

[^rhythmometry]: Cornelissen, Germaine. “Cosinor-based rhythmometry.” _Theoretical biology & medical modelling_ vol. 11 16. 11 Apr. 2014, doi:10.1186/1742-4682-11-16. [https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3991883/pdf/1742-4682-11-16.pdf](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3991883/pdf/1742-4682-11-16.pdf){: target="_blank" }.

[^physiology]: Franz Halberg, Deborah Powell, Kuniaki Otsuka, Yoshihiko Watanabe, Larry A. Beaty, Paul Rosch, Jerzy Czaplicki, Dewayne Hillman, Othild Schwartzkopff, and Germaine Cornelissen. "Diagnosing vascular variability anomalies, not only MESOR-hypertension". _American Journal of Physiology-Heart and Circulatory Physiology_ 2013 305:3, H279-H294. [https://journals.physiology.org/doi/full/10.1152/ajpheart.00212.2013](https://journals.physiology.org/doi/full/10.1152/ajpheart.00212.2013){: target="_blank" }.
