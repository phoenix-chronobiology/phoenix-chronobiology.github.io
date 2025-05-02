![Under Construction](../../images/underconstruction.svg)

!!! bug
    The following is a hodge-podge of ideas that must be:
    
    1. Reduced to what the Phoenix Chronobiology Projects want to say in this revision, and
    1. Rewritten into plain language.

## European CRA

!!! info "Source"
    The European Cyber Resilience Act [^cra]

The product shall:

1. Be delivered with a secure by default configuration, including the possibility to reset the product to its original state.
1. Ensure protection from unauthorised access by appropriate control mechanisms, including but not limited to authentication, identity or access management systems.
1. Protect the confidentiality of stored, transmitted or otherwise processed data, personal or other, such as by encrypting relevant data at rest or in transit by state of the art mechanisms.
1. Protect the integrity of stored, transmitted or otherwise processed data, personal or other, commands, programs and configuration against any manipulation or modification not authorised by the user, as well as report on corruptions.
1. Process only data, personal or other, that are adequate, relevant and limited to what is necessary in relation to the intended use of the product (‘minimisation of data’).
1. Protect the availability of essential functions, including the resilience against and mitigation of denial-of-service attacks.
1. Minimize its own negative impact on the availability of services provided by other devices or networks.
1. Be designed, developed and produced to limit attack surfaces, including external interfaces.
1. Be designed, developed and produced to reduce the impact of an incident using appropriate exploitation mitigation mechanisms and techniques.
1. Provide security related information by recording and/or monitoring relevant internal activity, including the access to or modification of data, services or functions.
1. Ensure that vulnerabilities can be addressed through security updates, including, where applicable, through automatic updates and the notification of available updates to users.

## OWASP

!!! info "Source"
    OWASP Developer Guide [^owasp]

### System configuration

* Restrict applications, processes and service accounts to the least privileges possible
* If the application must run with elevated privileges, raise privileges as late as possible, and drop as soon as possible
* Remove all unnecessary functionality and files
* Remove test code or any functionality not intended for production, prior to deployment
* The security configuration store for the application should be available in human readable form to support auditing
* Isolate development environments from production and provide access only to authorized development and test groups
* Implement a software change control system to manage and record changes to the code both in development and production

### Cryptographic practices

* Use peer reviewed and open solution cryptographic modules
* All cryptographic functions used to protect secrets from the application user must be implemented on a trusted system
* Cryptographic modules must fail securely
* Ensure all random elements such as numbers, file names, UUID and strings are generated using the cryptographic module approved random number generator
* Cryptographic modules used by the application are compliant to FIPS 140-2 or an equivalent standard
* Establish and utilize a policy and process for how cryptographic keys will be managed
* Ensure that any secret key is protected from unauthorized access
* Store keys in a proper secrets vault as described below
* Use independent keys when multiple keys are required
* Build support for changing algorithms and keys when needed
* Build application features to handle a key rotation

### File management

* Do not pass user supplied data directly to any dynamic include function
* Require authentication before allowing a file to be uploaded
* Limit the type of files that can be uploaded to only those types that are needed for business purposes
* Validate uploaded files are the expected type by checking file headers rather than by file extension
* Do not save files in the same web context as the application
* Prevent or restrict the uploading of any file that may be interpreted by the web server.
* Turn off execution privileges on file upload directories
* When referencing existing files, use an allow-list of allowed file names and types
* Do not pass user supplied data into a dynamic redirect
* Do not pass directory or file paths, use index values mapped to pre-defined list of paths
* Never send the absolute file path to the client
* Ensure application files and resources are read-only
* Scan user uploaded files for viruses and malware

## UK General Data Protection Regulation (GDPR)

!!! info "Source"
    United Kindom's Information Commissioner's Office [^gdpr]

