# Andrey Pautov

**Cybersecurity Researcher | AI-Powered Security Tooling | Malware Analysis | CTI | Offensive Security Research**

I build practical cybersecurity tools, malware-analysis workflows, threat intelligence research, and security testing utilities designed for analysts, defenders, researchers, and security engineers.

I focus on:
- AI-powered security automation
- Malware triage and static analysis
- Cyber Threat Intelligence (CTI)
- Offensive security research
- Detection-oriented defensive engineering

---

## Table of Contents

- [About Me](#about-me)
- [Featured Projects](#featured-projects)
- [Repository Portfolio](#repository-portfolio)
  - [AI-Powered Security](#ai-powered-security)
  - [Cyber Threat Intelligence](#cyber-threat-intelligence)
  - [Malware Analysis Tooling](#malware-analysis-tooling)
  - [Security Testing and Offensive Research](#security-testing-and-offensive-research)
  - [System, Networking, and Education Projects](#system-networking-and-education-projects)
- [Writing and Research](#writing-and-research)
- [Professional Links](#professional-links)
- [Current Focus](#current-focus)
- [Project Navigation](#project-navigation)
- [Philosophy](#philosophy)

---

## About Me

I am a cybersecurity researcher and builder focused on creating practical, research-backed tools and workflows that help security teams move faster from raw artifacts to actionable insight.

This GitHub profile includes:
- AI-assisted security tooling
- Malware-analysis utilities
- Static-analysis pipelines
- CTI research repositories
- Security testing tools
- Practical research and lab-oriented projects

I also publish technical cybersecurity articles and research on Medium:

**Medium:** [medium.com/@1200km](https://medium.com/@1200km)

---

## Featured Projects

### [StratusAI](https://github.com/anpa1200/stratus-ai)
AI-powered multi-cloud security scanner for AWS and GCP. Scans 9 AWS modules, 7 GCP modules, and 4 external modules; routes findings through Claude, GPT-4o, or Gemini for attack chain analysis and prioritized reports. Deploys to AWS ECS Fargate or GCP Cloud Run Job via a single interactive wizard.

> 📖 [Full engineering walkthrough on Medium](https://medium.com/@1200km/stratusai-i-built-an-ai-powered-cloud-security-scanner-for-aws-and-gcp-heres-everything-89c6702d3b84)

### [AuditAI](https://github.com/anpa1200/AuditAI)
AI-powered host vulnerability assessment and security auditing in a Dockerized workflow.

### [CTI](https://github.com/anpa1200/CTI)
Open-source cyber threat intelligence reports with evidence-labeled assessments, SOC-oriented guidance, and defensive research.

### [Static-malware-Analysis-Orchestrator](https://github.com/anpa1200/Static-malware-Analysis-Orchestrator)
One-command static malware analysis pipeline: triage, strings, PE imports, unpacking, and LLM-ready reporting.

### [Unpacker](https://github.com/anpa1200/Unpacker)
Modular malware packer detection and unpacking workflow for PE and ELF samples.

### [PE-Import-Analyzer](https://github.com/anpa1200/PE-Import-Analyzer)
PE import table analysis for malware triage and reverse-engineering support.

### [String-Analyzer](https://github.com/anpa1200/String-Analyzer)
String extraction and analysis for binaries to surface indicators, suspicious content, and analyst-relevant context.

---

## Repository Portfolio

## AI-Powered Security

### [StratusAI](https://github.com/anpa1200/stratus-ai)
AI-powered multi-cloud security scanner covering AWS (9 modules) and GCP (7 modules) plus external endpoint scanning. Uses Claude, GPT-4o, or Gemini to synthesize findings into attack chains and prioritized remediation. Deploys serverlessly to AWS ECS Fargate or GCP Cloud Run Job via a unified interactive wizard (`wizard.sh`).

Runs a full assessment in 2–4 minutes. Costs ~$0.01–$0.15 per scan depending on model. 125-test suite, zero live cloud calls in CI.

> 📖 **Article:** [StratusAI: I Built an AI-Powered Cloud Security Scanner for AWS and GCP — Here's Everything](https://medium.com/@1200km/stratusai-i-built-an-ai-powered-cloud-security-scanner-for-aws-and-gcp-heres-everything-89c6702d3b84)

### [AuditAI](https://github.com/anpa1200/AuditAI)
AI-powered host vulnerability assessment and security auditing platform designed to support practical security review workflows.

---

## Cyber Threat Intelligence

### [CTI](https://github.com/anpa1200/CTI)
Open-source CTI reports with evidence-labeled assessments, defensive guidance, and SOC-oriented research outputs.

---

## Malware Analysis Tooling

### [Static-malware-Analysis-Orchestrator](https://github.com/anpa1200/Static-malware-Analysis-Orchestrator)
One-command pipeline for static malware analysis: triage, strings, PE import analysis, unpacking, and LLM-ready reporting.

### [Unpacker](https://github.com/anpa1200/Unpacker)
Malware packer detection and unpacking framework supporting workflows such as detect → unpack → validate.

### [Basic-File-Information-Gathering-Script](https://github.com/anpa1200/Basic-File-Information-Gathering-Script)
File metadata and characteristic extraction tool for fast triage of suspicious or unknown files.

### [String-Analyzer](https://github.com/anpa1200/String-Analyzer)
Printable-string extraction and analysis utility for malware analysts, reverse engineers, and forensic investigators.

### [PE-Import-Analyzer](https://github.com/anpa1200/PE-Import-Analyzer)
Command-line utility for PE import table analysis with analyst-friendly explanations and flexible output.

### [Malware_analysis](https://github.com/anpa1200/Malware_analysis)
General malware analysis repository containing additional tooling and related experimentation.

---

## Security Testing and Offensive Research

### [Passwords](https://github.com/anpa1200/Passwords)
Security testing toolkit for generating personalized password wordlists, phone-based combinations, and encoded credential pairs for authorized assessments.

### [RTSP-brute-force-tool](https://github.com/anpa1200/RTSP-brute-force-tool)
Security testing utility for authorized RTSP authentication assessment and credential brute-force simulation.

### [vulnerable-cloud-lab](https://github.com/anpa1200/vulnerable-cloud-lab)
Terraform-based deployment of intentionally vulnerable GCP and AWS cloud environments for penetration testing training and security research.

---

## System, Networking, and Education Projects

### [SystemCheck](https://github.com/anpa1200/SystemCheck)
System configuration inspection tool for quick visibility into Linux host health and configuration state.

### [Networking](https://github.com/anpa1200/Networking)
Networking-focused Python repository for related experiments and utilities.

### [lpi](https://github.com/anpa1200/lpi)
LPI 010-160 exam simulator and training project built with a shared question-bank approach.

---

## Writing and Research

I regularly publish technical articles, walkthroughs, and research on Medium, including work on:
- AI-driven cybersecurity
- Malware analysis
- Static-analysis tooling
- CTI research
- Security automation
- Offensive-security workflows

**Recent articles:**

- [StratusAI: I Built an AI-Powered Cloud Security Scanner for AWS and GCP — Here's Everything](https://medium.com/@1200km/stratusai-i-built-an-ai-powered-cloud-security-scanner-for-aws-and-gcp-heres-everything-89c6702d3b84) — full engineering walkthrough: AWS + GCP scanner modules, multi-LLM routing, two-stage AI analysis, Terraform deployment on both clouds, 125-test suite

**All articles:**
[https://medium.com/@1200km](https://medium.com/@1200km)

---

## Professional Links

- **Medium:** [medium.com/@1200km](https://medium.com/@1200km)
- **LinkedIn:** [linkedin.com/in/andrey-pautov-44718441](https://www.linkedin.com/in/andrey-pautov-44718441)

---

## Current Focus

I am currently focused on:
- Building practical AI-powered cybersecurity tools
- Expanding malware-analysis automation workflows
- Publishing high-quality CTI research
- Improving analyst productivity through structured tooling and automation
- Connecting offensive research with real defensive value

---

## Project Navigation

If you are visiting this profile for the first time, start here:

1. [StratusAI](https://github.com/anpa1200/stratus-ai) — multi-cloud AI security scanner (AWS + GCP)
2. [AuditAI](https://github.com/anpa1200/AuditAI)
3. [CTI](https://github.com/anpa1200/CTI)
4. [Static-malware-Analysis-Orchestrator](https://github.com/anpa1200/Static-malware-Analysis-Orchestrator)
5. [Unpacker](https://github.com/anpa1200/Unpacker)
6. [PE-Import-Analyzer](https://github.com/anpa1200/PE-Import-Analyzer)
7. [String-Analyzer](https://github.com/anpa1200/String-Analyzer)
8. [Basic-File-Information-Gathering-Script](https://github.com/anpa1200/Basic-File-Information-Gathering-Script)
9. [Passwords](https://github.com/anpa1200/Passwords)
10. [RTSP-brute-force-tool](https://github.com/anpa1200/RTSP-brute-force-tool)
11. [vulnerable-cloud-lab](https://github.com/anpa1200/vulnerable-cloud-lab)
12. [SystemCheck](https://github.com/anpa1200/SystemCheck)
13. [Malware_analysis](https://github.com/anpa1200/Malware_analysis)
14. [lpi](https://github.com/anpa1200/lpi)
15. [Networking](https://github.com/anpa1200/Networking)

---

## Philosophy

I believe security tooling should be:
- Practical
- Transparent
- Research-driven
- Analyst-friendly
- Easy to integrate into real workflows

My goal is to build tools and research that are not only technically strong, but operationally useful.

---

# Cybersecurity Research • Practical Tooling • Intelligence-Driven Engineering
