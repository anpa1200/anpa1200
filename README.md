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
  - [Android APK Analysis](#android-malware-analysis-tooling)
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

### [Android-Malware-Analysis](https://github.com/anpa1200/Android-Malware-Analysis)
AI-powered static analysis framework for Android APK files. Combines YARA rule matching, semantic component name analysis, weighted threat scoring, VirusTotal cross-validation, and multi-provider LLM classification (Claude, OpenAI, Gemini, or local Ollama) — producing MITRE ATT&CK-mapped reports and Frida instrumentation scripts entirely in the terminal. No sandbox, no uploads required.

> 📖 [Full guide on Medium](https://medium.com/@1200km/android-apk-analysis-tool-ai-powered-static-malware-analysis-in-your-terminal-4beb239dad12)

### [AIDebug](https://github.com/anpa1200/AIDebug)
AI-assisted malware reverse engineering debugger. Combines Capstone disassembly, FLIRT signature matching, automatic malware pattern detection (XOR loops, stack strings, API hashing, RDTSC timing, direct syscalls), per-function CFG visualization, and Claude AI analysis — all in a live terminal UI. Optional Frida dynamic mode adds runtime register snapshots, memory diffs, automatic unpacking detection, and network traffic capture. Generates HTML reports with inline CFG SVGs, YARA rules, and JSON export for SIEM/SOAR. Supports remote frida-server for INetSim-isolated sandbox workflows.

> 📖 [Full engineering walkthrough on Medium](https://medium.com/@1200km/ai-powered-malware-debugger-that-explains-every-function-it-sees-2a28ef75df8a)

### [StratusAI](https://github.com/anpa1200/stratus-ai)
AI-powered multi-cloud security scanner for AWS and GCP. Scans 9 AWS modules, 7 GCP modules, and 4 external modules; routes findings through Claude, GPT-4o, or Gemini for attack chain analysis and prioritized reports. Deploys to AWS ECS Fargate or GCP Cloud Run Job via a single interactive wizard.

> 📖 [Full engineering walkthrough on Medium](https://medium.com/@1200km/stratusai-i-built-an-ai-powered-cloud-security-scanner-for-aws-and-gcp-heres-everything-89c6702d3b84)

### [AuditAI](https://github.com/anpa1200/AuditAI)
AI-powered host vulnerability assessment and security auditing in a Dockerized workflow.

### [cvss_4.0](https://github.com/anpa1200/cvss_4.0)
Command-line CVSS v4.0 enrichment tool. Takes CVE IDs and produces CVSS-BTE scores — Base + Threat + Environmental — by pulling live data from CISA KEV, EPSS, and NVD. Outputs severity bands, SLA recommendations, and full BTE vector strings. Six built-in asset profiles: `internet_facing`, `internal_vlan`, `isolated_ot`, `dev_test`, `healthcare_ehr`, `pci_payment`. CSV and JSON export.

> 📖 [CVSS v4.0: The Practical Field Guide for Vulnerability Management](https://medium.com/bugbountywriteup/cvss-v4-0-the-practical-field-guide-for-vulnerability-management-5b5a59728456)

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

### [AIDebug](https://github.com/anpa1200/AIDebug)
AI-assisted malware reverse engineering debugger powered by Claude. Full pipeline: static PE/ELF parsing → recursive-descent disassembly → FLIRT library identification → malware pattern detection → CFG construction → Claude AI function explanation → optional Frida dynamic instrumentation.

Key capabilities:
- **FLIRT matching** — identifies msvcrt, zlib, OpenSSL functions; skips AI for them
- **8 malware patterns** — XOR decryption loops, stack strings, API hash resolution, RDTSC timing checks, direct syscall stubs, NOP sleds, null-safe XOR, Base64 table references
- **CFG visualization** — basic block decomposition; text in TUI, inline SVG in HTML reports
- **Frida dynamic mode** — register/memory snapshots, memory diffs, unpacking detection (VirtualProtect RWX→RX), Winsock + WinInet traffic capture
- **Remote frida-server** (`--frida-host`) — run AIDebug on host with real internet while malware runs in INetSim-isolated VM
- **Reporting** — self-contained HTML report, YARA rules, JSON export for SIEM/SOAR

Supports PE32/PE64/ELF across x86, x86-64, ARM, AArch64, RISC-V.

> 📖 **Article:** [I Built an AI-Powered Malware Debugger That Explains Every Function It Sees](https://medium.com/@1200km/ai-powered-malware-debugger-that-explains-every-function-it-sees-2a28ef75df8a)

### [StratusAI](https://github.com/anpa1200/stratus-ai)
AI-powered multi-cloud security scanner covering AWS (9 modules) and GCP (7 modules) plus external endpoint scanning. Uses Claude, GPT-4o, or Gemini to synthesize findings into attack chains and prioritized remediation. Deploys serverlessly to AWS ECS Fargate or GCP Cloud Run Job via a unified interactive wizard (`wizard.sh`).

Runs a full assessment in 2–4 minutes. Costs ~$0.01–$0.15 per scan depending on model. 125-test suite, zero live cloud calls in CI.

> 📖 **Article:** [StratusAI: I Built an AI-Powered Cloud Security Scanner for AWS and GCP — Here's Everything](https://medium.com/@1200km/stratusai-i-built-an-ai-powered-cloud-security-scanner-for-aws-and-gcp-heres-everything-89c6702d3b84)

### [AuditAI](https://github.com/anpa1200/AuditAI)
AI-powered host vulnerability assessment and security auditing platform designed to support practical security review workflows.

---

## Cyber Threat Intelligence

### [cvss_4.0](https://github.com/anpa1200/cvss_4.0)
CVSS v4.0 enrichment pipeline: pulls live NVD vectors, checks CISA KEV, queries EPSS, applies asset environmental profiles, and outputs CVSS-BTE vectors with severity bands and SLA recommendations. Single dependency (`requests`), six built-in profiles, CSV + JSON output.

> 📖 [CVSS v4.0: The Practical Field Guide for Vulnerability Management](https://medium.com/bugbountywriteup/cvss-v4-0-the-practical-field-guide-for-vulnerability-management-5b5a59728456)

### [CTI](https://github.com/anpa1200/CTI)
Open-source CTI reports with evidence-labeled assessments, defensive guidance, and SOC-oriented research outputs.

---

## Malware Analysis Tooling

### [Android-Malware-Analysis](https://github.com/anpa1200/Android-Malware-Analysis)
Terminal-native APK analysis pipeline: static analysis via androguard, YARA scanning (20 rules covering Anubis, Cerberus, Joker, SpyNote, Metasploit RAT, Stalkerware, and more), semantic component decoding, entropy-based obfuscation detection, VirusTotal lookup, and AI-generated reports with MITRE ATT&CK mappings and Frida hooks. Supports Claude, OpenAI GPT-4o, Google Gemini, and local Ollama.

> 📖 **Article:** [Android APK Analysis Tool: AI-Powered Static Malware Analysis in Your Terminal](https://medium.com/@1200km/android-apk-analysis-tool-ai-powered-static-malware-analysis-in-your-terminal-4beb239dad12)

### [AIDebug](https://github.com/anpa1200/AIDebug)
Step-by-step malware debugger powered by Claude AI. Explains every function — name, summary, parameters, behaviors, MITRE ATT&CK technique, risk level — with optional Frida runtime hooks, memory diffs, unpacking detection, and network traffic capture. See [AI-Powered Security](#ai-powered-security) for full details.

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

- [Android APK Analysis Tool: AI-Powered Static Malware Analysis in Your Terminal](https://medium.com/@1200km/android-apk-analysis-tool-ai-powered-static-malware-analysis-in-your-terminal-4beb239dad12) — practical guide to the Android-Malware-Analysis tool: all 4 analysis phases explained, multi-provider AI setup (Claude/OpenAI/Gemini/Ollama), VirusTotal integration, real SpyNote/SpyMax Frida hook walkthrough, risk scoring formula, batch analysis, and architecture overview. (Mar 2026)

- [CVSS v4.0: The Practical Field Guide for Vulnerability Management](https://medium.com/bugbountywriteup/cvss-v4-0-the-practical-field-guide-for-vulnerability-management-5b5a59728456) — complete practitioner guide: CVSS-B → CVSS-BT → CVSS-BTE lifecycle, exploit maturity decision logic (KEV + EPSS), environmental metric profiles, industry-specific scoring (healthcare, OT/ICS, PCI), Log4Shell/CitrixBleed/MOVEit/Erlang OTP worked examples, CVSS vs SSVC comparison, automation tool. (Mar 2026)

- [Infrastructure Pivoting: How CTI Analysts Expand From a Single IOC to a Full Attacker Network](https://medium.com/@1200km) — field manual for tracing attacker infrastructure: 7 pivot types (passive DNS, reverse IP, ASN/hosting reuse, TLS certificates, subdomain enumeration, Shodan/Censys/FOFA, WHOIS), C2 network tracing worked example, common mistakes, interview-ready answers. Includes `autoWF.py` — automated pivot tool (VirusTotal + SecurityTrails + crt.sh). 32 min read. (Mar 2026)

- [Attribution Methodology: How to Build, Defend, and Challenge a Threat Actor Attribution](https://medium.com/@1200km) — practitioner's guide for CTI analysts: 5-level attribution spectrum, 4 evidence types ranked by strength (IOC overlap → TTP consistency → operator mistakes), false flag detection, APT29/Cozy Bear/SVR worked exercise, confidence model, common mistakes, interview-ready frameworks. (Mar 2026)

- [ATT&CK as a Working Tool: Theory and Hands-On Practical Usage](https://medium.com/@1200km) — practitioner's guide for CTI analysts, detection engineers, and threat hunters: framework anatomy, 14 tactics, 5 hands-on use cases (threat report mapping, gap analysis with Navigator, Sigma + ATT&CK detection engineering, threat hunting, adversary emulation), worked example, tooling reference, and quick-reference cheatsheet. 64 min read. (Mar 2026)

- [I Built an AI-Powered Malware Debugger That Explains Every Function It Sees](https://medium.com/@1200km/ai-powered-malware-debugger-that-explains-every-function-it-sees-2a28ef75df8a) — full walkthrough of AIDebug: FLIRT matching, malware pattern detection, CFG visualization, Frida dynamic hooks, unpacking detection, network traffic capture, INetSim sandbox integration

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

1. [Android-Malware-Analysis](https://github.com/anpa1200/Android-Malware-Analysis) — AI-powered Android APK static analysis (YARA + semantic + VT + Claude/OpenAI/Gemini/Ollama)
2. [AIDebug](https://github.com/anpa1200/AIDebug) — AI-assisted malware debugger (Claude + Frida + Capstone)
3. [StratusAI](https://github.com/anpa1200/stratus-ai) — multi-cloud AI security scanner (AWS + GCP)
4. [AuditAI](https://github.com/anpa1200/AuditAI)
5. [cvss_4.0](https://github.com/anpa1200/cvss_4.0) — CVSS v4.0 BTE enrichment tool (KEV + EPSS + asset profiles)
5. [CTI](https://github.com/anpa1200/CTI)
6. [Static-malware-Analysis-Orchestrator](https://github.com/anpa1200/Static-malware-Analysis-Orchestrator)
7. [Unpacker](https://github.com/anpa1200/Unpacker)
8. [PE-Import-Analyzer](https://github.com/anpa1200/PE-Import-Analyzer)
9. [String-Analyzer](https://github.com/anpa1200/String-Analyzer)
10. [Basic-File-Information-Gathering-Script](https://github.com/anpa1200/Basic-File-Information-Gathering-Script)
11. [Passwords](https://github.com/anpa1200/Passwords)
12. [RTSP-brute-force-tool](https://github.com/anpa1200/RTSP-brute-force-tool)
13. [vulnerable-cloud-lab](https://github.com/anpa1200/vulnerable-cloud-lab)
14. [SystemCheck](https://github.com/anpa1200/SystemCheck)
15. [Malware_analysis](https://github.com/anpa1200/Malware_analysis)
16. [lpi](https://github.com/anpa1200/lpi)
17. [Networking](https://github.com/anpa1200/Networking)

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
