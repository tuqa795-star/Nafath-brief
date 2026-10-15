Version: NAFATH-V4
Track: Software



## Overview
Nowadays,many services needs  internet and software System work properly. These System may face many security problems that may affect operations. Software passwords need to be secure, while AI System must be checked to protect from attackers cannot change it easily. Mobile applications need to keep user information safe from attackers. Networking,if it's false route then announcements can send internet traffic to different location.  Cybersercurity helps to find weaknesses before cause problem and fix it directly. It is important to understand and to know which software components are used in application because may contain security issues.  This six areas are connected together, and a weaknesses in one of them it make problem security for whole service. For the software track, an important question is how application setting and secrets can be stored safely from attackers.


## Software
Applications use different settings during deployment,testing and production. The twelve Factor Application methodology recommends keeping application settings separate from the code. It will be exposed the password,API keys when files are shared , if it is written directly in the code .the devloper should build secure methods to protected from attackers and control who can access them.
Resource: The Twelve-Factor App - Config - https://12factor.net/config

## AI
AI system can be attached in different ways . In an evasion attack, someone changes the input to make AI give wrong answer or result. In data poisoning attack, someone used to train the AI by changes the data ,which can affect what AI learns. And some attackers try to find private information in training data .So testing AI system can help to protect the data and reduce these risks.
Resource: NIST AI 100-2e2025 - Adversarial Machine Learning: A Taxonomy and Terminology of Attacks and Mitigations - https://csrc.nist.gov/pubs/ai/100/2/e2025/final

## Mobile
Mobile applications may store sensitive information, it need to be secure from attackers. The OWASP Mobile application security verification Standard MASVS provides security requirements. These include protecting stored data , secure communication over  the internet and checking user identities . It helps identify weaknesses.
Resource: OWASP MASVS - https://mas.owasp.org/MASVS/


## Networking
BGP it helps network send information where internet traffic should go.The trouble starts with route hijacking when a network announces routes it has no right to. Traffic can end up with wrong place or cause a service to stop working . PRKI helps check whether allowed to announced a certine block of IP addresses.  It can't stop every kind of routing attack,and it can't verify the whole path your traffic takes.
Resource: RFC 6811 - BGP Prefix Origin Validation - https://www.rfc-editor.org/rfc/rfc6811

## Cybersecurity
Log4Shell (CVE-2021-44228) was a serious flaw in Apache Log4j 2,Log4Shell a java tool that saves records of what aprogram dose. Attackers could trick it into running their own harmful code in computer. This was a huge problem because so many programs used Log4j. Companies had to find every place they used it, inststal the fixed version, and then test that the problem was really gone.
Resource: CISA - Mitigating Log4Shell and Other Log4j-Related Vulnerabilities - https://www.cisa.gov/news-events/cybersecurity-advisories/aa21-356a

## Data
A software Bill of Material (SBOM) is a list of all the parts that make up a piece of software, like the ingredients on a food label. It shows each parts name , version,and who made it , and how the parts are linked. If a security problem is found in one part, a company can check the list to see if it 8s software uses that part . If the list kept up to date, developer can quickly find what is affected and decide what to fix or replace.
Resource: CISA - Minimum Elements for a Software Bill of Materials (SBOM) - https://www.cisa.gov/resources-tools/resources/2025-minimum-elements-software-bill-materials-sbom

## Misconception in My Track
Many people think a private repository is enough to keep passwords and API keys safe. It is not. Someone with access can share the code by mistake, or the wrong person can break into an account. Also,a secret you delet can still be found in the repositorys history.  Story secrets in a separate, protected place, let only the write people use them, and replace any key that was exposed . A private repo protects your code, but it dose not protect every secret.
Source heading: The Twelve-Factor App, Config https://12factor.net/config

## Open Question
How can teams safely change passwords and API keys in development, testing, and production without stopping important services?
