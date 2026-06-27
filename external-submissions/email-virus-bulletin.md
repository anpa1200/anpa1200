# Virus Bulletin Editorial Pitch

To: editorial@virusbulletin.com

Subject: Malware-analysis research/tooling pitch: analyst-validated AI workflows with MalwareGraph and AIDebug

Hello Virus Bulletin editorial team,

I am sharing a malware-analysis tooling and methodology pitch that may be
relevant for a Virus Bulletin article, blog item, or future conference
consideration.

The work consists of two related tools and one integrated platform module:

- MalwareGraph: a safe static malware-analysis service for analyst workstations,
  with password-protected ZIP intake, hashing, string/IOC extraction, PE function
  graph recovery, packer and obfuscation signals, safe static UPX decompression,
  and graph-ready analyst output.
- AIDebug: an AI-assisted malware reverse-engineering debugger that produces
  function-level explanations, behavior tags, ATT&CK mappings, IOC exports, YARA
  seed rules, JSON, and analyst reports.
- AdversaryGraph Malware Analysis: an integrated browser workflow that connects
  malware findings to CTI, ATT&CK/TTP review, IOC enrichment, and analyst
  validation.

The core research question is how to use AI in malware analysis without
outsourcing judgment to the model. The workflow treats AI output as structured
analyst-assistance data and keeps validation gaps explicit: unproven runtime
control flow, missing entrypoint disassembly, unresolved imports, packer layers,
network assumptions, and branch conditions are all surfaced for review.

Links:

- MalwareGraph: https://github.com/anpa1200/malwaregraph
- AIDebug: https://github.com/anpa1200/AIDebug
- AdversaryGraph docs: https://1200km.com/adversarygraph-docs/
- Malware analysis docs: https://1200km.com/adversarygraph-docs/malware-analysis
- External validation: https://1200km.com/external-validation.html

Possible article angle:

"AI-assisted malware analysis with explicit validation gaps: building feedback
loops around static triage, debugger-style function stepping, and dynamic
behavior summaries."

I can provide screenshots, sample output using inert test files, or a more
formal article outline if this is of interest.

Best regards,
Andrey Pautov
https://github.com/anpa1200
https://1200km.com/
