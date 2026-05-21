# Andrey Pautov

[Main portfolio hub: anpa1200.github.io](https://anpa1200.github.io/) — start here for my CTI reports, Docusaurus sites, tools, labs, and Medium research.

Practical CTI engineer with an offensive-security and malware-analysis background. I build tooling that turns reports into hunts, IOCs into pivots, malware samples into ATT&CK-mapped detections, and CVEs into prioritized work.

| CTI as engineering | Operator-grade tradecraft | Offensive and malware lab depth |
|---|---|---|
| Reports to detections. IOCs to pivots. CVEs to work queues. | Evidence labels, attribution discipline, ATT&CK mapping, hunting hypotheses. | Labs, malware tooling, cloud testing, AD/Kubernetes/GCP workflows. |

![Medium followers](https://img.shields.io/badge/Medium%20followers-1.3K-black)
![Python](https://img.shields.io/badge/Python-primary-blue)
![LinkedIn](https://img.shields.io/badge/LinkedIn-andrey--pautov-blue)
![Twitter](https://img.shields.io/badge/X-@AndreyPa5-black)

I came to CTI through offensive security and malware analysis, which changes how I write intelligence. I care less about polished reports and more about what a defender can do next: hunt the behavior, enrich the IOC, map the technique, validate the claim, prioritize the vulnerable asset, and hand the SOC something testable.

## Start Here

| Project | Defender value | Links |
|---|---|---|
| **AIDebug** | Explains malware functions and turns reverse-engineering output into ATT&CK mappings, YARA, IOC lists, and reports. | [Repo](https://github.com/anpa1200/AIDebug) · [Article](https://medium.com/@1200km/ai-powered-malware-debugger-that-explains-every-function-it-sees-2a28ef75df8a) |
| **Android-Malware-Analysis** | Static APK triage with YARA, semantic scoring, VirusTotal context, ATT&CK output, and Frida hooks. | [Repo](https://github.com/anpa1200/Android-Malware-Analysis) · [Article](https://medium.com/@1200km/android-apk-analysis-tool-ai-powered-static-malware-analysis-in-your-terminal-4beb239dad12) |
| **cvss_4.0** | Converts CVEs into CVSS-BTE prioritization using NVD, CISA KEV, EPSS, and asset profiles. | [Repo](https://github.com/anpa1200/cvss_4.0) · [Article](https://medium.com/bugbountywriteup/cvss-v4-0-the-practical-field-guide-for-vulnerability-management-5b5a59728456) · [Guide](https://anpa1200.github.io/cvss/) |
| **CTI** | Evidence-labeled threat reports with defensive guidance and reusable report templates. | [Repo](https://github.com/anpa1200/CTI) · [Israel CTI site](https://anpa1200.github.io/israel-government-threat-actors-cti/) |
| **stratus-ai** | Multi-cloud AI security scanner for AWS, GCP, and external exposure with attack-chain synthesis. | [Repo](https://github.com/anpa1200/stratus-ai) · [Article](https://medium.com/@1200km/stratusai-i-built-an-ai-powered-cloud-security-scanner-for-aws-and-gcp-heres-everything-89c6702d3b84) |
| **autoWF** | IOC-to-infrastructure pivoting tool for CTI analysts. | [Repo](https://github.com/anpa1200/autoWF) · [Article](https://infosecwriteups.com/infrastructure-pivoting-how-cti-analysts-expand-from-a-single-ioc-to-a-full-attacker-network) |

## CTI Deliverables

### Threat Reports

- [CTI](https://github.com/anpa1200/CTI) — citation-linked reports on Handala / Void Manticore, Sandworm / APT44, and MuddyWater / Seedworm with evidence labels: Observed, Reported, Assessed, Claimed.
- [Israel Government Threat Actors CTI](https://anpa1200.github.io/israel-government-threat-actors-cti/) — defensive CTI knowledge base for Israeli government, public-sector, municipal, critical-infrastructure, and supplier exposure.

### Tradecraft And Methodology

- [CTI Analyst Field Manual](https://anpa1200.github.io/cti-analyst-field-manual/) — analytic judgment, hunting hypotheses, source handling, confidence language, and detection-ready outputs.
- [Attribution Methodology](https://medium.com/@1200km/attribution-methodology-how-to-build-defend-and-challenge-a-threat-actor-attribution-071066437ced)
- [Infrastructure Pivoting](https://infosecwriteups.com/infrastructure-pivoting-how-cti-analysts-expand-from-a-single-ioc-to-a-full-attacker-network)
- [ATT&CK as a Working Tool](https://medium.com/@1200km/att-ck-as-a-working-tool-theory-and-hands-on-practical-usage-d63835c9f101)
- [Manual CTI vs. AI-Assisted CTI](https://medium.com/@1200km/manual-cti-vs-ai-assisted-cti-a-step-by-step-clock-comparison-ee08325203fc)
- [CTI Kill Chain](https://medium.com/@1200km/cti-kill-chain-an-analyst-guide-with-real-world-evidence-c3bef6fd2979)

### CTI Program Design

- [Customer-Driven AI CTI Project](https://anpa1200.github.io/customer-driven-ai-cti-project/) — gate-controlled CTI-to-detection methodology.
- [Customer-Driven AI CTI Project Template](https://anpa1200.github.io/customer-driven-ai-cti-project-template/) — reusable project template from intelligence requirements to hunts, detections, and delivery.

### Detection And Hunting

- [From Threat Intelligence to Detection](https://medium.com/@1200km)
- [Threat Hunting with the Pyramid of Pain](https://medium.com/@1200km)
- [Single-Event Detection Rules](https://medium.com/@1200km)
- [Correlation-Based Detection Rules](https://medium.com/@1200km)
- [Endpoint Threat Hunting](https://medium.com/@1200km)
- [Protocol-Level Network Threat Hunting](https://medium.com/@1200km)
- [The Invisible Pipeline: Defending CI/CD](https://medium.com/@1200km)

## Malware-Analysis Stack

| Repo | What it produces |
|---|---|
| [AIDebug](https://github.com/anpa1200/AIDebug) | Function explanations, CFGs, YARA, JSON, HTML, ATT&CK mappings, IOC lists. |
| [Android-Malware-Analysis](https://github.com/anpa1200/Android-Malware-Analysis) | APK static triage, YARA hits, MITRE output, VirusTotal context, Frida hooks. |
| [Static-malware-Analysis-Orchestrator](https://github.com/anpa1200/Static-malware-Analysis-Orchestrator) | One-command triage, strings, PE imports, unpacking, LLM-ready reports. |
| [Unpacker](https://github.com/anpa1200/Unpacker) | Packer detection and unpacking workflow for PE and ELF. |
| [PE-Import-Analyzer](https://github.com/anpa1200/PE-Import-Analyzer) | DLL/API import explanations and analyst-friendly output. |
| [String-Analyzer](https://github.com/anpa1200/String-Analyzer) | Printable strings with suspicious-content context. |
| [Basic-File-Information-Gathering-Script](https://github.com/anpa1200/Basic-File-Information-Gathering-Script) | File metadata triage for unknown samples. |

## Vulnerability Management

- [cvss_4.0](https://github.com/anpa1200/cvss_4.0) — CVSS v4.0 BTE enrichment with NVD, CISA KEV, EPSS, and six asset profiles.
- [CVSS v4.0 Field Guide](https://anpa1200.github.io/cvss/) — practitioner guide for vulnerability management teams.
- [Medium article](https://medium.com/bugbountywriteup/cvss-v4-0-the-practical-field-guide-for-vulnerability-management-5b5a59728456) — practical CVSS-BTE explanation and examples.

## Offensive Lab And Research

This is not the headline. It is the reason the CTI is grounded.

- [HexStrike-AI Guide](https://anpa1200.github.io/Hexstrike-AI-guide/) — AI-driven pentesting and security-research field guide.
- [vulnerable-cloud-lab](https://github.com/anpa1200/vulnerable-cloud-lab) — Terraform-deployed vulnerable AWS and GCP labs.
- [Passwords](https://github.com/anpa1200/Passwords) — personalized wordlists and credential-pair generation for authorized assessments.
- [RTSP-brute-force-tool](https://github.com/anpa1200/RTSP-brute-force-tool) — authorized RTSP credential testing.

## Writing

- [Medium profile](https://medium.com/@1200km)
- [Navigate My Blog](https://medium.com/@1200km/navigate-my-blog-all-articles-by-topic-ffd800ef5480)
- [Blog Navigator](https://anpa1200.github.io/medium-blog-navigation/)

Curated CTI and detection reads:

1. [CTI Kill Chain](https://medium.com/@1200km/cti-kill-chain-an-analyst-guide-with-real-world-evidence-c3bef6fd2979)
2. [Infrastructure Pivoting](https://infosecwriteups.com/infrastructure-pivoting-how-cti-analysts-expand-from-a-single-ioc-to-a-full-attacker-network)
3. [Attribution Methodology](https://medium.com/@1200km/attribution-methodology-how-to-build-defend-and-challenge-a-threat-actor-attribution-071066437ced)
4. [ATT&CK as a Working Tool](https://medium.com/@1200km/att-ck-as-a-working-tool-theory-and-hands-on-practical-usage-d63835c9f101)
5. [Manual CTI vs. AI-Assisted CTI](https://medium.com/@1200km/manual-cti-vs-ai-assisted-cti-a-step-by-step-clock-comparison-ee08325203fc)
6. [AI in Offensive Operations](https://medium.com/@1200km/ai-in-offensive-operations-how-threat-actors-use-artificial-intelligence-4eaeeaf029a9)

## Contact

- Site: https://anpa1200.github.io
- Medium: https://medium.com/@1200km
- LinkedIn: https://www.linkedin.com/in/andrey-pautov/
- Twitter/X: https://x.com/AndreyPa5
- PayPal: [user: confirm donation URL]

I write CTI like the operator is still moving and the SOC has to act today.
