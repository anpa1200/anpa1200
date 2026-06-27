# Hacker News / Show HN Submission

Submit: https://news.ycombinator.com/submit

## Title

Show HN: AdversaryGraph - AI-assisted CTI and malware-analysis workbench

## URL

https://1200km.com/adversarygraph/

## First Comment

I built AdversaryGraph as an analyst-focused CTI-to-detection workbench.

It connects ATT&CK mapping, actor similarity, IOC enrichment, detection-gap
review, STIX/OpenCTI handoff, and malware-analysis workflows in one browser
workspace. The new v4 release adds a malware-analysis module with safe static
analysis, decompilation/debugger-style views, clickable TTP pivots, and
AI-assisted function/dynamic-analysis summaries.

The main design decision is that AI output is not treated as truth. It is
analyst-assistance data. The UI keeps validation gaps visible: unproven runtime
execution, unresolved imports, packer layers, missing entrypoint disassembly,
branch conditions, and uncertain ATT&CK mappings.

Docs: https://1200km.com/adversarygraph-docs/
Repo: https://github.com/anpa1200/adversarygraph
MalwareGraph: https://github.com/anpa1200/malwaregraph
AIDebug: https://github.com/anpa1200/AIDebug

I am especially interested in feedback from people who do CTI, detection
engineering, malware triage, or OpenCTI/MISP/STIX workflows.
