# Help Net Security Pitch

To: press@helpnetsecurity.com

Subject: Open-source AI-assisted CTI and malware-analysis platform release: AdversaryGraph v4, MalwareGraph, AIDebug

Hello Help Net Security team,

I am sharing a new open-source/source-available security research and tooling
release that may fit your audience of security practitioners and analysts:
AdversaryGraph v4, with the related MalwareGraph and AIDebug malware-analysis
workflow.

AdversaryGraph is an AI-assisted CTI-to-detection workbench for ATT&CK mapping,
actor similarity analysis, IOC enrichment, detection-gap review, STIX/OpenCTI
handoff, and analyst validation. The v4 release adds a full Malware Analysis
module with safe static analysis, decompilation/debug workflow views, clickable
ATT&CK/TTP pivots, AI-assisted dynamic-analysis summaries, and analyst-ready
malware research output.

Related tools:

- MalwareGraph: standalone safe static malware-analysis service for Linux/REMnux-style analyst workstations.
- AIDebug: AI-assisted malware reverse-engineering debugger that produces function summaries, ATT&CK tags, IOC output, YARA seeds, and analyst reports.

Links:

- Project hub: https://1200km.com/adversarygraph/
- Documentation: https://1200km.com/adversarygraph-docs/
- Live threat matrix: https://1200km.com/threat-matrix/
- AdversaryGraph repo: https://github.com/anpa1200/adversarygraph
- MalwareGraph repo: https://github.com/anpa1200/malwaregraph
- AIDebug repo: https://github.com/anpa1200/AIDebug
- External validation: https://1200km.com/external-validation.html

Key angle:

This is not positioned as an autonomous malware verdict engine. The project is
built around analyst validation: every AI-generated mapping, malware summary,
similarity lead, and attribution hint is treated as an investigation lead that
must be checked against evidence.

I can provide screenshots, a short walkthrough, or a technical Q&A if useful.

Best regards,
Andrey Pautov
https://github.com/anpa1200
https://1200km.com/
