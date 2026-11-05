Windows Event Log Investigation | SOC Project

"SOC" (https://img.shields.io/badge/Domain-Cybersecurity-blue)
"Project" (https://img.shields.io/badge/Project-Windows%20Log%20Analysis-green)
"Status" (https://img.shields.io/badge/Status-Educational-orange)

1. Project Overview

This project demonstrates a Windows Security Event Log investigation workflow relevant to a Security Operations Center (SOC) Analyst.

The investigation focuses on authentication monitoring, suspicious login patterns, Windows process creation, event correlation, and security incident reporting.

Dataset notice: All event records are simulated for educational purposes. No real production endpoint or organisation was accessed.

2. Investigation Objectives

- Analyse successful and failed Windows logons.
- Identify repeated authentication failures.
- Investigate potentially suspicious login activity.
- Examine Windows process creation events.
- Correlate security events using timestamps.
- Map relevant activities to MITRE ATT&CK.
- Prepare an investigation report with recommendations.

3. Tools and Technologies

- Windows Security Event Logs
- Windows Event Viewer concepts
- GitHub
- CSV sample datasets
- MITRE ATT&CK Framework

4. Windows Event IDs

- 4624 — Successful logon
- 4625 — Failed logon
- 4672 — Special privileges assigned
- 4688 — Process creation
- 1102 — Security audit log cleared

5. Project Structure

Investigation Modules

1. "Windows Logon Activity" (01-Logon-Activity/README.md)
2. "Windows Process Creation" (02-Process-Creation/README.md)
3. "Investigation Timeline" (03-Investigation-Timeline/README.md)
4. "Investigation Findings" (04-Findings/README.md)

Supporting Files

- "Simulated Windows Security Events" (evidence/windows_security_events.csv)
- "Dataset Description" (evidence/dataset-description.md)
- "Windows Event Log Reference" (evidence/event-log-reference.md)
- "Investigation Report" (04-Findings/investigation-report.md)
- "MITRE ATT&CK Mapping" (04-Findings/mitre-attack-mapping.md)
- "Final Conclusion" (04-Findings/final-conclusion.md)
- "Investigation Checklist" (04-Findings/investigation-checklist.md)

6. Investigation Scenario

The simulated dataset contains:

- Four failed login attempts against the admin account.
- A successful network logon following those failures.
- A special privileges assignment event.
- Process creation events involving cmd.exe and powershell.exe.

The sequence is treated as suspicious and requires further investigation. It does not establish that an actual attack occurred.

7. MITRE ATT&CK Relevance

Potentially relevant techniques:

- T1110 — Brute Force
- T1078 — Valid Accounts
- T1059 — Command and Scripting Interpreter

These mappings are preliminary and based on simulated activity.

8. Investigation Outcome

Assessment: Suspicious Activity — Further Investigation Required

Recommended actions include validating the successful login, reviewing privilege assignments, examining process command lines, and correlating additional endpoint and network telemetry.

9. Project Limitations

- Uses simulated event records.
- Does not include real endpoint telemetry.
- No live SIEM investigation was performed.
- No real incident response actions were executed.

10. Learning Outcomes

- Windows authentication event analysis.
- Security Event ID identification.
- Process creation investigation.
- Event timeline reconstruction.
- Basic threat mapping using MITRE ATT&CK.
- SOC investigation documentation and reporting.

---

Author: Riyaz
Project: SOC Analyst Portfolio — Project 02