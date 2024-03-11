---
title: Requirements
---
![Under Construction](../images/underconstruction.svg)

!!! bug
    The diagrams in this article are out-of-date but included as placeholders to organize the article.

## Actors

![Actors](../images/requirements-actors-model.png)

### Actor profile table

| Actor | Profile: Background and Skills |
| ----- | ------------------------------ |
| patient | May be sick or may want to know health status.<br><br>May vary between “Does not want to be bothered” and wanting biofeedback to modify behavior |
| specialist | a physician<br><br>Called for help by primary care physician |
| clinician | Deals directly with patients<br><br>May access medical records<br><br>May be primary care physician, secondary care physician (specialist), physician’s assistant, registered nurse, nursing assistant, certified medical assistant |
| physician | a clinician<br><br>makes clinical decisions<br><br>diagnoses patient |
| nurse | a clinician<br><br>Deals directly with device<br><br>Manages interaction between device and patient<br><br>Responsible for data transfer<br><br>Creates report for physician<br><br>Creates report for patient |

## Context

![Context Diagram](../images/context-diagram.png)

## Use cases

## Required attributes

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
