# Black Hat Europe 2026 Briefings Portal Submission

Portal: https://blackhat.com/call-for-papers.html

Status: Black Hat Europe 2026 Call for Briefings is open June 3-July 22, 2026.

## Talk Title

Analyst-Validated AI for CTI and Malware Analysis: Feedback Loops, Validation Gaps, and Graph-Ready Detection Handoff

## Track

Defense / Malware / AI / Threat Intelligence

## Abstract

AI is useful in CTI and malware analysis only when the workflow makes uncertainty
visible. This talk presents AdversaryGraph v4, MalwareGraph, and AIDebug as a
practical architecture for analyst-validated AI: static and dynamic malware
findings are converted into graph-ready entities, ATT&CK/TTP candidates, IOC
pivots, detection leads, and explicit validation gaps instead of final
autonomous verdicts.

The talk shows how to build feedback loops around static triage, function-level
reverse engineering, dynamic behavior summaries, CTI enrichment, and detection
engineering. It covers failure modes such as hallucinated ATT&CK mappings,
unproven runtime control flow, unresolved imports, packer layers, false actor
similarity, and unsupported attribution. The result is a methodology for using
AI to accelerate analyst work while preserving evidence, uncertainty, and human
review.

## Outline

1. Why autonomous AI malware verdicts fail.
2. Architecture: AdversaryGraph, MalwareGraph, AIDebug, IOC/TTP graph pivots.
3. Static analysis workflow: PE metadata, strings, imports, packer signals,
   function graph recovery.
4. Dynamic workflow: process creation, file writes/deletes, registry changes,
   network attempts, DNS lookups, API calls, memory allocation, loaded modules,
   injected code, persistence, command execution, and branch decisions.
5. AI feedback loops: ask, verify, step, test, re-rank, and summarize.
6. Validation gaps as first-class output.
7. Detection handoff: Sigma/YARA/STIX/OpenCTI/Navigator outputs.
8. Lessons learned from building the platform.

## Speaker Bio

Andrey Pautov is a cybersecurity researcher and builder focused on CTI,
ATT&CK-driven detection engineering, malware-analysis workflows, and
AI-assisted analyst tooling. He maintains the 1200km security research ecosystem,
including AdversaryGraph, MalwareGraph, AIDebug, CTI research reports, and
detection-engineering projects.

## Links

- Project hub: https://1200km.com/adversarygraph/
- Docs: https://1200km.com/adversarygraph-docs/
- Repo: https://github.com/anpa1200/adversarygraph
- MalwareGraph: https://github.com/anpa1200/malwaregraph
- AIDebug: https://github.com/anpa1200/AIDebug