* [Lawfulness, fairness and transparency](#lawfulness-fairness-and-transparency)
* [Purpose limitation](#purpose-limitation)
* [Data minimization](#data-minimization)
* [Accuracy](#accuracy)
* [Storage limitation](#storage-limitation)
* [Integrity and confidentiality (security)](#integrity-and-confidentiality-security)
* [Accountability](#accountability)

### Lawfulness, fairness and transparency

**Lawfulness**

- [x] We have identified an appropriate lawful basis (or bases) for our processing.
- [x] If we are processing special category data or criminal offence data, we have identified a condition for processing this type of data.
- [x] We don’t do anything generally unlawful with personal data.

**Fairness**

- [x] We have considered how the processing may affect the individuals concerned and can justify any adverse impact.
- [x] We only handle people’s data in ways they would reasonably expect, or we can explain why any unexpected processing is justified.
- [x] We do not deceive or mislead people when we collect their personal data.

**Transparency**

- [x] We are open and honest, and comply with the transparency obligations of the right to be informed.

### Purpose limitation

- [x] We have clearly identified our purpose or purposes for processing.
- [x] We have documented those purposes.
- [x] We include details of our purposes in our privacy information for individuals.
- [x] We regularly review our processing and, where necessary, update our documentation and our privacy information for individuals.
- [x] If we plan to use personal data for a new purpose other than a legal obligation or function set out in law, we check that this is compatible with our original purpose or we get specific consent for the new purpose.

### Data minimization

- [x] We only collect personal data we actually need for our specified purposes.
- [x] We have sufficient personal data to properly fulfil those purposes.
- [x] We periodically review the data we hold, and delete anything we don’t need.

### Accuracy

- [x] We ensure the accuracy of any personal data we create.
- [x] We have appropriate processes in place to check the accuracy of the data we collect, and we record the source of that data.
- [x] We have a process in place to identify when we need to keep the data updated to properly fulfil our purpose, and we update it as necessary.
- [x] If we need to keep a record of a mistake, we clearly identify it as a mistake.
- [x] Our records clearly identify any matters of opinion, and where appropriate whose opinion it is and any relevant changes to the underlying facts.
- [x] We comply with the individual’s right to rectification and carefully consider any challenges to the accuracy of the personal data.
- [x] As a matter of good practice, we keep a note of any challenges to the accuracy of the personal data.

### Storage limitation

- [x] We know what personal data we hold and why we need it.
- [x] We carefully consider and can justify how long we keep personal data.
- [x] We have a policy with standard retention periods where possible, in line with documentation obligations.
- [x] We regularly review our information and erase or anonymise personal data when we no longer need it.
- [x] We have appropriate processes in place to comply with individuals’ requests for erasure under ‘the right to be forgotten’.
- [x] We clearly identify any personal data that we need to keep for public interest archiving, scientific or historical research, or statistical purposes.

### Integrity and confidentiality (security)

- [x] We process personal data in a manner that ensures its appropriate security, including protection against unauthorised or unlawful processing and against accidental loss, destruction or damage, using appropriate technical or organisational measures

### Accountability

We put in place appropriate technical and organizational measures, such as:

- [x] adopting and implementing data protection policies (where proportionate);
- [x] taking a 'data protection by design and default' approach &mdash; putting appropriate data protection measures in place throughout the entire lifecycle of our processing operations;
- [x] putting written contracts in place with organisations that process personal data on our behalf;
- [x] maintaining documentation of our processing activities;
- [x] implementing appropriate security measures;
- [x] recording and, where necessary, reporting personal data breaches;
- [x] carrying out data protection impact assessments for uses of personal data that are likely to result in high risk to individuals’ interests;
- [x] appointing a data protection officer (where necessary); and
- [x] adhering to relevant codes of conduct and signing up to certification schemes (where possible).

## Other

Keep secrets out of public platforms, such as GitHub. Use a purpose-built secrets management platform.

De-identify data.

Apply privileged access management[^pam]


[^cra]: "Annex 1: Essential Cybersecurity Requirements", **The European Cyber Resilience Act**. Proposal 14 September 2022. [https://www.european-cyber-resilience-act.com/Cyber_Resilience_Act_Annex_1.html](https://www.european-cyber-resilience-act.com/Cyber_Resilience_Act_Annex_1.html){: target="_blank" }.

[^owasp]: The OWASP^&reg;^ Foundation. "Define Security Requirements Checklist", **OWASP Developer Guide**. Draft version 4.x, accessed 8 March 2024. [https://owasp.org/www-project-developer-guide/draft/design/web_app_checklist/define_security_requirements/](https://owasp.org/www-project-developer-guide/draft/design/web_app_checklist/define_security_requirements/){: target="_blank" }

[^gdpr]: Information Commissioner's Office, "UK GDPR guidance and resources". Website, accessed 8 March 2024. [https://ico.org.uk/for-organisations/uk-gdpr-guidance-and-resources/](https://ico.org.uk/for-organisations/uk-gdpr-guidance-and-resources/){: target="_blank" }.

[^pam]: Fortra, LLC. "Privileged Access Management". Website, accessed 7 March 2024. [https://www.coresecurity.com/privileged-access-management](https://www.coresecurity.com/privileged-access-management){: target="_blank" }.
