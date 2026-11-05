Windows Event Timeline Analysis

Case ID: SOC-WIN-001

1. Overview

This timeline analyses the sequence of simulated Windows Security Events.

2. Key Observations

- 09:00 — Normal interactive logon by riyaz.
- 09:05–09:06 — Four failed logon attempts against admin.
- 09:07 — Successful network logon for admin from the same source IP.
- 09:08 — Special privileges assigned to admin.
- 09:10 — cmd.exe process created.
- 09:11 — powershell.exe process created.

3. Suspicious Sequence

Repeated failed authentication attempts were followed by successful access, privilege assignment and command-line process activity.

4. Assessment

This sequence warrants further investigation for possible brute-force activity and account compromise.

5. Recommended Investigation

- Validate whether the successful login was authorised.
- Review the account's privilege assignment.
- Examine process command-line arguments.
- Correlate additional endpoint and network logs.

6. Data Source

Simulated Windows Security Events — SOC-WIN-001.

7. Disclaimer

This is an educational investigation using simulated records. The sequence does not prove a real attack.