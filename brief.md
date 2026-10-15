Version: NAFATH-V4
Track: Software



## Overview
Nowadays,many services needs  internet and software System work properly. These System may face many security problems that may affect operations. Software passwords need to be secure, while AI System must be checked to protect from attackers cannot change it easily. Mobile applications need to keep user information safe from attackers. Networking,if it's false route then announcements can send internet traffic to different location.  Cybersercurity helps to find weaknesses before cause problem and fix it directly. It is important to understand and to know which software components are used in application because may contain security issues.  This six areas are connected together, and a weaknesses in one of them it make problem security for whole service. For the software track, an important question is how application setting and secrets can be stored safely from attackers.


## Software
The Twelve-Factor App methodology recommends storing deployment-specific configuration in environment variables rather than hard-coding it in application code. This includes database credentials, service keys, and settings that change between environments. Separating configuration from code makes applications easier to deploy and maintain. It also reduces the risk of exposing secrets through public repositories or shared source code. Sensitive credentials should be managed securely and access should be restricted.

Resource: The Twelve-Factor App - Config - https://12factor.net/config
## AI
Adversarial attacks target machine learning systems in different ways. Evasion attacks manipulate inputs during use to cause incorrect predictions, while poisoning attacks corrupt training data or the learning process to influence model behavior. Privacy attacks may reveal information about training data, and misuse attacks can exploit generative AI capabilities. Organizations should assess these risks throughout the AI lifecycle and apply suitable testing, monitoring, and mitigation measures.

Resource: NIST AI 100-2e2025 - Adversarial Machine Learning: A Taxonomy and Terminology of Attacks and Mitigations - https://csrc.nist.gov/pubs/ai/100/2/e2025/final
## Mobile
The OWASP Mobile Application Security Verification Standard (MASVS) defines security controls for mobile applications. It covers areas such as data storage, cryptography, authentication, network communication, platform interaction, code quality, resilience, and privacy. Developers and security testers use these controls to guide assessments and identify weaknesses. The Mobile Application Security Testing Guide (MASTG) provides practical testing guidance to help verify whether an application meets the relevant controls.

Resource: OWASP MASVS - https://mas.owasp.org/MASVS/

## Networking
BGP route hijacking occurs when an autonomous system announces incorrect or unauthorized IP prefixes, potentially causing internet traffic to follow an unintended path. Resource Public Key Infrastructure (RPKI) supports Route Origin Validation by checking whether a route announcement is authorized by the holder of the IP address resources. However, RPKI origin validation does not verify the entire route path or prevent every attack, including certain attacks involving a legitimate origin AS.

Resource: RFC 6811 - BGP Prefix Origin Validation - https://www.rfc-editor.org/rfc/rfc6811

## Cybersecurity
Log4Shell (CVE-2021-44228) was a critical remote code execution vulnerability in Apache Log4j 2, a widely used Java logging library. It could allow attackers to execute code on vulnerable systems when affected logging functionality processed malicious input. Its severity came from its potential for remote exploitation and the widespread use of the library. Organizations were advised to identify affected assets, upgrade to patched versions, apply temporary mitigations when necessary, and verify remediation.

Resource: CISA - Mitigating Log4Shell and Other Log4j-Related Vulnerabilities - https://www.cisa.gov/news-events/cybersecurity-advisories/aa21-356a

## Data
A Software Bill of Materials (SBOM) is a structured inventory of the components included in a software product. It helps organizations identify dependencies and investigate whether vulnerable components affect their systems. An SBOM should include the supplier name, component name, component version, other unique identifiers, dependency relationships, the SBOM author, and the creation timestamp. Organizations can use this information to improve supply-chain visibility and respond more effectively to newly discovered vulnerabilities.

Resource: CISA - Minimum Elements for a Software Bill of Materials (SBOM) - https://www.cisa.gov/resources-tools/resources/2025-minimum-elements-software-bill-materials-sbom

## Misconception in My Track
A common misconception is that storing passwords and API keys in a private code repository makes them safe. In reality, repository access can expand, code can be shared accidentally, and credentials may remain in version history even after removal. The Twelve-Factor App methodology recommends separating deployment configuration from code and storing it in environment variables. Secrets should also be managed with appropriate access controls. This approach reduces accidental exposure, although environment variables alone do not guarantee complete secret protection.



## Open Question
How can an organization securely manage and rotate application secrets across development, testing, and production environments without interrupting critical services?
