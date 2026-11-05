Lessons Learned – Malicious URL Investigation

1. Threat Intelligence

Using multiple intelligence sources such as URLhaus and VirusTotal provides better context than relying on a single reputation score.

2. IOC Analysis

A useful investigation records URLs, domains, IP addresses and hashes with their correct source and type.

3. Evidence Validation

A favicon hash must not be confused with the hash of a downloaded payload. Every indicator should be labelled accurately.

4. SOC Investigation

A malicious URL detection should lead to further investigation of DNS activity, proxy logs, downloads and endpoint alerts.

5. Incident Response

Recommended actions include blocking malicious indicators, identifying affected endpoints, preserving evidence and escalating confirmed suspicious activity.

6. Detection Engineering

Threat intelligence can be integrated into SIEM monitoring to identify access to known malicious URLs.

7. Investigation Limitations

A malicious URL reputation does not automatically prove that a user was infected. Endpoint telemetry is required to establish impact.

Final Learning Outcome

This investigation improved my understanding of threat intelligence, IOC documentation, URL reputation analysis, SOC triage, incident response recommendations and basic SIEM detection logic.

Project Type: Educational public threat-intelligence investigation.