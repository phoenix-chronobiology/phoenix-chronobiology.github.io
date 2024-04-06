![Under Construction](../../images/underconstruction.svg)

## Overview

**{{ config.site_name }}** underpin an emerging healthcare program that uses [chronobiologic](../glossary#chronobiology) techniques to prevent [strokes](../glossary#stroke) and other effects of cardiac disease.

The system uses blood pressure measurements taken approximately every 30 minutes, day and night, in ambulatory fashion. Ideally, seven days of data are available. This data is analyzed with **[cosinor](cosinor.md)** and **[cumulative-sum](cusum.md)** algorithms.

The results of an analysis is available directly to the patient, and when appropriate, to the patient’s healthcare provider. Analysis solutions are automated and easy to use.

The associated databases contain physiological data about large numbers of individuals over time, as well as physiological and psychological data on populations. The databases are available to chronophysiologists who create the reference sets needed by the analysis techniques, as well as to chronobiology researchers.

The solution is global in scope. Its capability is widely distributed and fronted by multi-linguage websites.

The solution employs a zero-trust security model, with defense in depth.

The solution treats privacy as paramount, giving the patient control over who has access to the patient's data.

The public-facing websites contain:

* The analysis tools
* Libraries of reference materials for different audiences (physician, general public, student)
* Lists of commercially-available ambulatory blood pressure monitors

!!! question "Proposal for and Concern About Social Networks"
    The solution previously envisioned connections to popular social networking websites as means to motivate members of the general public to use the system and disseminate information that they find to be trustworthy and popular.  The social networking mechanisms would be designed to allow the general public to collaborate and discover individualized treatments that are more effective than those that have passed one-size-fits-all style clinical trials, and would allow comparative analyses of individual and population based physiological and psychological data, starting with but not limited to their own blood pressure.

    Links to social networks are problematic because they would open vulnerabilities to privacy and security.

## Context

!!! bug
    The diagrams in this article are out-of-date but are included as placeholders to organize the article.

![Context Diagram](../../images/context-diagram.png)

Inputs: blood pressure measurements taken approximately every 30 minutes, day and night, in ambulatory fashion.


## Actors

![Actors](../../images/requirements-actors-model.png)

### Actor profile table

| Actor | Profile: Background and Skills |
| ----- | ------------------------------ |
| patient | May be sick or may want to know health status.<br><br>May vary between “Does not want to be bothered” and wanting biofeedback to modify behavior |
| specialist | a physician<br><br>Called for help by primary care physician |
| clinician | Deals directly with patients<br><br>May access medical records<br><br>May be primary care physician, secondary care physician (specialist), physician’s assistant, registered nurse, nursing assistant, certified medical assistant |
| physician | a clinician<br><br>makes clinical decisions<br><br>diagnoses patient |
| nurse | a clinician<br><br>Deals directly with device<br><br>Manages interaction between device and patient<br><br>Responsible for data transfer<br><br>Creates report for physician<br><br>Creates report for patient |


## Use cases


The mechanism for detecting high risk of stroke and guiding treatment requires “continuous” blood pressure measurements; blood pressure measurements taken approximately every 30 minutes, day and night, in ambulatory fashion, are analyzed via cosinor and cumulative sum.

The analysis can be automated on, and dispensed from, a worldwide multi-lingual website.  The results of the analysis are to be made available to the patient directly, and when appropriate, to the patient’s healthcare provider.  The associated databases are useful to chronobiology researchers, as they contain physiological data on large numbers of individuals over time as well as physiological and psychological data on populations.

The chronobiological analyses to be used in the first version of the website are Sphygmochron™ reports (circadian rhythm analysis based on cosinor mathematics) and CUSUM reports (based on cumulative sum mathematics derived from the manufacturing “quality control” arena).  The Sphygmochron detects six Vascular Variability Disorders (VVDs, persistent incorrect circadian rhythm characteristics in blood pressure or heart rate) that act as indicators of risk of stroke.  VVDs are mathematically defined as anomalies in the circadian phase, amplitude, and MESOR (a time-adjusted average) of BP and HR time series, when compared to healthy peers of the same gender and age group.  One VVD is a more precise definition of hypertension than that defined by the WHO, and others VVDs represent independent, additive indicators of stroke risk; an individual with MESOR hypertension, circadian hyper-amplitude tension, excessive pulse pressure, and deficient heart rate variability has a nearly 100% risk of stroke within six years.

The CUSUM detects the time at which changes in a metric such as SBP MESOR became statistically significant.  The Halberg Chronobiology Center developed a “self-starting CUSUM” that eliminates the need to specify a “target value” to be met.  

The website will provide the reports and data access mechanisms that meet appropriate security and privacy constraints.  Standard search and relational-database query capability will be provided.  The public-facing website will contain the analysis tools, libraries of reference materials for different audiences (physician, general public, student), lists of commercially-available cABPMs, and connections to popular social networking websites to motivate members of the general public to use the system and disseminate information that they find to be trustworthy and popular.  The social networking mechanisms are designed to allow the general public to collaborate and discover individualized treatments that are more effective than those that have passed one-size-fits-all style clinical trials, and will allow comparative analyses of individual and population based physiological and psychological data, starting with but not limited to their own blood pressure.

## Required attributes

!!! bug
    Reconcile the following with [Design goals](design-goals.md) and [Quality goals](quality-goals.md).

Inexpensive
: Free and open source software [^foss]

Highly decomposed
: Each component quickly engineered by very small team (usually one person)

Extensible &mdash; highly recomposable
: Multiple actors, vaguely organized
: Evolving user classes, usage scenarios, environments
: Highly re-usable components

Scalable
: Ready to cope with volume increases due to:

    - Wearers
    - Acquired data
    - Analysis requests

Secure
: The design incorporates:

    * Threat modeling [^threat]
    * Principle of least privilege [^polp]
    * Defense in depth &mdash; zero trust [^zero]
    * Secure defaults
    * Person identity management

Maintains privacy of data subject
: 1. Wearer owns measurements of the wearer's body
  1. Caregivers are custodians
  1. System operators are custodians
  1. Control belongs to the user

[^foss]: Wikipedia. "Free and open-source software". Website, accessed 8 March 2024. [https://en.wikipedia.org/wiki/Free_and_open-source_software](https://en.wikipedia.org/wiki/Free_and_open-source_software){: target="_blank" }.

[^threat]: Wikipedia. "Threat model". Website, accessed 8 March 2024. [https://en.wikipedia.org/wiki/Threat_model](https://en.wikipedia.org/wiki/Threat_model){: target="_blank" }.

[^polp]: Wikipedia. "Priciple of Least Privelege". Website, accessed 8 March 2024. [https://en.wikipedia.org/wiki/Principle_of_least_privilege](https://en.wikipedia.org/wiki/Principle_of_least_privilege){: target="_blank" }.

[^zero]: Wikipedia. "Zero Trust Security Model". Website, accessed 8 March 2024. [https://en.wikipedia.org/wiki/Zero_trust_security_model](https://en.wikipedia.org/wiki/Zero_trust_security_model){: target="_blank" }.
