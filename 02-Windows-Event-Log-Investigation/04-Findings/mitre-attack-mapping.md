MITRE ATT&CK Mapping

Investigation Case: SOC-WIN-001

This document maps observed simulated activities to relevant MITRE ATT&CK techniques.

1. Brute Force

- Tactic: Credential Access
- Technique: T1110 — Brute Force
- Observation: Multiple failed login attempts followed by a successful login.
- Status: Potentially relevant; requires further investigation.

2. Valid Accounts

- Tactic: Initial Access
- Technique: T1078 — Valid Accounts
- Observation: A successful login occurred after repeated failures.
- Status: Possible account misuse; not confirmed.

3. Command and Scripting Interpreter

- Tactic: Execution
- Technique: T1059 — Command and Scripting Interpreter
- Observation: cmd.exe and powershell.exe appear in simulated process creation events.
- Status: Requires command-line and parent-process analysis.

Disclaimer

These are preliminary mappings based on simulated data. They do not establish that an attack occurred.