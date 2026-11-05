SOC Investigation Checklist

Authentication Analysis

- [ ] Identify failed logon events (4625).
- [ ] Identify successful logon events (4624).
- [ ] Check repeated failures from the same IP.
- [ ] Correlate failed and successful logons.
- [ ] Review logon types.

Privilege Analysis

- [ ] Identify special privilege events (4672).
- [ ] Verify the account associated with privilege assignment.

Process Analysis

- [ ] Identify process creation events (4688).
- [ ] Review process names.
- [ ] Examine parent-child relationships.
- [ ] Review command-line arguments.

Timeline Analysis

- [ ] Arrange events chronologically.
- [ ] Correlate authentication and process activity.
- [ ] Record suspicious sequences.

Final Reporting

- [ ] Document findings.
- [ ] Map relevant MITRE ATT&CK techniques.
- [ ] Provide recommendations.
- [ ] State investigation limitations.

Data Source

Simulated Windows Security Event dataset — SOC-WIN-001.