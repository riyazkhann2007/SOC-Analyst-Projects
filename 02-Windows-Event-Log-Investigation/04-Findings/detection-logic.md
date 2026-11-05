Windows Authentication Detection Logic

Case ID

SOC-WIN-001

Detection 1: Repeated Failed Logons

Windows Event ID: 4625

Detection idea:

Generate an alert when an account experiences five or more failed logon attempts from the same source IP within ten minutes.

Pseudocode

GROUP failed logon events BY:
    Username
    Source IP

TIME WINDOW: 10 minutes

CONDITION:
    Failed logon count >= 5

ACTION:
    Generate authentication alert

Detection 2: Failed Logons Followed by Successful Logon

Windows Event IDs: 4625 and 4624

Detection idea:

Identify an account that experiences repeated failed logons followed by a successful logon from the same source IP within a defined time window.

Pseudocode

IF:
    5 or more Event ID 4625
    for the same username and source IP
    within 10 minutes

AND:
    Event ID 4624 occurs for the same
    username and source IP

THEN:
    Generate high-priority investigation alert

Detection 3: Privilege Assignment

Windows Event ID: 4672

Investigate special privilege assignments associated with accounts showing suspicious authentication activity.

Detection 4: Suspicious Process Creation

Windows Event ID: 4688

Review process creation events for unexpected command-line activity, suspicious PowerShell execution and unusual parent-child relationships.

False Positive Considerations

- Legitimate users may enter incorrect passwords.
- Shared systems may generate multiple authentication failures.
- Administrative scripts may launch command-line tools.
- Privileged accounts may legitimately generate Event ID 4672.

Important Testing Note

These are educational detection concepts, not deployed or tested production rules.

The existing simulated dataset contains four failed logons, so it does not meet the proposed five-failure threshold. The suspicious sequence can still be investigated manually.

Recommended Data Sources

- Windows Security Event Logs
- Windows Event ID 4624
- Windows Event ID 4625
- Windows Event ID 4672
- Windows Event ID 4688
- Endpoint Detection and Response telemetry

Analyst Recommendation

Correlate authentication, privilege assignment and process creation events instead of investigating each event in isolation.